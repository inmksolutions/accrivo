# 📊 Accrivo — Frequently Asked Questions & Navigation Guide

Welcome to the official Accrivo FAQ. This guide covers every feature in the app along with step-by-step navigation instructions to help you get the most out of your personal finance manager.

---

## Table of Contents

1. [General & Privacy](#1-general--privacy)
2. [Dashboard — Your Home Screen](#2-dashboard--your-home-screen)
3. [Accounts & Ledger Management](#3-accounts--ledger-management)
4. [Adding & Editing Transactions](#4-adding--editing-transactions)
5. [Dues & Managed Accruals](#5-dues--managed-accruals)
6. [Budget Plans](#6-budget-plans)
7. [Categories](#7-categories)
8. [Recurring Rules (Automation)](#8-recurring-rules-automation)
9. [Financial Overview (Reports)](#9-financial-overview-reports)
10. [Settings & Personalization](#10-settings--personalization)

---

## 1. General & Privacy

**Q: What is Accrivo?**
**A:** Accrivo is a privacy-first personal finance manager that uses professional **double-entry bookkeeping** principles to guarantee perfectly accurate records. It goes beyond basic expense tracking to help you manage loans, dues, credit cards, budgets, and long-term wealth — all while keeping your data 100% on your device.

**Q: Does Accrivo send my financial data to a server?**
**A:** No. Accrivo is **offline-first**. Your financial data is stored locally on your device only. There are no forced cloud syncs. The optional Google Drive backup is initiated only by you, and the backup file is saved directly in your own Drive.

**Q: Do you track my usage or send crash reports?**
**A:** We use Firebase for anonymized analytics and crash reporting to improve the app. However, you have **Total Telemetry Control**. You can easily opt out of Analytics, Crashlytics, and Cloud Messaging directly from the app's settings.

**Q: Is there any fraud prevention built-in?**
**A:** Yes. We utilize the Google Play Integrity API and Cloudflare to prevent fraudulent installations and secure our referral system, ensuring fair play without accessing your personal financial data.

**Q: Can I lock the app for extra security?**
**A:** Yes. Navigate to **Settings → Security & Lock** to configure a PIN-based lock. Once enabled, the app will require your biometric (fingerprint/face) or PIN to open. The lock screen also uses a security question as a fallback recovery method.

**Q: What does "double-entry bookkeeping" mean for me as a user?**
**A:** In practice, it means every financial action is perfectly balanced — money never appears from nowhere or disappears mysteriously. When you add an expense, your account balance decreases and the expense category increases. This guarantees your **Net Worth**, **Dues**, and **Account Balances** are always mathematically consistent.

---

## 2. Dashboard — Your Home Screen

The Dashboard is your financial command center. It is the first screen you see when you open the app.

**Navigation:** Open the app → You are on the **Dashboard**.

### What you see on the Dashboard:

**Cash Liquidity Card (Top)**
- Shows your total **spendable cash** — the combined balance of all your Bank accounts and Wallets.
- This is the money you can actually use today.

**Dues Summary Panel**
- Shows a real-time snapshot of your outstanding dues, split into three cards:
  - 🔴 **Overdue** — Dues that have already passed their due date. Tap to go directly to the Dues screen.
  - 🟢 **Total Pending** — Total amount across all active Payables and Receivables.
  - 🟡 **Due Soon** — Dues due within the next 7 days.
- Each card shows a **Payable** (you owe) and **Receivable** (owed to you) breakdown.

**Credit Utilization Panel** *(visible only if you have credit cards)*
- Shows your overall **credit utilization percentage** across all credit cards.
- Color-coded health status: `EXCELLENT` (≤30%), `MODERATE` (≤60%), `HIGH USAGE` (>60%).
- **Upcoming Statement Cycles:** A horizontal scroll list showing each credit card's unbilled amount and statement period end date. Tap any card to go to its ledger.

**Recent Activity Section**
- Shows your **5 most recent transactions** with their description, date, and amount.
- Color-coded: Green for income, Red for expenses, App-color for transfers.
- Tap any transaction to edit it.
- Tap **"View All"** to go to the full Transactions list.

**Side Drawer**
- Tap the ☰ menu icon (top-left) to open the **App Drawer**, which is the main navigation hub for all sections of the app.

---

## 3. Accounts & Ledger Management

Manage all your financial accounts — bank accounts, wallets, credit cards, and people you owe money to or who owe you.

**Navigation:** App Drawer → **Accounts**

### Screen Layout:
Accounts are organized in three sections:
- **ASSETS** — Bank accounts, wallets, cash, and other assets you own.
- **LIABILITIES** — Credit cards and other accounts representing what you owe.
- **PEOPLE** — Contacts with outstanding loans (money you lent or borrowed).

### Key Actions:

**Q: How do I add a new account?**
**A:** On the Accounts screen, tap the **`+` (Add) button** at the bottom right. Choose the account type (Bank, Wallet, Credit Card, etc.), enter its name, opening balance, and any additional details like credit limit.

**Q: How do I view an account's transaction history (ledger)?**
**A:** Tap on any account card. This opens the account's **Ledger View**, which shows every transaction affecting that account, sorted by date.

**Q: How do I edit or archive an account?**
**A:** Tap the **Edit (pencil) icon** in the top-right of the Accounts screen to enter **Edit Mode**. Each account card will show edit and archive buttons. Tap the **pencil icon** on a specific card to edit it, or the **archive icon** to deactivate it.

**Q: Can I hide accounts with a zero balance?**
**A:** Yes. Tap the **eye icon** in the top-right of the Accounts screen to toggle visibility of zero-balance accounts.

**Q: What does it mean to "archive" vs "delete" an account?**
**A:** If an account has linked transactions, it cannot be fully deleted — it will be **archived** instead. Archived accounts are hidden from the main list but retain their full transaction history. You can view and restore them from the "ARCHIVED ACCOUNTS" section at the bottom of the Accounts screen.

**Q: How do I see the money I've lent to or borrowed from a person?**
**A:** In the **PEOPLE** section of the Accounts screen, each contact is listed with a net balance showing whether they owe you or you owe them. Tap the contact to open a **Contact Ledger**, which shows all loan and repayment transactions with that person.

**Credit Card Features:**
- Credit card accounts display an **available credit** and **credit limit** progress bar directly on the card, color-coded by utilization (green/amber/red).
- An **OVERLIMIT** badge appears if the outstanding balance exceeds the credit limit.

---

## 4. Adding & Editing Transactions

The transaction entry form is the most powerful screen in the app. It supports two different modes to fit your workflow: **Standard Mode** and **Advanced Ledger Mode**. You can switch between them in Settings.

**Navigation:** Tap the **`+` (Add) floating button** anywhere, or from a ledger, or from the App Drawer → **Add Transaction**.

### 1. Standard Mode (Intent-Based)
Best for most users. It provides a guided, step-by-step form based on your intent.
- **Expense (↑):** Money leaving your account (e.g., groceries). Select where the money is coming FROM, then choose an Expense Category.
- **Income (↓):** Money coming into your account (e.g., salary). Choose an Income Category (source), then select where the money is going TO.
- **Transfer (⇄):** Moving money between your own accounts. Select the FROM account and the TO account.

### 2. Advanced Ledger Mode (Auto-Detect)
Best for power users. A lightning-fast, single-screen interface.
Instead of manually selecting Expense/Income/Transfer tabs, you simply select two accounts. The app **automatically detects** the transaction type based on the accounts you choose (e.g., selecting Wallet and Bank automatically creates a Transfer).

### Transaction Live Preview
As you fill out the form, Accrivo generates a real-time, natural language visual preview of the transaction's impact before you even save it, guaranteeing absolute accuracy.

**Q: Can I split a transaction across multiple categories?**
**A:** Yes. For Expense and Income transactions, tap **"+ Add Split"** to add another category row. Each row has its own amount and category. The total of all splits should match the header amount. The header amount auto-calculates from the splits unless you manually type it.

**Q: Can I backdate a transaction?**
**A:** Yes. Tap the **Transaction Date** field and pick any past date.

**Q: Can I attach receipts to my transactions?**
**A:** Yes! You can attach photos of your receipts directly to a transaction. These images are stored **strictly locally** on your device and are never uploaded to our servers, maintaining your absolute privacy.

**Q: How do I edit or delete a transaction?**
**A:** Tap any transaction from a ledger or the Recent Activity list on the Dashboard. The same "Add Transaction" form opens in **Edit Mode**, pre-filled with the existing data. A **delete (trash) icon** appears in the top-right to remove it.

---

## 5. Dues & Managed Accruals

The Dues screen shows all your active financial obligations — money you owe and money owed to you — with due dates and urgency levels.

**Navigation:** App Drawer → **Managed Dues**, or tap any Dues card on the Dashboard.

### Screen Layout:

**Summary Card (Top)**
- Shows three totals at a glance:
  - 🟢 **Receivable** — Total pending amount others owe you.
  - 🔴 **Payable** — Total pending amount you owe others.
  - ⚖️ **Net Dues** — Your net position (positive = you're owed more).

**Grouped Sections:**
Dues are automatically sorted into three collapsible groups:
- 🔴 **Overdue** — Past their due date.
- 🟡 **Due Today** — Due today.
- 🔵 **Upcoming** — Future due dates.

Tap any section header to collapse or expand it.

**Q: How do I add a due/accrual?**
**A:** Dues are created automatically when you use **Advanced Ledger Mode** to transfer money between a Bank/Wallet and a Person account (Lending or Borrowing). You can also have a **Recurring Rule** create a due reminder automatically on a schedule.

**Q: How do I settle (mark as paid) a due?**
**A:** Tap on any due card. A **Settle Options** dialog will appear, letting you record a partial or full settlement payment, which automatically creates the corresponding transaction.

**Q: How do I search for a specific due?**
**A:** Tap the **🔍 Search icon** in the top-right of the Dues screen. Type a contact name, account name, or title to filter the list in real time.

**Q: Can I filter dues by type or urgency?**
**A:** Yes. Tap the **"Filter" floating button** at the bottom right. A bottom sheet opens with:
- **Type filters:** All, Payables, or Receivables.
- **Timing filters:** All, Overdue, Due Today, or Due Soon.

Tap **Apply Filters** to confirm. An active filter badge shows how many filters are enabled.

**Q: What is the swipe gesture on due cards?**
**A:** Swipe a due card to reveal quick actions (this is an interactive hint shown to first-time users with a "peek" animation to help you discover the feature).

---

## 6. Budget Plans

Create date-range budget plans to set spending targets and track your actual spending against them.

**Navigation:** App Drawer → **Budgets**

### Screen Layout:

The Budgets screen has **three tabs:**

| Tab | Description |
|---|---|
| **Plans** | Your active, draft, and archived budget plans |
| **Templates** | Saved reusable budget structures |
| **Projections** | Forward-looking financial projections |

### Plans Tab:

**Q: How do I create a budget plan?**
**A:** On the Budgets screen, tap the **`+` button** in the top-right corner, or the **"New Plan"** button. This opens the **Budget Wizard**, a step-by-step guide to set up your plan:
1. Set a plan name and date range (start and end dates).
2. Add envelopes (spending categories with allocation amounts).
3. Optionally set income targets.
4. Activate or save as draft.

**Q: What is an "envelope"?**
**A:** An envelope is a budget line item — a specific spending category (e.g., Food, Rent, Entertainment) with an allocated amount. The Budget Plan distributes your total budget into these envelopes.

**Q: How do I track spending against my budget?**
**A:** Tap on any budget plan card to open the **Budget Detail Screen**. It shows each envelope with:
- The allocated amount.
- The actual amount spent (pulled from your real transactions).
- A visual progress bar color-coded by how close you are to the limit.

**Q: How do I duplicate a plan for the next month?**
**A:** Long-press any budget plan card to open the Actions menu. Select **"Copy to Next Period"** to create a duplicate plan with dates shifted forward by one period. This is ideal for monthly budgets.

**Q: How do I save a budget as a template for reuse?**
**A:** Long-press a plan card → **"Save as Template"**. Give the template a name. It will appear in the **Templates** tab and can be used to quickly start new plans with the same structure.

**Q: What do the status badges on plan cards mean?**
| Badge | Meaning |
|---|---|
| `ACTIVE` | Plan is currently running within its date range |
| `DRAFT` | Plan saved but not yet activated |
| `ENDED` | Plan's end date has passed |
| `ARCHIVED` | Manually archived / no longer in use |

---

## 7. Categories

Organize your income and expenses into a custom hierarchy of groups and subcategories.

**Navigation:** App Drawer → **Categories**

### Screen Layout:

Categories are split into two top-level sections:
- **EXPENSE** — Categories for tracking where money goes (e.g., Food → Groceries, Dining).
- **INCOME** — Categories for tracking where money comes from (e.g., Salary, Freelance).

Each section contains expandable **Category Groups**, which can hold **Subcategories** inside.

### Key Actions:

**Q: How do I add a new category group?**
**A:** Tap the **"Add Group" button** at the bottom right. A form sheet slides up — select the type (Expense or Income), choose an icon, enter a name, and save.

**Q: How do I add a subcategory?**
**A:** Expand any category group by tapping on it. On the group header, tap the **`+` circle icon** to add a subcategory inside that group.

**Q: How do I edit or delete a subcategory?**
**A:** Slide any subcategory row to the **left** to reveal Edit (blue) and Delete (red) actions. Alternatively, tap the **⋮ (three-dot) menu** on the subcategory row.

**Q: How do I edit or delete a category group?**
**A:** Tap the **⋮ (three-dot) menu** on the group header → select **"Edit Group"** or **"Delete Group"**. Deleting a group also removes all its subcategories.

**Q: What happens to past transactions if I delete a category?**
**A:** Transactions are preserved. The category is **archived** rather than hard-deleted if transactions are linked to it, ensuring no historical data is lost.

---

## 8. Recurring Rules (Automation)

Set up rules to automate the tracking of regular, repeating financial events like subscriptions, salary, or loan repayments.

**Navigation:** App Drawer → **Recurring Rules**

### Screen Layout:

The screen has two tabs:
- **Active** — Rules that are currently running and will generate future entries.
- **History** — Rules that have been stopped or completed.

Each rule card shows:
- Rule name and type (Expense/Income/Transfer).
- Frequency (e.g., "Monthly – From 01 Jan 26").
- Next Due Date.
- Mode badge: `TRANSACTION` (auto-posts to ledger), `DUE REMINDER` (creates a notification/due), or `TRANSACTION + DUE REMINDER`.

### Key Actions:

**Q: How do I create a new recurring rule?**
**A:** Tap the **"New Rule" button** at the bottom right. The **Add Recurring Rule Screen** opens with these fields:
1. **Name** — e.g., "Netflix Subscription".
2. **Type** — Expense, Income, Transfer, or Due.
3. **Amount** — Fixed amount for the rule.
4. **Accounts** — Which account(s) it affects.
5. **Category** — Expense or income category.
6. **Frequency** — Daily, Weekly, Monthly, Quarterly, Yearly, or One-time.
7. **Start Date / End Date** — When the rule begins and optionally ends.
8. **Mode** — Choose whether to **Auto-post a transaction** (recommended for automatic tracking) or just **create a Due Reminder** (sends a notification on the due date for manual action).

**Q: What does "Auto-post" mean?**
**A:** When enabled, the system automatically records the transaction to your ledger on the scheduled date — no manual action needed. Perfect for predictable fixed bills like rent or subscriptions.

**Q: Can a recurring rule also create a due reminder?**
**A:** Yes. Enable **"Also create a Due Reminder"** when setting up an auto-posting rule. This gives you a notification AND posts the transaction — useful for bills you want to verify before they're recorded.

**Q: How do I delete a recurring rule?**
**A:** Swipe the rule card from **right to left** to reveal a red delete action. Confirm the deletion. Past transactions created by the rule are not affected.

**Q: Can I edit a rule?**
**A:** Yes. Tap any rule card to open it in Edit mode.

**Q: What are "Loan Repayment" rules?**
**A:** When you record a transaction involving a Person with an installment repayment schedule, Accrivo automatically creates a **Loan Repayment** recurring rule to track the schedule. These are marked with the `LOAN REPAYMENT` badge and linked to the original transaction.

---

## 9. Financial Overview (Reports)

Get a complete picture of your financial health, wealth trends, and account allocations.

**Navigation:** App Drawer → **Financial Overview**

### Screen Sections:

**Net Worth Header**
- Shows your **total Net Worth** (all Assets minus all Liabilities).
- Displays a **momentum indicator** — the percentage change vs. last month (↑ green = growing, ↓ red = shrinking).
- Tap the card to see a tooltip explaining how Net Worth is calculated.

**Intelligence KPI Grid**
Four metric cards displayed in a 2×2 grid. Tap any card to see a detailed explanation tooltip:

| Metric | What It Means |
|---|---|
| **Savings Rate** | % of your monthly income that you kept (not spent). Higher is better. |
| **Runway** | How many months/years your current liquid assets would last based on your average monthly expenses. |
| **Debt Ratio** | Your total liabilities as a % of your total assets. Lower is better (under 20% = Good Standing). |
| **Burn Rate** | Your average daily spending cost based on the last 6 months. |

**Monthly Cash Flow Chart**
- A line chart showing **Income vs. Expenses** over the last 6 months.
- Green line = income, Red line = expenses.

**View Detailed Trends**
- Tap the **"View Detailed Trends"** banner to open the **Cash Flow Insights Screen**, which provides a deeper per-month breakdown.

**Asset Allocation**
- Expandable cards for **ASSET** and **LIABILITY** breakdowns.
- Shows every account within each category with its balance and a proportional progress bar showing what % of the total it represents.

---

## 10. Settings & Personalization

Customize your Accrivo experience, manage backups, and control security.

**Navigation:** App Drawer → **Settings**

### Settings Sections:

#### 🔵 Account & Subscription
**Cloud & Account** → Tap to access:
- **Google Drive Backup** — Back up your local database to your own Google Drive.
- **Restore from Backup** — Restore your database from a previous Google Drive backup.
- **Pro Subscription** — Manage your Accrivo Pro plan.
- **Referrals** — Share your referral code to unlock benefits.

#### 🔵 Preferences

**Theme & Appearance**
- Navigate: **Settings → Theme & Appearance**
- Choose **Light**, **Dark**, or **System** (follows phone settings).
- Select from multiple **color palettes** (each with a unique name and emoji) to customize the app's accent color.

**Localization**
- Navigate: **Settings → Localization**
- Set your **currency symbol** (e.g., ₹, $, €).
- Set your **number format** (e.g., Indian or International format).

**Notifications**
- Navigate: **Settings → Notifications**
- Configure which events trigger reminders (e.g., due dates for accruals, recurring rule alerts).

#### 🔵 Local Data Security & Backup

**Security & Lock**
- Navigate: **Settings → Security & Lock**
- Set up a **PIN** to lock the app.
- Configure **Biometric Unlock** (fingerprint/face).
- Set up **Security Questions** as a fallback recovery method.

**Export to Excel / CSV** *(Pro / Adventurer feature)*
- Navigate: **Settings → Export to Excel / CSV**
- Generate reports exportable in Excel or CSV format for external analysis.

#### 🔵 Maintenance

**Re-sync All Balances**
- Tap to force a full recalculation of all account and category balances from scratch.
- Use this if you ever suspect a display inconsistency.

#### 🔵 Privacy & About

**Analytics, Stability & Cloud Messaging**
- Toggle to share (or not share) anonymous crash reports and usage data. You can also opt out of Firebase Cloud Messaging (FCM) token uploads, while still receiving anonymous app announcements.

**Send Feedback**
- Tap to open a feedback form where you can report a bug or suggest a new feature.

**About Accrivo**
- Opens the official Accrivo website with more information about the mission and roadmap.

---

## 💡 Tips & Best Practices

- **Start with Accounts:** Before adding any transactions, set up all your bank accounts, wallets, and credit cards in the **Accounts** section with their correct current balances (as Opening Balance).
- **Use Categories:** The more specific your categories, the better your budget tracking and reports will be.
- **Check the Dashboard Daily:** The Dashboard is designed to show the most actionable information — check it regularly for overdue dues and credit utilization alerts.
- **Automate What You Can:** Use **Recurring Rules** for fixed monthly expenses like rent, insurance, or subscriptions to minimize manual entry.
- **Back Up Regularly:** Periodically go to **Settings → Cloud & Account** and create a backup to your Google Drive to ensure your data is always safe.
