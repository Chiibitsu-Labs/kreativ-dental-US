# Kreativ Dental Mission Control - MVP Specification

## Decision

Yes, David should have his own platform. It should be an operational layer around the clinic process, not a replacement for the clinic's medical CRM.

## Product promise

> David can see who needs attention, what to say, what happens next, and whether his relationships are progressing—without handling clinical records or guessing.

## Primary users

- **David:** answer questions, see priority leads, prepare for conversations, and check relationship status.
- **Chii:** operate leads, draft responses, manage content, update the KB, and report ROI.
- **Craig/Bronwyn / USA team (optional lightweight access):** enter qualified leads into the clinic CRM, acknowledge handoffs, and update a non-clinical stage.

## MVP modules

### 1. Today

- leads needing a reply;
- follow-ups due;
- handoffs awaiting acknowledgement;
- blockers and pending decisions;
- one-click `Ask the KB`.

### 2. Lead inbox

- minimal intake record;
- source and state;
- qualification summary;
- consent status;
- priority and next action;
- response-draft button.

### 3. Pipeline

Kanban or compact list using the stages in [pipeline and attribution](pipeline-and-attribution.md).

### 4. Handoff

- generate lead ID;
- produce the official handoff email;
- preserve David as source agent;
- route the qualified lead to Craig and Bronwyn for clinic CRM entry;
- send patient records to the official USA email, not Mission Control;
- track acknowledgement, CRM-entry confirmation, and external CRM ID.

### 5. Ask the KB

- answer with evidence status;
- show what David may say;
- show what must be escalated;
- cite the KB page and section;
- refuse to infer medical conclusions.

### 6. Content

- 4+1 weekly calendar;
- state variants for Texas, Ohio, and Indiana;
- approval status;
- claim/offer check;
- published link and inquiry attribution.

### 7. ROI

- conversations;
- qualified leads;
- handoffs;
- handoff-to-booking progression;
- booked consultations;
- treatment starts when reported;
- content published and inquiries generated;
- response time;
- estimated hours saved;
- commission pipeline where contractually supportable.

## Data boundary

### Store

- identity and contact details needed to continue the relationship;
- state, source, consent, stage, ownership, next action, dates;
- high-level need category and prospect-provided goal;
- records-available/sent flag;
- official CRM reference and attribution status;
- non-clinical notes.

### Never store in the MVP

- X-rays, scans, clinical photographs, dental records, or treatment attachments;
- detailed medical history, medications, diagnoses, or clinical opinions;
- passport, payment-card, banking, or insurance files;
- raw email/chat archives;
- AI-generated medical conclusions.

If a later version accepts medical records, it becomes a materially different product requiring explicit privacy, security, retention, access, vendor, and legal review.

## Status synchronization

Craig and Bronwyn have confirmed that they enter qualified patients into the clinic CRM and will keep David informed of meaningful developments. Mission Control therefore tracks David's relationship and follow-up layer rather than attempting to replace the clinic CRM.

Use the simplest path first:

1. **Now:** handoff email includes the lead ID, routes the qualified patient to Craig and Bronwyn, and asks for acknowledgement when clinic CRM entry is complete.
2. **Next:** agree which meaningful non-clinical stages they will share and whether updates arrive by email or a private one-click form.
3. **Later:** integrate with the clinic CRM through an approved API, webhook, limited view, or scheduled export if available.

The system remains useful even without integration because it owns David's relationship workflow and follow-up commitments.

## Access model

- Chii: administrator;
- David: full access to his leads and KB, restricted settings;
- USA status updater: only assigned handoffs and non-clinical status fields;
- no public lead pages;
- activity log for status and attribution changes;
- least-privilege access by default.

## MVP success criteria

- David can answer a routine question without guessing.
- Chii can turn an inquiry into a reviewed response and next action in minutes.
- Every handoff has a lead ID, consent, and source attribution.
- No medical attachment enters the platform.
- David can see which relationships require attention.
- A weekly ROI summary can be produced without reconstructing events from chats.

## Not in the first release

- clinical-record upload;
- treatment-plan generation;
- payment processing;
- automated medical triage;
- scraping private groups;
- unsolicited bulk messaging;
- replacing the clinic CRM.
