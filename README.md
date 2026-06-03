# Prototype

Single-file clickable mockup of Stan's v1 patient intake. Open `index.html` in any browser. No build, no dependencies, no server required.

## What it covers

The prototype walks the four surfaces a patient hits in the first session:

1. **Safety screen** — the seven red-flag questions that gate every intake. Toggle any item to see the emergency-referral branch.
2. **Framework selection** — the screen where intake routes to one of six clinical advisors (McKenzie, Sarno, Sahrmann, McGill, Manual Therapy, or the Optimal multi-framework synthesis).
3. **Classification** — sample of the McKenzie centralization route by default. Pick "McGill / Biomechanics" instead to see the chair-test screen and a discogenic-pattern routing.
4. **Plan handoff** — what the patient sees after classification: education, self-treatment guidance, and the bridge to the Specialist Finder.

## What it is not

- Not the production design. Visual polish is intentionally low so reviewers focus on flow and content, not chrome.
- Not a complete walkthrough. Several sub-flows (PROM cadence, concierge scheduling, clinician dashboard) are documented in the spec bundle but not yet prototyped.
- Not connected to data. Every input is local state. Refresh resets it.

## Why this lives at `/prototype/index.html`

The original copy is still at `00_meeting/prototype/Stan_v1_Prototype_Intake.html` because the Engineer Brief PDF references that path. This top-level location exists so engineers (and their coding agents) can find it without reading the README first.

If you change one, update the other. Or pick one canonical location and delete the duplicate before this drifts.

## Related specs

- Product behavior: [`../02_spec/Stan_v1_Product_Spec.docx`](../02_spec/Stan_v1_Product_Spec.docx)
- Intake logic the prototype demonstrates: [`../03_clinical/decision_flow/LBP_Intake_Triage_Router.md`](../03_clinical/decision_flow/LBP_Intake_Triage_Router.md)
- Acceptance criteria for these screens: [`../02_spec/Stan_v1_Acceptance_Criteria.xlsx`](../02_spec/Stan_v1_Acceptance_Criteria.xlsx)
