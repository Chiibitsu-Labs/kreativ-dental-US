# AI Project Setup

## Project A - David Copilot

Purpose: give David a simple place to ask questions, prepare for calls, draft replies, and create handoffs.

### Add these files

- `README.md`
- everything under `knowledge/`
- `playbooks/lead-intake.md`
- `playbooks/bronwyn-response-playbook.md`
- `playbooks/handoff.md`
- `operations/pipeline-and-attribution.md`
- `operations/open-decisions.md`
- `operations/claims-register.md`
- `templates/`
- `ai/david-copilot-instructions.md`
- `ai/test-cases.md`

Use the complete contents of `ai/david-copilot-instructions.md` as the project's custom instructions.

### Give David these starter prompts

- `/answer Where should this person send their X-rays?`
- `/prep Prospect has a large quote and is afraid of travelling.`
- `/reply [paste a sanitized message or summary]`
- `/handoff [paste the operational lead summary]`

Do not paste raw patient records or clinical images into the project.

## Project B - Kreativ Operator

Purpose: let Chii process leads, create responses, manage content, maintain the KB, and produce ROI reports.

### Add these files

- the complete sanitized repository;
- `ai/operator-instructions.md` as custom instructions.

### Main commands

- `/lead`
- `/reply`
- `/handoff`
- `/content`
- `/radar`
- `/weekly`

## Acceptance test

Run every scenario in `ai/test-cases.md`. The project is ready only when it:

- routes records to the official USA inbox;
- refuses diagnosis and clinical interpretation;
- preserves David's source attribution;
- handles out-of-state leads without claiming territory;
- refuses to publish the conflicting offer;
- cites the correct KB section;
- produces concise, usable answers.

## Updating the projects

GitHub is the canonical source. When a KB file changes:

1. update and review it in GitHub;
2. record the evidence status and source;
3. replace the corresponding project file;
4. rerun affected acceptance tests;
5. note the update date in the weekly scorecard.
