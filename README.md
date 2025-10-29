# Loan Process User Manual for Business Central (Sacco)

Welcome to the **Loan Process User Manual** documentation project for **Microsoft Dynamics 365 Business Central (Sacco)**.

This repository hosts the Docusaurus-based documentation site, which serves as the comprehensive user manual for Sacco's loaning operations.



##  Project Overview

This documentation project captures and explains all loan management processes in **Business Central**, including:

* Loan Application & Qualification
* Loan Appraisal & Approval
* Loan Disbursement
* Guarantor Management
* Loan Repayment
* Interest Calculation & Posting
* Loan Rescheduling / Refinancing / Top-up
* Loan Reports

The documentation mirrors the **Microsoft Learn** style and structure.



##  Getting Started

Follow these steps to set up and contribute to the documentation locally.

### 1. Clone the Repository

Use SSH (recommended):

```bash
git clone git@github.com:Raddames-Tonui/loan_process_user_manual_bc.git
```

Or HTTPS:

```bash
git clone https://github.com/Raddames-Tonui/loan_process_user_manual_bc.git
```

Then navigate into the project folder:

```bash
cd loan_process_user_manual_bc
```



### 2. Install Dependencies

You can use **pnpm** (preferred for speed and consistency) or **npm**.

#### Option A: Using pnpm

Install pnpm globally if you don’t have it:

```bash
npm install -g pnpm
```

Then install the project dependencies:

```bash
pnpm install
```

#### Option B: Using npm

If you prefer npm:

```bash
npm install
```



### 3. Run the Documentation Site Locally

Start the Docusaurus development server:

#### Using pnpm:

```bash
pnpm start
```

#### Using npm:

```bash
npm run start
```

Then open your browser and go to:

```
http://localhost:3000
```

This allows you to preview your changes in real-time.



### 4. Project Structure

```
loan_process_user_manual_bc/
├─ docs/                    # Markdown documentation files
├─ static/img/              # Images and screenshots
├─ src/                     # Components and custom pages
├─ sidebars.js              # Sidebar navigation (Table of Contents)
├─ docusaurus.config.js     # Site configuration
├─ package.json             # Dependencies and scripts
└─ README.md                # This file
```

All documentation files (`.md`) should live inside `/docs/`.



##  Collaboration Workflow

We follow a **branch-based workflow** to maintain consistency.

### 1. Create a New Branch

Each contributor should work on a feature or section in a separate branch:

```bash
git checkout -b feature/loan-disbursement
```

Use meaningful names for branches, e.g.:

* `feature/loan-application`
* `update/interest-calculation`
* `fix/sidebar-order`

### 2. Make Your Edits

* Add or edit documentation in the `/docs/` folder.
* Add screenshots under `/static/img/`.

### 3. Stage and Commit Changes

```bash
git add .
git commit -m "Added Loan Disbursement documentation section"
```

### 4. Push Your Branch to GitHub

```bash
git push origin feature/loan-disbursement
```

### 5. Open a Pull Request

* Go to the GitHub repository: [Loan Process User Manual BC](https://github.com/Raddames-Tonui/loan_process_user_manual_bc)
* Click **Compare & Pull Request**
* Provide a brief description of your changes
* Assign reviewers if applicable

Once reviewed and approved, your branch will be **merged** into the `development` branch and finally to `main` if no conflicts.



##  Deployment (for Maintainers)

Deployment is handled through **Netlify**:

* **Build command:** `pnpm run build`
* **Publish directory:** `build`

Each push to `main` automatically triggers a new deployment.



##  Documentation Standards

To maintain consistency with Microsoft Learn style:

* Use clear section headings (`##`, `###`).
* Write step-by-step instructions.
* Include screenshots where possible.
* Use callouts for notes:

  ```md
  > [!NOTE]
  > Only authorized users can approve loan applications.
  ```
* Keep formatting consistent across all sections.



## 🧩 Useful Commands

| Command          | Description                                  |
| - | -- |
| `pnpm start`     | Start local development server               |
| `pnpm run build` | Build static production files                |
| `pnpm run serve` | Serve production build locally               |
| `git status`     | Check modified files                         |
| `git pull`       | Sync your branch with the latest main branch |



##  Tips for Effective Collaboration

* Always pull the latest `development` branch before starting new work:

  ```bash
  git checkout development
  git pull origin development
  ```
* Keep commits focused and descriptive.
* Avoid committing large binary files (e.g., raw screenshots >2MB).
* Maintain consistency in tone, structure, and formatting.



##  Summary

This repository is the single source of truth for the **Sacco Loaning Process Manual in Business Central**. All contributors should:

* Use the provided structure
* Follow branching and PR guidelines
* Maintain Microsoft Learn–style clarity and professionalism

Once your changes are merged, the live documentation will automatically update on Netlify.



<!-- **Maintainer:** Raddames Tonui -->
**Repository:** [git@github.com:Raddames-Tonui/loan_process_user_manual_bc.git](git@github.com:Raddames-Tonui/loan_process_user_manual_bc.git)

