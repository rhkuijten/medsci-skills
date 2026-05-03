# Medical Presentation Templates

Section structure, slide counts, and design tone for the four medical presentation
contexts handled by this skill. Each template is a starting outline — not a rigid
template. Adapt to specific paper, audience, and time slot.

> **Sources**: RadioGraphics 2025 ("Winning at the Radiology Podium," DOI 10.1148/rg.250003);
> RSNA Refresher Course Committee guidelines; UAB Physician Scientist Development Office
> journal club framework; ASHP journal club template; medsci-skills internal patterns from
> 2026-04 grand rounds and journal club decks.
>
> **Triggered from**: SKILL.md Phase 0 (Outline) — pick the template matching the
> presentation context, then customize. Cross-reference `slide_design_principles.md` (§2
> reading-time budget table) and `critic_rubrics/slide.md` Section G.

---

## 1. Journal club (paper-driven, peer trainees)

**Audience**: residents / fellows + 1–2 faculty. Same-specialty cohort.
**Time**: 20–30 min total (10–15 min present + remainder discussion).
**Tone**: Methodologically rigorous, critical, peer-collegial.
**Slide count**: ~20–25 (1 slide / 30–60 s).

### Section structure

| # | Section | Slides | Purpose |
|---|---|---|---|
| 1 | Title + COI | 1 | Paper citation, presenter, date, disclosure |
| 2 | Why this paper | 1 | Clinical question that led to selection |
| 3 | Background | 1–2 | Existing evidence, what's known vs unknown |
| 4 | Research question (PICO) | 1 | Population / Intervention / Comparison / Outcome |
| 5 | Study design | 1–2 | Schema diagram of arms, randomization, follow-up |
| 6 | Methods | 1–2 | Cohort, eligibility, primary outcome, statistical plan |
| 7 | Results | 3–5 | Primary outcome figure, key tables, subgroup if relevant |
| 8 | Strengths / Weaknesses | 1 | 2-column slide (per `critic_rubrics/slide.md` G.30) |
| 9 | Limitations | 1 | Author-acknowledged + presenter-identified |
| 10 | Statistical vs clinical significance | 1 | Effect size + NNT / absolute risk reduction |
| 11 | Clinical implications | 1 | How this changes (or doesn't change) practice |
| 12 | Take-home messages | 1 | 3 bullet points, no more |
| 13 | References / Q&A | 1 | Inline citations + key supporting refs |

### Design seed
- **Color**: Institutional accent (1) + neutral grays (2). No 3-D, no decorative animation.
- **Typography**: Sans-serif (Helvetica / Calibri / Pretendard for KR). 28 pt title /
  18–20 pt body.
- **Figures**: Use figures from the paper directly (cite slide-corner). Do not re-render
  unless adding emphasis annotations.
- **Speaker note density**: 5–10 s of spoken content per slide.

### Pre-presentation checklist
- [ ] Faculty review of paper selection (per UAB framework — verify educational
      significance, relevance for practice, validity).
- [ ] Read paper independently before reading the abstract (avoid author-framing bias).
- [ ] Allocate ~50% of total time to discussion, not lecture.
- [ ] Verify `submission_safe: true` is not needed (journal club ≠ submission).

---

## 2. Grand rounds (mixed specialty / mixed seniority)

**Audience**: Multi-specialty, mixed trainee + attending. May include non-radiologists for
imaging-themed rounds.
**Time**: 45–60 min total (35–45 min present + remainder Q&A).
**Tone**: Educational, broadly accessible, single-take-home framing.
**Slide count**: ~30–45 (1 slide / 60–90 s, with worked examples).

### Section structure

| # | Section | Slides | Purpose |
|---|---|---|---|
| 1 | Title + COI + Acknowledgments | 1–2 | Title, presenter affiliation, disclosure, mentor credit |
| 2 | Learning objectives | 1 | 3–4 specific objectives (verb + noun pattern) |
| 3 | Hook / clinical case | 1–2 | A real (de-identified) case that motivates the topic |
| 4 | Why this matters now | 1 | Burden / incidence / unmet clinical need |
| 5 | Background (concept review) | 2–3 | Pathophysiology / imaging principles, accessible level |
| 6 | Current standard of care | 1–2 | Where the field is today, what the gap is |
| 7 | Recent evidence | 5–8 | 2–3 key papers; one slide per take-home |
| 8 | Worked imaging examples | 4–8 | Side-by-side cases illustrating each teaching point |
| 9 | Practice algorithm / decision tree | 1–2 | Synthesis: how to apply in daily practice |
| 10 | Limitations of current evidence | 1 | Honest framing of what we still don't know |
| 11 | Future directions | 1 | Trials in progress, AI/computational angles if relevant |
| 12 | Take-home messages | 1 | Map back to learning objectives |
| 13 | Return to opening case | 1 | Show how the talk's content alters the case management |
| 14 | Q&A / References | 1 | Inline cites throughout; reference handout if requested |

### Design seed
- **Color**: Institutional palette + 1 accent for highlights. Avoid >3 colors per slide.
- **Typography**: Title 32 pt / body 20–22 pt (room may seat ≥ 100).
- **Figures**: Mix of paper figures, original imaging, and SMART Servier anatomical icons.
  AI-image disclosure if anything is AI-generated.
- **Worked examples**: Build-up animations acceptable (sequential reveal of imaging
  findings) — but only when the build encodes a teaching step.

### Pre-presentation checklist
- [ ] Learning objectives written with measurable verbs (avoid "understand"; prefer
      "identify," "differentiate," "recommend").
- [ ] Imaging consent / de-identification verified for all cases.
- [ ] Disclosure slide includes industry relationships, advisory roles, prior publications
      cited.
- [ ] Mentor pre-review completed (typical 1–2 weeks before).

---

## 3. Conference talk (RSNA / ECR / KCR / society meeting)

**Audience**: Specialist peers; high domain expertise.
**Time**: 7–12 min present + 2–3 min Q&A (oral session standard).
**Tone**: Tight, data-dense, focused on contribution.
**Slide count**: ~10–14 for 10-min talk; ~14–18 for 12-min (1 slide / 45–60 s).

### Section structure

| # | Section | Slides | Purpose |
|---|---|---|---|
| 1 | Title + Disclosure | 1 | Title, authors, affiliation, COI in 1 slide |
| 2 | Background + Gap | 1–2 | Tight: 1 sentence on context, 1 on gap |
| 3 | Hypothesis / Aim | 1 | Stated as a sentence-headline |
| 4 | Methods | 1–2 | Cohort flow diagram + key methodological choice |
| 5 | Primary results | 2–3 | One figure per result; sentence-headline title |
| 6 | Subgroup / sensitivity | 1 | Only if it's the most defensible secondary finding |
| 7 | Limitations | 1 | Brief — acknowledge top 2–3 |
| 8 | Conclusions | 1 | 1 sentence; mirrors abstract conclusion |
| 9 | Acknowledgments | 1 | Funding, collaborators, departmental support |

### Design seed
- **Color**: One accent for primary result; everything else neutral.
- **Typography**: ≥ 24 pt body throughout (auditorium projection).
- **Figures**: Re-render journal figures for slide context (drop methodological detail,
  enlarge axis labels, direct-label series). RSNA / ECR projection rooms project at 1080p
  — vector PDFs preferred.
- **Speaker pace**: 130–150 words/min for academic delivery; rehearse to ensure last
  slide arrives at 9:30 of a 10-min slot.

### Pre-presentation checklist
- [ ] Abstract was accepted for oral (not poster) — confirm slot type and time.
- [ ] Audience response system not used (oral sessions don't typically include ARS).
- [ ] Submitted disclosure to society (society disclosures often separate from manuscript
      COI).
- [ ] Backup slide stack for top-3 anticipated questions ready.

---

## 4. Lecture / didactic (residents, course material)

**Audience**: Trainees in structured curriculum (radiology residents, fellows, medical
students).
**Time**: 50–60 min (full lecture slot).
**Tone**: Pedagogical, build-up, recap-friendly.
**Slide count**: ~30–40 (1 slide / 90–120 s, with worked examples and recap slides).

### Section structure

| # | Section | Slides | Purpose |
|---|---|---|---|
| 1 | Title + Lecture position in curriculum | 1 | "Lecture 4 of 12: Body MRI series" |
| 2 | Learning objectives | 1 | Mapped to curriculum competencies |
| 3 | Recap of prior lecture | 1–2 | Where we were last time |
| 4 | Today's roadmap | 1 | 3–5 sections previewed |
| 5 | Section 1: Concept | 3–5 | Build-up + worked example + check-for-understanding |
| 6 | Section 2: Concept | 3–5 | Same pattern |
| 7 | ... | | |
| 8 | Synthesis / decision algorithm | 2–3 | How sections connect into clinical workflow |
| 9 | Self-assessment questions | 2–3 | 3–5 multiple-choice with answer reveal |
| 10 | Take-home messages | 1 | Map back to learning objectives |
| 11 | Pre-reading for next lecture | 1 | Specific paper / textbook chapter |
| 12 | References + further reading | 1 | Curated list, not exhaustive |

### Design seed
- **Color**: Course palette consistent across all lectures in series.
- **Typography**: Title 28 pt / body 20 pt. Build-up animations acceptable for stepwise
  concept introduction.
- **Figures**: Mix of textbook diagrams, original imaging, SMART Servier icons. Reusable
  asset library across lecture series (per `pptx-mac-compatibility` rule — single asset
  source).
- **Recap pattern**: At each section end, a 1-slide recap before moving on. Helps
  trainees with weaker prior knowledge.
- **Self-assessment**: Use audience-response polling if classroom supports it; otherwise
  show MCQ → pause → reveal answer + explanation slide.

### Pre-presentation checklist
- [ ] Lecture position in curriculum confirmed (not duplicating prior lecture content).
- [ ] Self-assessment questions mapped to learning objectives.
- [ ] Pre-reading assignment matches the lecture's prerequisites.
- [ ] Course-level branding consistent (logo, color, font).

---

## Mapping to SKILL.md phases

| Template element | SKILL.md phase | Notes |
|---|---|---|
| Audience definition | Phase 0 | Required input — controls template choice |
| Time slot | Phase 0 | Determines slide count target |
| Section structure | Phase 0 → outline | Use template as starting outline; customize |
| Speaker script density | Phase 2 | 130–150 wpm for academic talks |
| Slide design tokens | Phase 3 | See `slide_design_principles.md` §4 |
| Q&A backup slides | Phase 4 | Per template's anticipated-question profile |
| Pre-presentation checklist | Phase 4 | Run before final delivery |

## Cross-references
- `slide_design_principles.md` — design foundations (Reynolds, Duarte, Knaflic, Tufte)
- `critic_rubrics/slide.md` — per-slide quality scoring
- `workflow-checklist.md` — end-to-end Phase 0 → 4 production checklist
- `~/.claude/rules/pptx-mac-compatibility.md` — TIFF / sp3d / app.xml / srcRect defects
- `~/.claude/rules/journal-ai-image-policies.md` — AI-image policy (visual abstract /
  Central Illustration cases)
