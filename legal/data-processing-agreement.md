# Data Processing Agreement — draft

> **DRAFT — not effective and not a statement that Sofrato is a processor for every activity.** Use only where the parties' actual roles require a controller–processor agreement. Prepared on 14 November 2026. Complete the annexes, assess the supplier chain, and validate operational commitments before agreement or publication as operative terms.

## 1. Parties and applicability

This draft is intended for the customer identified in Annex A ("Controller") and **SOFRATO SPÓŁKA Z OGRANICZONĄ ODPOWIEDZIALNOŚCIĄ**, ul. Św. Mikołaja 8/11, lok. 208, 50-125 Wrocław, Poland, KRS **0001169631**, NIP **8971953020**, REGON **541548549** ("Processor"), only for processing where those roles are established.

Contact: **[contact@sofrato.com](mailto:contact@sofrato.com)**.

If the supplier structure instead involves a processor and subprocessor, or an independent controller for an activity, adapt the agreement to those roles. This draft does not replace the customer's agreement with Atlassian.

**Effective date and incorporation into the customer agreement:** {{DPA_EFFECTIVE_DATE_AND_INCORPORATION}}

## 2. Instructions and purpose

The Processor will process the personal data described in Annex A only on the Controller's documented instructions, including concerning transfers, unless applicable law requires otherwise. Where legally permitted, the Processor will notify the Controller of such a legal requirement before processing.

The permitted purposes are supplying the agreed Lessons Learned Hub functionality and associated authorized support, security, and maintenance. The Processor will inform the Controller if it considers an instruction to infringe applicable data protection law. Additional instructions and their handling must be recorded through the agreed contact process.

The Controller is responsible for the lawfulness of its instructions, necessary notices and legal bases, data minimization, user authorization, and configuring Confluence permissions appropriately. Both parties acknowledge that lessons and project/watchlist content have the app's site-wide sharing model, independently of source-page read restrictions.

## 3. Confidentiality and security

The Processor will restrict access to authorized persons who need it for the agreed purposes and who are bound by appropriate confidentiality obligations. It will implement appropriate technical and organizational measures taking account of the risks, nature, scope, and context of processing.

The agreed measures and actual publisher access arrangements must be recorded in Annex B. The current use of Forge, Forge SQL, and server-side write checks is implementation evidence, not proof that every Article 32 requirement or all publisher processes have been satisfied.

## 4. Other processors

The Processor will engage other processors only under the agreed specific or general written authorization and will impose applicable equivalent data protection obligations. Where required by applicable law, it remains responsible for its other processors' performance of those obligations.

Annex C must identify the provider entities, functions, locations, and contractual roles. Atlassian's involvement must be assessed against the actual contracts rather than assumed to be a subprocessor merely because the app runs on Forge.

**Authorization, advance notice, objection period, and resolution procedure:** {{SUBPROCESSOR_AUTHORIZATION_NOTICE_AND_OBJECTIONS}}

## 5. Assistance and personal data breaches

Taking account of the nature of processing, the Processor will provide appropriate assistance with the Controller's obligations concerning data-subject requests, security, breach notifications, impact assessments, and prior consultations, as applicable and with the information available to it.

The Processor will notify the Controller without undue delay after becoming aware of a personal data breach affecting the processing under this agreement, provide available relevant details, and cooperate with response and remediation. Further information can follow in stages as it becomes available. Responsibilities for notifying authorities and affected people remain governed by applicable law; platform reporting obligations are separate.

**Private request, escalation, and breach coordination procedure:** {{REQUEST_AND_INCIDENT_PROCESS}}

Do not present a request-handling or erasure process as operational until the necessary procedures and capabilities have been validated.

## 6. Return, deletion, and duration

On termination of the processing services, at the Controller's choice the Processor will delete or return the relevant personal data and delete existing copies unless applicable law requires retention. The agreed implementation must include verified handling of platform storage, retained copies, and any lawful exceptions, as described in Annex A.

The app's current logical deletion and watchlist removal do not satisfy a promise of immediate permanent erasure. This draft must not be executed with an undefined or unworkable return/deletion mechanism.

## 7. Information and audits

The Processor will make available information necessary to demonstrate compliance with the applicable processor obligations and allow for and contribute to audits, including inspections, by the Controller or an authorized auditor. Practical arrangements must preserve confidentiality and other customers' security without preventing rights required by law.

**Audit contact, practical procedure, and any lawful cost arrangements:** {{AUDIT_ARRANGEMENTS}}

## 8. Transfers and agreement priority

Transfers to third countries must have a lawful basis and applicable safeguards. Complete Annex C with the actual destinations and mechanisms. This draft is not itself an EU Standard Contractual Clauses instrument and does not establish EU-only storage.

In a conflict on processing obligations, the finalized DPA will take priority over the customer agreement to the extent stated there and permitted by law. Other commercial terms remain governed by the underlying agreement, subject to applicable law.

## Annex A — Processing description

| Item | Description |
|---|---|
| Controller identity and privacy contact | {{CUSTOMER_IDENTITY_AND_PRIVACY_CONTACT}} |
| Subject matter | Operation and authorized support of Lessons Learned Hub on the customer's Confluence Cloud installation |
| Nature and purpose | Store, retrieve, display, search, match, update, attribute, and report project lessons and watchlist activity; apply permissions and diagnose failures |
| Duration | {{PROCESSING_DURATION_AND_RETENTION}} |
| Data subjects | Customer users and people whose personal data the customer lawfully includes in app content or authorized support correspondence |
| Personal data types | Atlassian account IDs, displayed names/avatar references, user-entered project/lesson/watchlist content, source-page references, activity metadata, and necessary diagnostic/support information within the agreed scope |
| Sensitive data | Not intended for special-category data; customer instructions and controls must prevent inappropriate submissions |
| Return and deletion procedure, timing, retained copies, exceptions | {{DATA_RETURN_AND_VERIFIED_ERASURE_PROCEDURE}} |
| Controller instructions/contact route | {{DOCUMENTED_INSTRUCTION_CHANNEL}} |

## Annex B — Technical and organizational measures

Observed application features: Forge-hosted runtime and Forge SQL storage; calls to Confluence as the current user; server-side checks for app writes; attribution and logical-removal fields. These features require operational and contractual verification before they become commitments.

{{VERIFIED_TECHNICAL_AND_ORGANIZATIONAL_MEASURES}}

Complete the measures for access authorization and review, confidentiality, platform configuration, encryption and key responsibilities, logging and retention, vulnerability management, incident response, data-subject requests, erasure, backups/recovery, staff practices, and periodic verification. State what Atlassian provides and what Sofrato controls; do not claim unverified certifications.

## Annex C — Providers, locations, and transfers

{{VERIFIED_PROVIDER_ENTITIES_ROLES_COUNTRIES_AND_TRANSFER_MECHANISMS}}

Include the assessed Atlassian/Forge relationship, support email hosting where relevant to this agreement, any additional providers, and the agreed authorization/notification process. Confirm whether customer residency controls apply to this specific app and data type.

## Basis for review

Review the finalized agreement against applicable law, including [Regulation (EU) 2016/679, particularly Article 28](https://eur-lex.europa.eu/eli/reg/2016/679/oj). A template cannot establish the parties' actual roles or implement compliance processes.

[Back to documentation](../README.md) · [Privacy Policy draft](privacy-policy.md) · [Terms of Use draft](terms-of-use.md)
