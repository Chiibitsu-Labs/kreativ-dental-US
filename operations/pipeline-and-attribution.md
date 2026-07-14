# Pipeline and Attribution

## Confirmed qualified-lead route

`CONFIRMED` by Bronwyn and Craig's July 14, 2026 written clarification.

1. Obtain the patient's consent to introduce them and share the minimum contact information.
2. Send the qualified lead to Craig and Bronwyn through the official USA channel.
3. Craig and Bronwyn enter the patient into the Kreativ Dental CRM.
4. They coordinate the next steps with the Budapest clinic.
5. David remains involved and is informed of meaningful developments when appropriate and when the patient is comfortable with this.

Mission Control is David's relationship, follow-up, attribution, and ROI layer. It does not replace or duplicate the clinic's medical CRM.

## Minimum handoff information

- full name;
- email address;
- telephone number;
- city and state of residence;
- brief explanation of the patient's dental concern or treatment need;
- whether X-rays, photographs, or an existing treatment plan are available.

The patient should send clinical files directly to Craig and Bronwyn through the official USA email thread. Mission Control records only whether records are available/sent and the relevant dates.

## Mission Control stages

| Stage | Meaning | Required next action |
|---|---|---|
| `NEW` | Inquiry captured but not reviewed | Review and assign |
| `CONTACTED` | First human response sent | Await response or follow up |
| `INTERESTED` | Prospect is open to exploring Budapest | Complete practical qualification |
| `QUALIFIED` | Relevant need, openness, and next step established | Obtain introduction consent |
| `HANDOFF_READY` | Required summary and consent complete | Send official introduction |
| `HANDOFF_SENT` | Sent to Craig/Bronwyn | Obtain acknowledgement |
| `ACKNOWLEDGED` | USA team confirms receipt | Await CRM entry or next step |
| `CRM_ENTERED` | Craig/Bronwyn confirms clinic CRM entry | Record external ID if available |
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
- `handoff_recipient` - Craig/Bronwyn / official USA inbox;
- `attribution_acknowledged_at`;
- `external_crm_id` - when supplied by the USA team;
- `commission_status` - unknown, pending, eligible, paid, disputed, or not eligible;
- `commission_rate`;
- `commission_basis` - pending confirmation;
- `commission_amount` - optional and access-restricted.

## Out-of-state leads

`CONFIRMED WITH OPEN MECHANICS`

- David receives credit for patients he personally generates even outside his assigned territory.
- The original source must be clearly recorded.
- Where another established agent represents the patient's state, the existing out-of-territory arrangement may include commission sharing.
- Bronwyn's July 13 clarification stated that David receives 5% from out-of-state dental patients.
- The July 14 clarification confirms source credit and sharing where applicable but does not restate the percentage or define its calculation.

Operationally:

1. Help the person normally.
2. Record `source_agent = David Lee` when David created the relationship.
3. Mark `territory_status = OUT_OF_TERRITORY`.
4. Send the qualified lead to Craig and Bronwyn for clinic CRM entry and routing.
5. Record 5% as the latest specific written out-of-state rate.
6. Leave calculation basis, applicability, split, eligibility, payment timing, refund handling, and dispute status pending until documented.

Source attribution and territory ownership are separate concepts.

## Duplicate leads

If the clinic CRM already contains the person:

- do not create competing Mission Control records;
- preserve the earliest known source evidence and timestamp;
- ask Craig/Bronwyn to apply the clinic duplicate/attribution rule;
- mark the Mission Control record `ATTRIBUTION_REVIEW` until resolved.

## Commission questions still pending

- Is David's in-state rate the reported 10%, and where is it documented?
- When exactly does the 5% out-of-state rate apply versus another split?
- Is commission calculated from quoted, invoiced, completed, or collected treatment?
- When is commission earned and when is it paid?
- How are refunds, changed plans, staged treatment, and return visits handled?
- How are pre-existing CRM leads and duplicate referrals credited?
