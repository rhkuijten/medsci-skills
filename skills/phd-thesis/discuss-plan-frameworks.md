# discuss-plan-frameworks

Knowledge library for the `discuss-plan` skill. This file contains all templates, tables, archetypes, positioning tools, scope calibration, and examiner models used across the workflow.

This file is **not a workflow**. It contains no phases, no rules, no sequence logic. It is the instrument tray; `discuss-plan.md` is the operating protocol. When `discuss-plan.md` instructs Claude to use a specific template or framework, Claude reads it from here.

-----

## 1. Papers-to-Aims Matrix

**[Used in: Phase 3B]**

Purpose: map each included paper to the thesis aims and confirm its contribution at thesis level.

|Paper|Thesis Aim / Sub-Question|Method|Key Finding (1 sentence)|Contribution to Thesis Claim|
|-----|-------------------------|------|------------------------|----------------------------|
|     |                         |      |                        |                            |

### Filling rules

- **Key Finding**: one sentence only. If student writes a paragraph, ask them to reduce to one sentence before proceeding.
- **Contribution to Thesis Claim**: must be thesis-level. If student writes a paper-level finding, ask: *"What does this finding let you argue at the level of the whole thesis?"*
- **Papers not mapping to any aim**: flag immediately.

> "This paper doesn't appear to connect to any of your thesis aims — should it be reconsidered for exclusion?"

-----

## 2. Thematic Synthesis Table

**[Used in: Phase 3B]**

Purpose: map evidence across papers per theme, identify interpretations and boundary conditions.

|Theme|Paper 1 Evidence|Paper 2 Evidence|Paper 3+ Evidence|Thesis-Level Interpretation|Boundary Conditions|Support Strength|
|-----|----------------|----------------|-----------------|---------------------------|-------------------|----------------|
|     |                |                |                 |                           |                   |                |

### Filling rules

- **Each theme**: evidence from at least 2 included papers required. Single-paper themes are flagged:

> "This theme currently rests on only one paper. That belongs in the individual paper's discussion, not the integrative chapter. Can we find a second paper that speaks to this, or should we absorb this into another theme?"
- **Thesis-Level Interpretation**: what the pattern means for the overarching argument — not a paper summary.
- **Boundary Conditions**: where the claim holds and where it does not. Contradictions between papers are named here, **not resolved away**.
- **Support Strength**:
  - `Strong` = multi-paper, multi-method.
  - `Tentative` = single paper or single methodological strand only.
  - Always label this explicitly.

-----

## 3. Literature Positioning Table

**[Used in: Phase 1C and Phase 3B]**

Purpose: position each theme against existing field knowledge. Prevents internally focused synthesis that ignores the broader field.

|Theme|Existing Field Consensus|Thesis Contribution|Implication for Field|Prior Work Contradicted (if any)|
|-----|------------------------|-------------------|---------------------|--------------------------------|
|     |                        |                   |                     |                                |

### Filling rules

- **Existing Field Consensus**: what the field believed or assumed before this thesis. If the student is unsure, ask:

> "What would a review paper written before your first study have concluded about this question?"
- **Thesis Contribution**: what the thesis adds, shifts, or challenges. Must be specific — *"confirms existing knowledge"* is not a contribution.
- **Implication for Field**: what changes in how the field should think, practice, or research because of this thesis.
- **Prior Work Contradicted**: name specific studies or consensus positions the thesis contradicts. If none, ask whether this is because the thesis genuinely confirms everything — or because the student has not looked hard enough for contradictions.

-----

## 4. Scope Calibration Framework

**[Used in: Phase 1D and Phase 3B]**

Purpose: explicitly bound all major claims to prevent overclaiming, inflated generalization, and false coherence.

For each major thesis claim, map all four dimensions:

### Population scope

- Who does this finding apply to?
- Which patient groups, demographics, clinical contexts?
- Who was explicitly excluded from the studies?

### Contextual scope

- In what settings does this apply? (hospital type, country, resource setting, time period)
- What implementation conditions are assumed?

### Inferential scope

- What can be directly inferred from the data?
- What is extrapolation beyond the data?
- What is hypothesis or speculation?
- Label each claim: `directly supported` / `plausible extension` / `speculative`.

### Causal scope

- Is this a correlation, association, or causal claim?
- What is the inferential basis? (RCT, observational, mechanistic)
- What confounding cannot be excluded?
- If causal language is used in an observational thesis, flag:

> "This design supports association, not causation. The language should reflect that."

### Calibration instruction for Claude

When a student makes a claim that exceeds its inferential basis, say directly:

> "That claim extends beyond what your study design can support. Let's reframe it as [weaker, accurate version]."

Do not smooth over this. Scope overclaiming is an examiner red flag.

-----

## 5. Discussion Architecture Archetypes

**[Used in: Phase 3A]**

Purpose: help the student choose the right discussion structure before building the outline. Thematic synthesis is not always optimal.

### Archetype 1 — Thematic synthesis (default)

- **Structure**: organize by cross-paper themes, not paper sequence.
- **Best for**: theses with papers that address related questions using different methods or populations, where patterns emerge across papers.
- **Fails when**: thesis is a sequential research program where each paper depends on the previous one.

### Archetype 2 — Chronological / research program evolution

- **Structure**: organize by how the research program developed — what each stage revealed that motivated the next.
- **Best for**: theses where papers build sequentially (validation study → clinical trial → implementation), or where the intellectual evolution of the program is itself a contribution.
- **Fails when**: papers are thematically parallel rather than sequential.

### Archetype 3 — Theory-driven structure

- **Structure**: organize around a theoretical framework — how the thesis tests, extends, or refines a specific theory or model.
- **Best for**: theses with a strong theoretical grounding where papers are designed to address theoretical questions.
- **Fails when**: thesis is primarily empirical/applied with weak theoretical framing — forcing theory onto atheoretical work produces hollow claims.

### Archetype 4 — Methods-first structure

- **Structure**: organize by methodological contribution before substantive findings — what the thesis's methodological advances enable.
- **Best for**: theses that make a primary contribution to methodology (new measurement tools, new analytical approaches, new study designs).
- **Fails when**: methodological contribution is secondary to substantive findings.

### Archetype 5 — Translational / clinical implications structure

- **Structure**: organize around the pathway from evidence to practice or policy — what the combined findings mean for clinical decision-making, guidelines, or health systems.
- **Best for**: clinical and health services theses where the practical implications are the central contribution.
- **Fails when**: thesis is primarily mechanistic or theoretical with limited direct clinical application.

### Archetype 6 — Problem-solution architecture

- **Structure**: organize around a defined problem and how the thesis progressively builds a solution.
- **Best for**: theses framed around a specific clinical or practical problem (e.g., underdiagnosis, treatment failure, implementation gap) where papers collectively build toward an answer.
- **Fails when**: papers address different problems rather than different aspects of one problem.

### Selection guidance for Claude

Present all archetypes briefly. Ask:

> "Which of these fits your thesis best, and why?"

If the student is unsure, ask:

> "Does the relationship between your papers feel more like parallel investigations of related questions, or like a sequential program where each paper built on the last?"

That distinction usually separates thematic from chronological.

**Note on hybrids**: hybrid architectures are legitimate. A thesis can be primarily thematic within a translational framing, for example. If a hybrid emerges, name it explicitly and sketch how it works.

-----

## 6. Examiner Model Calibration

**[Used in: Phase 1A and Phase 3A]**

Purpose: calibrate the discussion's argumentative style to the discipline and likely examiner. A clinical ML thesis and a qualitative sociology thesis require fundamentally different rhetorical behavior.

### Dimension 1 — Disciplinary epistemology

**Quantitative / biomedical orientation**

- Examiners expect: statistical evidence, effect sizes, confidence intervals, calibration.
- Argument style: empirical, evidence-graded, cautious causal language.
- Danger zones: overclaiming causation, ignoring confounding, underpowered claims.

**Qualitative / interpretive orientation**

- Examiners expect: thick description, theoretical saturation, reflexivity, transferability not generalizability.
- Argument style: interpretive, contextual, epistemologically explicit.
- Danger zones: positivist language, false quantification, ignoring researcher positionality.

**Mixed methods orientation**

- Examiners expect: explicit integration logic, epistemological coherence across strands, explanation of what each method adds.
- Argument style: integrative, explicit about strand complementarity.
- Danger zones: parallel reporting without integration, ignoring epistemological tensions.

**AI / computational methods orientation**

- Examiners expect: TRIPOD+AI or equivalent reporting, calibration evidence, external validation, clinical applicability.
- Argument style: technical precision, explicit performance limitations, deployment context.
- Danger zones: inflated performance claims, ignoring dataset shift, conflating model performance with clinical utility.

### Dimension 2 — Examiner type

**Methodologist examiner**

- Primary focus: are the methods defensible? Are the inferential claims calibrated to design?
- Key preparation: have a ready answer for every methodological limitation; pre-empt the attack.

**Clinical / applied examiner**

- Primary focus: does this change practice? Is the evidence strong enough to act on?
- Key preparation: clear translational pathway; realistic scope of recommendations.

**Theoretical examiner**

- Primary focus: does this contribute to theory? Is the theoretical framing coherent?
- Key preparation: explicit theoretical positioning; engagement with the relevant theoretical literature.

**Generalist examiner**

- Primary focus: is the thesis coherent and well-argued as a whole?
- Key preparation: clarity, signposting, accessible synthesis.

### Using the examiner model

After identifying discipline and examiner type, Claude produces a brief examiner model summary:

> "Based on your field and thesis type, your examiner is likely a [type] who will focus on [primary concerns]. The argumentative style that works best here is [style]. The most likely attack on your thesis is [attack]. We should make sure the discussion pre-empts this by [specific approach]."

-----

## 7. Contribution Statement Template

**[Used in: Phase 3A — deploy only if student is stuck]**

> "Taken together, these studies show that **[main thesis-level finding]**. Across the papers, the evidence suggests **[pattern or mechanism]**, particularly in **[context/population]**. This thesis contributes **[theoretical contribution]** by **[how it advances / clarifies / challenges existing work]**, and contributes **[practical contribution]** by **[implication for practice / policy / decision-making]**. At the same time, the findings are bounded by **[main limitation or uncertainty]**, so conclusions should be interpreted as **[calibrated claim]** rather than **[overstated claim]**."

### Instruction for Claude

Introduce this template only when the student has tried and failed to articulate a thesis-level claim. Say:

> "Let me offer a scaffold — you fill in the blanks, and we'll refine from there."

**Never fill in the blanks for the student.**

-----

## 8. Future Research Taxonomy

**[Used in: Phase 3B]**

Purpose: derive future research that is directly implied by the thesis — not generic filler.

### Valid derivation sources (use as prompts)

- **Unresolved contradictions**: *"Papers X and Y conflict on [point]. What study design would resolve that?"*
- **Methodological gaps**: *"All your papers use [method]. What would a study using [different method] add?"*
- **Untested populations**: *"Your findings apply to [population]. Which populations were excluded and need testing?"*
- **Mechanistic uncertainty**: *"You show association but not mechanism. What mechanistic study is implied?"*
- **Implementation barriers**: *"Your findings support [intervention]. What is the barrier to implementation, and what study would address it?"*
- **Replication needs**: *"Which findings rest on a single study and need independent replication?"*

### Distinction to enforce

- **Generic (not acceptable)**: "Future research should investigate larger samples."
- **Thesis-implied (required)**: "The conflicting findings between Papers 2 and 4 regarding [X] suggest a study directly comparing [condition A] and [condition B] in a prospectively designed cohort would resolve this."

-----

## 9. Common Pitfalls Checklist

**[Used in: Phase 4 — run with student before Deliverable 2]**

Claude works through this checklist interactively with the student, not as a passive list to hand over.

- ☐ Outline organized by themes, not paper sequence? (Paper 1 → Paper 2 → Paper 3 structure = fail)
- ☐ Opening summary answers the research question at thesis level? (Not paper-by-paper summaries)
- ☐ Every theme supported by at least 2 included papers?
- ☐ Contradictions named as boundary conditions, not ignored?
- ☐ Limitations stated at project level, not only paper level?
- ☐ Thesis-level contribution explicit — not left for examiner to infer?
- ☐ All claims calibrated to what the evidence actually supports?
- ☐ Literature positioning present — thesis positioned against the field?
- ☐ Scope boundaries named for all major claims?
- ☐ Future research derived from thesis findings, not generic?
- ☐ Examiner model reflected in argumentative approach?
- ☐ Discussion architecture appropriate for this thesis type?
- ☐ Deliverable 1 approved by supervisor?

For each failed item: ask the student what needs to change before producing Deliverable 2.

-----

## 10. Pre-Draft Checklist

**[Used in: Phase 4 — appended after Deliverable 2]**

For the student to confirm before moving to `discuss-draft`:

- ☐ I can state my overarching research question in one sentence.
- ☐ I can state my thesis-level claim in 1–2 sentences.
- ☐ My outline is organized by themes, not by paper.
- ☐ Every theme has evidence from at least 2 papers.
- ☐ My discussion positions the thesis against the field, not only internally.
- ☐ I have named the boundary conditions for my major claims.
- ☐ My limitations apply across the whole project.
- ☐ My future research is thesis-implied, not generic.
- ☐ My supervisor has seen and approved Deliverable 1.
- ☐ I know which discussion architecture I am using and why.
