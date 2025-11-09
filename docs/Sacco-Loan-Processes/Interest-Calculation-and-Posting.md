---
sidebar_position: 5
---

# Interest Calculation and Posting

The **total amount** to be repaid for a loan includes both the **principal** and the **interest** charged over the loan period.

The **interest rates** charged on loans are determined according to the **SACCO Policy**, which is regulated by **SASRA**.  
Each **loan product** has a minimum interest rate set up in the system — the rate charged to a specific client can vary, but it must remain within the policy limits.


## Interest Calculation Methods

There are four main types of **interest calculation methods** commonly used across loan products:

![Product Setup](/img/Interest-Calculation-And-Posting-1.jpg)

### 1. **Amortised Method**

For this method, the loan is repaid through **equal periodic installments**, which include both **principal and interest**.  
Over time, the **interest portion** of the repayment decreases because it is calculated based on the **remaining principal** after each repayment, while the **total payment** remains the same.

> Commonly used in: Mortgages, car loans, and long-term personal loans.


### 2. **Reducing Balance Method**

In this method, **interest is calculated on the remaining principal**, not on the original amount borrowed.  
As the principal reduces with each repayment, the **interest amount decreases** over time.

>  This results in a lower total interest compared to flat-rate methods.

### 3. **Reducing Flat Method**

With this method, **interest is calculated on the original principal**, but the **repayment schedule** is structured in a way that reduces the principal over time.  
This sometimes results in **slightly lower total interest** than a traditional flat-rate calculation.

> Acts as a middle ground between flat and reducing balance methods.


### 4. **Straight Line Method**

For this method, **interest is calculated on the original principal** for the **entire loan period**.  
The interest amount remains **constant** throughout the loan term.

> This method is simple but usually results in the **highest total interest** paid over time.

---

## Loan Product Setup

The **interest calculation method** is defined during **loan product setup** based on the **SACCO policy**.  

Once the interest is **charged**, it is **posted** — updating the relevant **General Ledger (G/L)** and **Loan Accounts**:

- **Credit:** Loan Account  
- **Debit:** Interest Income G/L Account

---

## Interest Calculation Process

For the loan at hand, interest is first calculated for a **specific billing period**.

![Interest Calculation Process](/img/Interest-Calculation-And-Posting-2.jpg)

Interest can be calculated **specifically** for individual loans or **generally** for all applicable loans, using filters in the system.

![Interest Filter](/img/Interest-Calculation-And-Posting-4.jpg)
![Interest Posting](/img/Interest-Calculation-And-Posting-5.jpg)

Once interest is generated, it is **posted** to the relevant **Credit** and **G/L Accounts**, and the **loan repayment** is determined as the sum of:

- The **Interest Amount**, and  
- The **Principal Repayment** for the loan.

<!-- Example Posting Image -->
![Entries Affected](/img/Interest-Calculation-And-Posting-6.jpg)



## Summary

| Method | Interest Basis | Payment Structure | Interest Trend | Typical Use |
|---------|----------------|-------------------|----------------|--------------|
| **Amortised** | Remaining Principal | Equal Installments | Decreases | Mortgages, long-term loans |
| **Reducing Balance** | Remaining Principal | Decreasing Interest | Decreases | Personal & SACCO loans |
| **Reducing Flat** | Original Principal (Adjusted) | Semi-decreasing | Slightly Decreases | Retail loans |
| **Straight Line** | Original Principal | Constant | Fixed | Short-term or simple loans |


:::tip[Note:]
 The method chosen during loan setup directly affects how repayments are structured, how interest accrues, and how postings are reflected in the SACCO’s financial records.

