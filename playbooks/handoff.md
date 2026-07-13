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

- To: `usa@kreativdentalclinic.eu`
- CC: David and the patient, with consent
- Subject: `David Lee referral - [Lead ID]`

Do not put a diagnosis, treatment details, or other sensitive information in the subject line.

## Handoff summary

Include only:

- lead ID;
- patient name and state;
- how the relationship began;
- the high-level situation in the patient's own terms;
- desired result;
- local plan or quote, if volunteered;
- rough travel timing;
- whether records are available;
- the specific next step requested;
- confirmation that David may remain copied.

Do not attach records yourself. Ask the patient to send them directly in the official email thread.

## After sending

1. Set stage to `HANDOFF_SENT`.
2. Record `handoff_at` and the USA inbox as recipient.
3. Record `source_agent = David Lee` regardless of patient state.
4. Set territory status to `IN_TERRITORY`, `OUT_OF_TERRITORY`, or `UNKNOWN`.
5. Request acknowledgement without slowing the patient's next step.
6. Follow up if there is no acknowledgement within two business days.
7. Do not chase the patient and the USA team simultaneously with conflicting messages.

## Relationship continuity

`WORKING_RULE`

David stays copied on non-clinical relationship and progress updates with patient consent. The patient may always request a direct/private conversation with the USA or clinic team. Respect that immediately.

## Status-update request

Use this compact request after handoff:

> For David's follow-up tracker, could you reply with the current stage when convenient: acknowledged, records requested, clinic review, consultation offered, booked, travelling, treatment started, completed, nurture, or closed? We only record the stage and next action, not clinical details.
