# discuss-plan-edge-cases

Complication manual for the `discuss-plan` skill. This file handles situations that fall outside the standard workflow in `discuss-plan.md`. It is read selectively — only when `discuss-plan.md` encounters a specific complication and references this file.

This file is **not a workflow**. It contains no phases, no sequence logic, no templates. Each section is a named trigger condition paired with a specific handling protocol. Tools (matrices, tables, frameworks) live in `discuss-plan-frameworks.md`; this file references them by name when needed.

-----

## 1. Mixed Methods Integration

**[Triggered when: included papers use fundamentally different methods]**

**Problem**: qualitative and quantitative papers cannot be forced into the same thematic claim without misrepresenting what each method can support. Parallel reporting without integration is equally wrong.

### Two-stage synthesis protocol

#### Stage 1 — Within-method synthesis

- Synthesize qualitative papers together: what patterns, themes, or mechanisms emerge from the qualitative strand?
- Synthesize quantitative papers together: what associations, effect sizes, or patterns emerge from the quantitative strand?
- Each strand produces its own internal synthesis first.

#### Stage 2 — Cross-method integration

Ask the student:

- "Where do the qualitative and quantitative strands converge? What does that convergence mean?"
- "Where do they diverge? Is the divergence methodological, contextual, or substantive?"
- "What does each strand show that the other cannot? What is only visible when both are read together?"

### Integration framing to offer

> "Because your papers use different methods, I suggest we first synthesize what the [qualitative/quantitative] papers show together, then interpret what changes when we read both strands side by side. This prevents forcing incompatible evidence into one claim prematurely."

### Epistemological tension check

If methods come from incompatible epistemological traditions (e.g., positivist RCT + constructivist grounded theory), ask:

> "Your papers come from epistemologically different traditions. How do you explain using both — do you see this as pragmatic triangulation, or do you have a theoretical justification for combining them?"

This question matters for the examiner.

-----

## 2. Conflicting Findings Across Papers

**[Triggered when: papers produce results that contradict each other]**

**Reframe immediately**: contradiction is not a weakness. It is information about boundary conditions, moderating variables, or methodological differences. Examiners expect contradictions in serious multi-paper theses. Ignoring them is the actual problem.

### Handling protocol

#### Step 1 — State the contradiction clearly and specifically

> "Papers X and Y report conflicting findings on [specific point]. Paper X found [A] in [context]. Paper Y found [B] in [context]."

#### Step 2 — Comparative analysis

Ask:

- "How do the populations or settings differ between these studies?"
- "How do the methods or measures differ?"
- "Which study has the stronger design for this specific question?"
- "Could both findings be true — in different conditions?"

#### Step 3 — Determine contradiction type

- **Type A — Methodological artifact**: the contradiction is explained by design differences. One finding is more robust. Name which one and why.
- **Type B — Genuine boundary condition**: both findings are valid in their respective contexts. Name the moderating factor.
- **Type C — Unresolved**: the evidence is genuinely insufficient to adjudicate. This becomes a future research direction.

#### Step 4 — Frame in the discussion

- **For Type A**: "Paper X's finding appears more robust because [design reason]. Paper Y's divergent finding may reflect [methodological explanation]."
- **For Type B**: "The divergence between Papers X and Y suggests this effect is conditional on [factor]. In [context A] we observe [A]; in [context B] we observe [B]."
- **For Type C**: "These conflicting findings cannot be resolved with current evidence. Future research should [specific design]."

### Instruction for Claude

Never smooth over contradictions to produce a cleaner narrative. An examiner will find them. Addressing them directly is always better than hoping they go unnoticed.

-----

## 3. Papers with Different Aims or Variables

**[Triggered when: included papers address different questions or measure different outcomes]**

**Problem**: students often feel their thesis lacks coherence when papers address different aims. Usually, the coherence exists at a level above the individual paper aims — at the overarching question level.

### Linking logic protocol

#### Step 1 — Return to the overarching research question

> "Let's hold all the individual paper aims aside for a moment. What single question is your thesis, as a whole, trying to answer?"

#### Step 2 — Map each paper's aim to a sub-question of that overarching question

> "If your overarching question is [X], what part of that question does Paper 1 address? What part does Paper 2 address?"

#### Step 3 — Build the linking logic statement together

> "Although the papers address different aims, they contribute to the same overarching question by answering complementary sub-questions. Paper 1 establishes [X], which provides the basis for Paper 2's analysis of [Y]. Paper 3 extends this by examining [Z] in [context]. Synthesized together, these studies support the thesis-level claim that [claim], while showing it is conditional on [boundary condition]."

#### Step 4 — Flag papers that cannot link

If a paper cannot be linked to any sub-question of the overarching question even after this exercise, flag it:

> "Paper [X] does not appear to answer any part of your overarching question, even as a sub-question. Should it remain in the thesis, or is it better placed as a published work that sits outside this particular thesis argument?"

-----

## 4. Unpublished Papers at Time of Skill Use

**[Triggered when: one or more included papers are in prep, under review, or accepted but not yet in print]**

**Risk**: building core thesis claims on results that are not yet fully documented, peer-reviewed, or stable creates vulnerability at examination.

### Handling protocol

#### Step 1 — Identify and label clearly

> "Paper [X] is currently [in prep / under review / accepted but not in print]. I'll flag this throughout our planning."

#### Step 2 — Assess dependency

Ask: "Is any core thesis claim dependent primarily on this paper's findings, rather than supported by multiple papers?"

If yes, flag explicitly:

> "Your claim that [X] currently rests primarily on Paper [Y], which is not yet published. If that paper is rejected, revised substantially, or its findings change, this affects the thesis argument. Can we identify additional support from other papers, or should this claim be treated as tentative?"

#### Step 3 — Label throughout outputs

- In Deliverable 1 and the Handoff Block, label all unpublished papers with their status.
- In the outline, mark claims that depend on unpublished work with a flag: `[DEPENDS ON UNPUBLISHED: Paper X]`.

#### Step 4 — Advise on language calibration

> "For claims supported primarily by unpublished work, use appropriately tentative language: 'preliminary findings suggest' rather than 'this thesis demonstrates.'"

-----

## 5. Fast-Forward Protocol for Returning Users

**[Triggered when: student has prior phase outputs and wants to resume or skip ahead]**

**Problem**: strict phase sequence frustrates advanced users who already have a completed synthesis table or outline, or who are resuming an interrupted session.

### Fast-forward rules

- Fast-forward is permitted **only** when the student can produce the output of the phase they want to skip.
- Claude must verify the prior output meets the completion criteria of the skipped phase (from `discuss-plan.md`) before proceeding.
- If prior output is incomplete, Claude names what is missing and offers to complete only those items — not repeat the whole phase.

### Protocol

#### Step 1 — Ask the student what they already have

> "Before we start, tell me what work you've already done — do you have a paper inventory, confirmed themes, a thesis-level claim, or an outline already drafted?"

#### Step 2 — For each completed phase output provided

- Verify it meets the completion criteria (from `discuss-plan.md`).
- If complete: accept and update working state.
- If incomplete: identify the specific gap and address only that.

#### Step 3 — Restate updated working state

Use the working state block from `discuss-plan.md` (Rule 6) before continuing.

#### Step 4 — Resume from the earliest incomplete phase

### Example handling

> "You have a confirmed paper inventory and a preliminary theme list — that covers Phases 0 and 1 partially. I'm missing confirmation that every paper maps to a theme, and I don't yet see a thesis-level claim. Let me check the theme–paper mapping first, then we'll develop the claim together."

-----

## 6. Student Resists Excluding Papers

**[Triggered when: student is emotionally or professionally attached to papers that the selection criteria suggest excluding]**

This is common. Papers represent years of work. Exclusion can feel like devaluation.

### Handling protocol

#### Step 1 — Acknowledge the work without capitulating

> "This is clearly a strong piece of work. The question isn't whether it's good research — it's whether it belongs in this particular thesis argument."

#### Step 2 — Reframe exclusion

> "A paper excluded from this thesis is not diminished. It still exists, is still published, and still contributes to your record. The thesis is a curated argument, not a complete bibliography."

#### Step 3 — Test examiner defensibility directly

> "If an examiner asks why this paper is included, what would you say? If the answer is 'because I wrote it' rather than 'because it answers [specific part of the thesis argument],' that's a signal."

#### Step 4 — Offer an alternative

> "If you want to acknowledge this paper without making it a core chapter, you could reference it briefly in the introduction as context, or in the discussion as a related finding — without it being a primary evidence source for your thesis claims."

#### Step 5 — Respect autonomy

If the student insists on including it anyway:

- Accept the decision.
- Flag it in the working state as `included despite weak thematic fit`.
- Ensure this is visible in the handoff block.
- Do not override the student's autonomy. Document the decision.

-----

## 7. Thesis with Only Two Papers

**[Triggered when: the included paper set is very small (n=2 or n=3)]**

**Risk**: with only two papers, cross-paper synthesis is thin. Single-paper themes are almost unavoidable. Examiner expectations for "integration" are harder to meet.

### Handling protocol

#### Step 1 — Reframe what integration means at this scale

> "With two papers, your integrative discussion will look different from a thesis with six papers. The integration question becomes: what does the combination of these two papers show that neither shows alone — and is that combination greater than the sum of its parts?"

#### Step 2 — Push harder on the literature positioning layer

> "With a small internal evidence base, the external positioning work becomes more important. Your discussion needs to show that even with two papers, you are making a specific contribution to the field's understanding of [topic]. The literature positioning table becomes load-bearing here."

Use the **Literature Positioning Table** from `discuss-plan-frameworks.md` with extra rigor.

#### Step 3 — Explore whether additional integrative chapters exist

> "Does your thesis include any additional integrative chapters beyond the papers — general introduction, methods overview, clinical context chapters? These can carry synthesis weight that doesn't fall entirely on the discussion."

#### Step 4 — Scope calibration becomes critical

With a thin evidence base, overclaiming is especially risky. Apply the **Scope Calibration Framework** from `discuss-plan-frameworks.md` rigorously to every major claim.
