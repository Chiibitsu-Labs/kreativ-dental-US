# Pipeline and Attribution

## Why attribution needs a mechanism

The supplied materials say David earns an agreed percentage when a patient he introduces proceeds with treatment. They do not explain how a lead is technically tagged, acknowledged, deduplicated, or handled across territories.

Without an attribution mechanism, a real David relationship could enter the USA team's CRM without durable evidence that David sourced it.

## Mission Control stages

| Stage | Meaning | Required next action |
|---|---|---|
| `NEW` | Inquiry captured but not reviewed | Review and assign |
| `CONTACTED` | First human response sent | Await response or follow up |
| `INTERESTED` | Prospect is open to exploring Budapest | Complete practical qualification |
| `QUALIFIED` | Relevant need, openness, and next step established | Obtain introduction consent |
| `HANDOFF_READY` | Summary and consent complete | Send official introduction |
| `HANDOFF_SENT` | Sent to USA inbox | Obtain acknowledgement |
| `ACKNOWLEDGED` | USA team confirms receipt | Await records or next step |
| `RECORDS_REQUESTED` | Patient invited to send records | Patient sends directly to USA inbox |
| `CLINIC_REVIEW` | USA/clinic team reviewing information | Await non-clinical status update |
| `CONSULTATION_OFFERED` | Appointment/consultation option presented | Patient decision |
| `BOOKED` | Appointment confirmed | Travel preparation |
| `TRAVELLING` | Travel is arranged or underway | Relationship support |
| `TREATMENT_STARTED` | Clinic confirms treatment began | Update attribution/commission status |
| `COMPLETED` | Treatment stage marked complete | Follow-up and outcome tracking |
| `NURTURE` | Interested but no current next step | Scheduled helpful follow-up |
| `CLOSED_LOST` | Not proceeding or unreachable | Record reason without sensitive detail |

These are internal operational stages, not claimed to match the clinic CRM.

## Attribution fields

Every lead record should contain:

- `lead_id` - generated, non-identifying reference;
- `source_agent` - David Lee when the relationship came through him;
- `source_channel` - referral, Facebook, website, event, community, etc.;
- `first_contact_at` - timestamp;
- `patient_state`;
- `territory_status` - in territory, out of territory, or unknown;
- `territory_owner` - David, another agent, national team, or pending;
- `handoff_at`;
- `handoff_recipient`;
- `attribution_acknowledged_at`;
- `external_crm_id` - when supplied by the USA team;
- `commission_status` - unknown, pending, eligible, paid, disputed, or not eligible;
- `commission_basis` - pending confirmation;
- `commission_amount` - optional and access-restricted.

## Out-of-state leads

`WORKING_RULE`

Do not reject, hide, or claim ownership of an out-of-state patient.

1. Help the person normally.
2. Record `source_agent = David Lee` if the relationship came through David.
3. Mark `territory_status = OUT_OF_TERRITORY`.
4. Hand the person to the USA team.
5. Ask the USA team to assign the correct territory owner.
6. Preserve David's source attribution separately from territorial ownership.
7. Do not promise David a commission or split until the contract/national-agent rule is confirmed.

Recommended commercial model for discussion:

- source credit belongs to the person who created the relationship;
- territory/service credit belongs to the assigned state agent;
- the clinic or national agents define any split before treatment begins.

This is a recommendation, not current policy.

## Duplicate leads

If the USA CRM already contains the person:

- do not create competing records;
- preserve the first known CRM record;
- attach David's relationship evidence and timestamp;
- ask Bronwyn/Craig to determine attribution under the contract;
- mark the Mission Control record `ATTRIBUTION_REVIEW` until resolved.

## Commission questions still pending

- Is the reported 10% calculated from quoted treatment, invoiced treatment, or collected clinic revenue?
- When is commission earned and when is it paid?
- How are refunds, changed plans, staged treatment, and return visits handled?
- What happens when source agent and territory owner differ?
- Does the separate finder/referral fee apply to David, only to non-agents, or both in specific cases?
