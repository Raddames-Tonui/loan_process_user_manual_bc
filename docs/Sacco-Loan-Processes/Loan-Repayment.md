---
sidebar_position: 6
---

# Loan Repayment

Once the loan interest has been calculated and posted, the next step is to process the **loan repayment**.  
Each repayment consists of two key components:

- **Principal Repayment** – The portion of the installment that reduces the outstanding loan balance.  
- **Interest Repayment** – The portion that covers the interest charged for the billing period.

The **repayment schedule** is automatically determined based on the **interest calculation method** selected during the loan product setup.

To generate a repayment schedule, click the **Generate Repayment Schedule** on the actions under the home tab

![Generate Loan Repayment](/img/Loan-Repayment-1.jpg)

> 💡 Ensure that the Loan Account is updated before generating the repayment schedule

For our loan here is the generated repayment schedule: [Loan Repayment Schedule](/files/Loan-Repayment-Schedule.pdf)

> 📉 Notice how the **interest** portion decreases while the **principal** portion increases each month, keeping the **total payment constant**.

---

### Loan Repayment Methods

The repayment is done based on the repayment method  that is determined during the loan application process.
Each loan setup has a specified repayment methods that is per sacco policy.

The repayment methods include: CheckOff, Salary, Direct Debit, Mobile Money, Board Allowance, Standing Order(Internal), Standing Order(External), Dividend, Pension

This repayment method(s) can be adjusted even after the loan is posted and disbursed.

The repayment method for the loan above is : **Salary**
![Generate Loan Repayment](/img/Loan-Repayment-2.jpg)

---

### 🧾 Repayment Posting

Though the repayment is using salary- the loan can be repayment can be done through any of the repayment methods of the loan setup.

For the user loan the repayment was done through a direct debit via a receipt.

![Receipt](/img/Loan-Repayment-3.jpg)

The user can suggest member loans to be repaid then it is repaid according to the outstanding amount.
The recovery amount includes the principal amount plus the accrued interest.

![Loan Repayment](/img/Loan-Repayment-4.jpg)

When a repayment is made, the system updates the relevant accounts as follows:

| Transaction | Account Debited | Account Credited |
|--------------|----------------|------------------|
| **Loan Repayment** | Member Deposit / Cash / Bank | Loan Account |
| **Interest Portion** | Loan Account | Interest Income G/L Account |

![Loan Repayment](/img/Loan-Repayment-6.jpg)

The General Ledger entries:

![Loan Repayment](/img/Loan-Repayment-8.jpg)

> 💡 The loan balance reduces after each repayment, and future interest is calculated based on the **new outstanding principal** (depending on the interest method).

The outstanding interest is zero and the next repayment is as per the repayment schedule.

![Loan Repayment](/img/Loan-Repayment-5.jpg)

---

### ⚙️ Repayment Processing Summary

When repayments are processed:

1. The repayment amount is **split** between interest and principal automatically.  
2. **Interest income** is posted to the respective **G/L account**.  
3. **Principal repayment** is applied to reduce the **loan balance**.  
4. The **member statement** and **loan ledger** are updated in real time.

---
For this member's Loan Repayment, after the receipt is posted, the system will automatically:

- Update the **loan balance**,  
- Post to the **General Ledger**, and  
- Reflect the repayment in the **member’s loan statement**.

---

> ✅ **Summary:**  
> Loan repayments cover both **principal and interest**, and the method of calculation (Amortised, Reducing Balance, Reducing Flat, or Straight Line) determines how these amounts change over time and how interest is applied to the loan balance.
