# Home Credit LAP Voice Agent

## Project Overview

This project documents a voice agent designed for the Home Credit Loan Against Property (LAP) qualification use case. The agent is configured using Bolna AI.

The voice agent contacts existing customers, explains the LAP offer of up to ₹75,00,000, collects preliminary eligibility information, and guides eligible customers toward a senior loan expert.

## Project Objectives

* Explain the Loan Against Property offer to customers.
* Verify customer identity before proceeding.
* Collect the information required for preliminary eligibility screening.
* Identify ineligible cases according to the configured business rules.
* Handle customer questions and answers provided out of order.
* Route existing property loan or loan-transfer requests according to the configured flow.
* Direct preliminarily qualified customers toward a senior loan expert.

## Key Qualification Criteria

The agent checks the following seven criteria:

1. **Property type:** Residential house/flat, commercial shop/office, or industrial factory. Agricultural property is ineligible under this offer.
2. **Ownership:** Sole or joint ownership.
3. **Original property documents:** Original documents must be available.
4. **Loan amount:** The maximum offer amount is ₹75,00,000, subject to eligibility and further review.
5. **Occupation and income:** Salaried or self-employed customers must receive income through a bank; cash-only income is ineligible.
6. **Property market value:** The customer's estimated current property value is collected.
7. **Loan tenure:** The requested tenure must be between 3 and 15 years, inclusive.

## Conversation Handling

The voice agent is designed to:

* Greet customers and verify their identity.
* Ask for a suitable callback time when a customer is busy.
* Remember answers already provided.
* Avoid repeating questions that have already been answered.
* Return to unanswered qualification questions before making a preliminary qualification decision.
* Explain ineligibility politely.
* Avoid promising final loan approval or inventing interest rates.
* Direct customers toward a senior loan expert when the configured qualification flow is completed.

## Technology

* **Voice agent platform:** Bolna AI
* **Interaction type:** AI-powered voice conversation
* **Use case:** Preliminary Loan Against Property qualification

## Repository Structure

```text
home-credit-lap-voice-agent/
├── README.md
├── .gitignore
└── docs/
    ├── system-prompt.md
    ├── business-rules.md
    ├── test-plan.md
    └── implementation-notes.md
```

## Testing

The test plan covers agricultural property, original document availability, loan amount limits, cash-only income, successful qualification, existing property loan requests, busy customers, and out-of-order answers.

Actual test results should be recorded after running each scenario in Bolna AI. Recordings and transcripts should only be described as actual evidence when they have genuinely been captured.

## Limitations

This repository documents the voice agent configuration and qualification rules. It does not independently deploy the voice agent, guarantee a callback, determine final loan approval, or guarantee loan terms.

## Submission

* **Published agent:** Bolna AI share link.
* **GitHub repository:** This repository.
* **Screen recording:** Google Drive link to the actual project demonstration, once recorded and uploaded.

## Privacy and Security

Do not commit passwords, API keys, private customer information, or confidential call recordings. Use test data when demonstrating the agent.
