# Home Credit LAP Voice Agent — Implementation Notes

## 1. Project Overview

This project implements a voice agent for preliminary qualification of existing Home Credit customers for a Loan Against Property (LAP) offer of up to ₹75,00,000.

The agent was configured using Bolna AI and follows the business rules and system prompt documented in this repository.

## 2. Platform and Configuration

* Voice agent platform: Bolna AI
* Use case: Preliminary Loan Against Property qualification
* Maximum offer amount: ₹75 lakh
* Qualification checklist: Seven eligibility criteria
* Documentation: System prompt, business rules, and test plan are maintained in the `docs/` directory.

## 3. Key Implementation Decisions

* Confirm customer identity before disclosing offer details.
* Ask one qualification question at a time.
* Track answers provided out of order and avoid unnecessary repetition.
* Immediately disqualify agricultural property using the required exact message.
* Route existing property-loan and loan-transfer enquiries to the appropriate specialist.
* Enforce the stated requirements for original property documents, bank-received income, loan amount, and tenure.
* Treat the outcome as preliminary qualification, not final loan approval.
* Avoid inventing interest rates, fees, callbacks, or approval promises.

## 4. Repository Structure

* `README.md` — Project overview and repository information.
* `.gitignore` — Excludes specified sensitive and unnecessary files.
* `docs/system-prompt.md` — Configured system prompt.
* `docs/business-rules.md` — Eligibility and conversation rules.
* `docs/test-plan.md` — Test scenarios and recorded results.
* `docs/implementation-notes.md` — Implementation summary and submission links.

## 5. Validation

The agent should be tested for normal qualification, out-of-order answers, agricultural-property disqualification, missing original documents, cash-only income, requested amounts above ₹75 lakh, out-of-range tenure, existing property loans, and customer refusal.

Record test outcomes in `docs/test-plan.md` based on actual observed behavior.

## 6. Submission Links

* Published Bolna agent: [Add published agent URL]
* GitHub repository: [Add GitHub repository URL]
* Screen recording: [Add Google Drive recording URL]

Replace these placeholders with the actual links before submitting.

## 7. Limitations

* The agent performs preliminary qualification only.
* Final eligibility and loan approval remain subject to further review.
* No interest rate, fee, approval, or callback should be promised unless supported by the relevant system information.
* Test results should reflect actual execution rather than assumed success.
