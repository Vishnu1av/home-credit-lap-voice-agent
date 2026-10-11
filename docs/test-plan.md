# Home Credit LAP Voice Agent — Test Plan

## 1. Purpose

This document records test scenarios for the Home Credit Loan Against Property (LAP) qualification voice agent built using Bolna AI.

The tests check conversation handling, the seven eligibility criteria, special disqualification rules, and the final preliminary qualification outcome.

## 2. Test Results

Record the actual result after running each test. Mark a test as **PASS** only when the observed agent behavior matches the expected behavior.

| Test ID | Scenario                                                           | Expected Result                                                                                                              | Actual Result |
| ------- | ------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------- | ------------- |
| T01     | Customer confirms identity and has time to talk                    | Agent explains the offer and begins the checklist                                                                            | Not recorded  |
| T02     | Customer is busy                                                   | Agent asks for a preferred callback time, thanks them, and ends the call without claiming a callback is scheduled            | Not recorded  |
| T03     | Customer states the property is agricultural                       | Agent says the exact required agricultural-property disqualification message and ends immediately                            | Not recorded  |
| T04     | Customer has residential, commercial, or industrial property       | Agent records the property type and continues the checklist                                                                  | Not recorded  |
| T05     | Customer does not have original property documents                 | Agent explains that the customer does not meet this offer's criteria and ends the call                                       | Not recorded  |
| T06     | Customer requests more than ₹75 lakh                               | Agent explains the ₹75 lakh limit and asks whether the customer will consider that amount                                    | Not recorded  |
| T07     | Customer receives income only in cash                              | Agent explains that cash-based income does not meet the offer criteria and ends the call                                     | Not recorded  |
| T08     | Customer requests a tenure outside 3–15 years                      | Agent explains the permitted range and asks whether the customer will choose a tenure within it                              | Not recorded  |
| T09     | Customer provides checklist answers out of order                   | Agent remembers clear answers and does not repeat questions unnecessarily                                                    | Not recorded  |
| T10     | Customer mentions an existing property loan or loan transfer       | Agent routes the enquiry to the appropriate specialist and ends the current qualification flow                               | Not recorded  |
| T11     | Customer meets all stated criteria and answers all seven questions | Agent summarizes the answers and explains that the case may proceed to senior loan expert review, without promising approval | Not recorded  |
| T12     | Customer declines to continue                                      | Agent respects the decision, thanks the customer, and ends politely                                                          | Not recorded  |

## 3. Execution Notes

For each test, record:

* Date tested
* Test ID
* Observed agent response
* Result: PASS, FAIL, or NOT RUN
* Notes or corrective action, if needed

## 4. Important Validation Checks

* The agricultural-property disqualification message must match the required wording exactly.
* The agent must not disclose offer details before confirming customer identity.
* The agent must track answers provided out of order.
* The agent must not treat unanswered checklist items as eligible answers.
* The agent must not invent interest rates, fees, approval decisions, or confirmed callbacks.
* Preliminary qualification must not be presented as final loan approval.

## 5. Overall Status

Overall test status: Pending verification.

Update this status after executing the scenarios and recording the actual results.
