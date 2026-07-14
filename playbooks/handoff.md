# Handoff Playbook

## When to hand off

Hand off when any of the following is true:

- the prospect says they want to explore the option seriously;
- they want to send records;
- they ask for treatment-specific price, timing, or suitability;
- they want an appointment or travel coordination;
- David or Chii cannot answer without guessing;
- the lead is outside Texas, Ohio, or Indiana.

## Consent

Before introducing the prospect, ask:

> May I introduce you by email to the Kreativ Dental USA patient-relations team and remain copied so I can continue helping with the process?

Record the response and date. Do not forward a private conversation or contact information without permission.

## Official route

Craig and Bronwyn have confirmed that qualified leads go directly to them. They enter the patient into the Kreativ Dental CRM and coordinate next steps with Budapest.

- To: `usa@kreativdentalclinic.eu`
- CC: David and the patient, with consent
- Subject: `David Lee referral - [Lead ID]`

Do not put a diagnosis, treatment details, or other sensitive information in the subject line.

## Handoff summary

Include only:

- lead ID;
- full name;
- email address;
- telephone number;
- city and state of residence;
- how the relationship began;
- a brief explanation of the patient's dental concern or treatment need;
- desired result;
- local plan or quote, if volunteered;
- rough travel timing;
- whether records are available;
- the specific next step requested;
- confirmation that David may remain copied.

Any available X-rays, photographs, or existing treatment plans are useful to Craig and Bronwyn, but David's tools must not retain them. Ask the patient to send them directly in the official email thread.

## After sending

1. Set stage to `HANDOFF_SENT`.
2. Record `handoff_at` and the USA inbox as recipient.
3. Record `source_agent = David Lee` regardless of patient state.
4. Set territory status to `IN_TERRITORY`, `OUT_OF_TERRITORY`, or `UNKNOWN`.
5. Request acknowledgement and confirmation of clinic CRM entry without slowing the patient's next step.
6. Record the external CRM ID if supplied; do not copy clinical CRM content into Mission Control.
7. For an out-of-state patient, preserve David as the original source and mark commission mechanics pending the applicable sharing arrangement.
8. Follow up if there is no acknowledgement within two business days.
9. Do not chase the patient and the USA team simultaneously with conflicting messages.

## Relationship continuity

`CONFIRMED`

David should remain involved with patients he introduces. Craig and Bronwyn will manage clinic coordination and keep him informed of meaningful developments. He may remain copied on relevant communications when appropriate and when the patient is comfortable with this. The patient may always request a direct/private conversation; respect that immediately.

## Status-update request

Use this compact request after handoff:

> For David's follow-up tracker, could you reply with the current stage when convenient: acknowledged, CRM entered, records requested, clinic review, consultation offered, booked, travelling, treatment started, completed, nurture, or closed? We only record the stage and next action, not clinical details.
