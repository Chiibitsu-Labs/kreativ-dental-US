# Kreativ Dental US Knowledge Base

Operational source of truth for David Lee's Kreativ Dental work in Texas, Ohio, and Indiana.

This repository is designed to power four things immediately:

1. reliable answers for David;
2. consistent lead qualification and handoff;
3. Bronwyn-style response drafting;
4. a future Kreativ Dental Mission Control without turning it into a medical-record system.

## Start here

- [Operating rules](knowledge/00-start-here.md)
- [David's quick answers](knowledge/david-quick-answers.md)
- [Roles and routing](knowledge/roles-and-routing.md)
- [Clinic and offer](knowledge/clinic-and-offer.md)
- [Patient journey](knowledge/patient-journey.md)
- [Lead intake](playbooks/lead-intake.md)
- [Response playbook](playbooks/bronwyn-response-playbook.md)
- [Handoff playbook](playbooks/handoff.md)
- [Pipeline and attribution](operations/pipeline-and-attribution.md)
- [Mission Control specification](operations/mission-control-spec.md)
- [Open decisions](operations/open-decisions.md)
- [David Copilot instructions](ai/david-copilot-instructions.md)
- [Operator instructions](ai/operator-instructions.md)
- [AI project setup](ai/project-setup.md)
- [Launch checklist](operations/launch-checklist.md)

## Official USA routing currently documented

- Patient records and clinical-review requests: `usa@kreativdentalclinic.eu`
- USA coordination phone: `+1 239 276 3162`
- USA Patient Relations Managers / National Agents: Craig and Bronwyn Jones

Patients should send X-rays and dental records directly to the USA inbox. David may remain copied with the patient's consent, but this repository and the planned Mission Control must not store X-rays, dental records, clinical photographs, medical histories, or treatment files.

## Evidence labels

Every operational statement should use one of these labels when its status matters:

- `CONFIRMED` - supported by a current authoritative source or directly confirmed by the responsible person.
- `WORKING_RULE` - safe operating choice adopted so work can proceed; not represented as clinic policy.
- `PENDING` - answer is needed from the responsible owner.
- `CONFLICT` - supplied sources disagree; do not publish or promise.
- `PROHIBITED` - action or claim must not be used.

## Source priority

When documents disagree, use this order:

1. signed contract or current written clinic instruction;
2. current official clinic material;
3. dated direct email from the responsible owner;
4. agent guide or training manual;
5. call notes or chat;
6. inference.

Newer direct instructions override older general guidance. For example, the July 12 email saying there is no individual regional advertising budget currently overrides the earlier general marketing guide.

## Repository safety

This is a sanitized knowledge base, not a patient database.

- Never commit patient names, contact details, IP addresses, travel itineraries, X-rays, dental records, clinical images, medical histories, or private email threads.
- Never commit David's private health, family, banking, payment, or home-address information.
- Use anonymized scenarios only.
- Keep raw source files outside this repository.
- Record a source name and date, not a copy of sensitive source content.

## Current build status

The operating model is usable now. Offer terms, out-of-state commission handling, external CRM fields, and post-handoff status synchronization remain pending confirmation and are isolated in [open decisions](operations/open-decisions.md) so they do not block the rest of the system.
