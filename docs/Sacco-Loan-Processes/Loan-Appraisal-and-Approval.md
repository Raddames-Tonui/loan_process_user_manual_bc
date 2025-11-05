---
sidebar_position: 2
---

# Sacco Loan Appraisal and Approval in Microsoft Dynamics 365 Business Central

*Applies to:* Microsoft Dynamics 365 Business Central

*Audience:* Loan Officers, Credit/Appraisal Analysts, Branch Managers/Approvers, System Admins
Version: 2025-11-05

## Overview

This guide is a complete user reference for Sacco loan Appraisal and Approval processes in Business Central. It follows Microsoft Learn style, detailing prerequisites, step-by-step procedures, fields, controls, troubleshooting, and FAQs. Use Tell Me (Alt+Q) to find pages.

## Process Flow

1. Initiated Application Intake
2. Appraisal (data capture, eligibility)
3. Generate Payment Schedule
4. Appraisal Report
5. Send for Approval
6. Approver Decision
7. Ready for Disbursement

## Step 1 — Start the Appraisal from the Loan Application

- On the Loan Application card, click the Appraisal action to expose the appraisal tools.
- Visual: ![Appraisal action button](../../static/img/loan-appraisal-approval/appraisal%20button.png)
- Outcome: I can now access Eligibility Breakdown, Generate Payment Schedule, and Generate Appraisal Report.

## Step 2 — Capture the appraisal details (financials, collateral, guarantors)

- Enter member income, other recurring income, existing loan obligations, deductions/expenses, and then capture collateral and guarantors as needed.
- Use our standard appraisal form to double‑check inputs and attach it to the application.
- Visuals for the card/views I worked on:
  - Appraisal form: [Loan Appraisal form.pdf](../../static/img/loan-appraisal-approval/Loan%20Appraisal%20form.pdf)
  - Context screens I reviewed/edited:
    - ![Application view](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20151539.png)
    - ![Application view](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20152838.png)
    - ![Application view](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20153033.png)
    - ![Application view](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20153442.png)
    - ![Application view](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20153635.png)

## Step 3 — Run the Eligibility Breakdown and read the KPIs

- Choose Appraisal > Eligibility Breakdown to calculate eligibility based on the captured financials and product rules.
- Compare what you see on screen to the PDF to validate figures (share multiple cap, DTI, recommended amount/term, and any exception flags).
- Visuals:
  - On-screen breakdown: ![Eligibility Breakdown page](../../static/img/loan-appraisal-approval/Loan%20Appraisal%20Breakdown.png)
  - Detailed reference: [loan eligibility breakdown.pdf](../../static/img/loan-appraisal-approval/loan%20eligibility%20breakdown.pdf)
- What to check before moving on:
  - Requested vs. share‑multiple cap
  - DTI against product threshold (note any exception)
  - Recommended amount/term and conditions I must enforce

## Step 4 — Generate a Payment Schedule to validate affordability

- Click Appraisal > Generate Payment Schedule and confirm Principal, Rate, Term, Frequency, Grace (if any), and First Installment Date.
- Make sure installments, dates, and totals look right for the method (reducing/flat) before I commit.
- Visual: ![Generate Payment Schedule dialog](../../static/img/loan-appraisal-approval/Generate%20Payment%20Schedule.png)

## Step 5 — Generate and attach the Appraisal Report

- Use Appraisal > Generate Appraisal Report to compile the formal memo for approval.
- Verify it includes member profile, incomes/obligations, collateral/guarantors, eligibility KPIs, schedule summary, and any conditions; then I attach the PDF to the application.
- Visuals:
  - Action: ![Generate Appraisal Report action](../../static/img/loan-appraisal-approval/generate%20appraisal%20report.png)
  - Preview: ![Preview of Appraisal Report](../../static/img/loan-appraisal-approval/preview%20Appraisal%20Report.png)

## Step 6 — Send the appraised loan for approval

- From the application, click Send for Approval and add a short message: recommended amount/term, any exceptions, and key conditions (e.g., extra guarantor, share top‑up).
- Visual: ![Send for Approval action](../../static/img/loan-appraisal-approval/send%20loan%20for%20approval.png)
- Result: Approval Entries are created and the document locks while it’s pending.

## Step 7 — How the approver acts on the request

- The approver opens Approvals > Requests to Approve, opens the loan, and reviews my Header, Appraisal/Financials, Collateral/Guarantors, Schedule, Attachments, and the Appraisal Report.
- Visual: ![Approval actions available to approver](../../static/img/loan-appraisal-approval/Approval%20actions.png)
- Actions they can take (as shown): Approve, Reject (with a comment), Delegate, or Request Changes. I always read their comments for the audit trail and re‑submit if asked.

## What each screenshot proves in my flow

- appraisal button.png — Where I access the Appraisal menu on the application card.
- Loan Appraisal Breakdown.png — The live eligibility KPIs I reviewed (share multiple, DTI, recommended amount/term).
- loan eligibility breakdown.pdf — The detailed numbers I relied on for the memo.
- Generate Payment Schedule.png — The exact parameter dialog I used to validate affordability.
- generate appraisal report.png & preview Appraisal Report.png — The report action and the preview I checked before attaching.
- send loan for approval.png — The action I used to trigger the workflow.
- Approval actions.png — The approver’s decision buttons I expect them to use.
- Screenshot 2025-10-31 *.png — The application pages/tabs I edited and double‑checked during appraisal.

## The data I make sure to capture before approval

- Member & Product: Member No./Name; Product Code/Name
- Amount & Tenor: Requested vs. Recommended Amount; Requested vs. Recommended Term
- Income & Obligations: Gross/Net monthly income; other recurring income; existing installments; deductions/expenses
- Eligibility KPIs: Share‑multiple cap; DTI; net pay/allowable deduction; exceptions and rationale
- Collateral/Guarantors: Values and coverage %; guarantor exposure/limits
- Schedule summary: Frequency; first installment date; total interest/repayment
- Attachments: Appraisal Report PDF; appraisal form; eligibility breakdown PDF; KYC evidence

## How I keep control and a clean audit trail

- I rely on maker‑checker via approvals so my document locks while pending.
- I put concise, decision‑ready comments in the approval message and attach the PDFs.
- I keep all adjustments (like conditions or exceptions) written in both the report and approval comments.

## If I hit a snag (what I do)

- Appraisal actions not visible → I confirm I’m on a Loan Application card, have permission, and the product is Released.
- Eligibility Breakdown empty → I re‑enter missing income/obligations/product data and run it again.
- Can’t generate schedule → I fill principal, rate, term, frequency, and first installment date; then retry.
- Appraisal Report won’t open → I check that the report is published and allow pop‑ups.
- Can’t send for approval → I confirm Approver User Setup, workflow activation, and approver limits.
- Approver can’t act → I check Approval Entries for delegation or substitutes and nudge the current assignee.

## Appendix — The exact images and documents I used

- ![Appraisal button](../../static/img/loan-appraisal-approval/appraisal%20button.png)
- ![Generate Appraisal Report](../../static/img/loan-appraisal-approval/generate%20appraisal%20report.png)
- ![Preview Appraisal Report](../../static/img/loan-appraisal-approval/preview%20Appraisal%20Report.png)
- ![Loan Appraisal Breakdown](../../static/img/loan-appraisal-approval/Loan%20Appraisal%20Breakdown.png)
- [loan eligibility breakdown.pdf](../../static/img/loan-appraisal-approval/loan%20eligibility%20breakdown.pdf)
- ![Generate Payment Schedule](../../static/img/loan-appraisal-approval/Generate%20Payment%20Schedule.png)
- ![Send for Approval](../../static/img/loan-appraisal-approval/send%20loan%20for%20approval.png)
- ![Approval actions](../../static/img/loan-appraisal-approval/Approval%20actions.png)
- Context screenshots I referenced:
  - ![Screenshot](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20151539.png)
  - ![Screenshot](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20152838.png)
  - ![Screenshot](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20153033.png)
  - ![Screenshot](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20153442.png)
  - ![Screenshot](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20153635.png)
  - ![Screenshot](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20154617.png)
  - ![Screenshot](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20154641.png)
  - ![Screenshot](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20154740.png)
  - ![Screenshot](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20155035.png)
  - ![Screenshot](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20155338.png)
  - ![Screenshot](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20160103.png)
  - ![Screenshot](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20160232.png)
  - ![Screenshot](../../static/img/loan-appraisal-approval/Screenshot%202025-10-31%20160318.png)
