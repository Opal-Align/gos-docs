# OPAL gOS — Platform Overview

## What is OPAL gOS?

OPAL gOS is a practice management platform designed to improve your practice's efficiency, revenue cycle, and patient engagement. It guides your team through the natural flow of a patient's journey — from scheduling and eligibility verification through to collections and follow-up.

## Accessing the Platform

- **URL:** https://platform.opalalign.com/login
- **Credentials:** Provided by your manager on go-live day

## Account Setup

On go-live day, practice managers and office leads receive an invitation email from `invite@microsoft.com`.

1. Click **Accept Invitation** in the email
2. Enter the security code sent to your registered email
3. You will be redirected to https://platform.opalalign.com automatically
4. Log in with your credentials

For login issues, contact: **Support@OpalAlign.com**

## Primary Navigation

```
Relay  »  Collect  »  Produce  »  Schedule
```

Each tab represents a key area of your practice's daily workflow. Your access level determines which tabs and features are visible to you.

## User Access Levels

| Level | Role | Description |
|-------|------|-------------|
| L1 | Staff | Day-to-day task completion |
| L2 | Senior Staff / Front Desk | Can escalate, reassign tasks, and manage users |
| L3 | Practice Manager | Manages multiple practices, full access to Settings |
| L4 | Revenue Cycle Manager | Highest authority — home screen shows Collections Queue directly |

## Home Screen (L1–L3)

After logging in, L1–L3 users see a dashboard with:

- **KPI Summary** — live counts for Relay, Collect, Produce, and Schedule activity
- **OPALescence Points** — your personal score from completed tasks
- **Current Streak** — consecutive days with task activity, plus your all-time best
- **MTD Trend** — your month-to-date OPALescence total
- **Leaderboards** — Practice and Global rankings, updated in real time

> **L4 users** are taken directly to the Collections Queue on login — no dashboard.

## Top Navigation Bar

In addition to the four main tabs, the top bar includes:

| Element | Description |
|---------|-------------|
| Patient Search | Search any patient by name across all screens |
| Practice Selector | Switch between practices without logging out (appears when you manage more than one practice) |
| Settings (gear icon) | Access Settings (L2 can access Users; L3 accesses all settings) |
| Profile Avatar | Shows your name and role on hover |

## Support

- **In-app chatbot:** gEMMAi — available at the bottom right of every screen
- **Email support:** Support@OpalAlign.com

---

---

---

---

# Relay

## Overview

Relay is your team's communication hub. It centralizes all patient messaging, eligibility verification, and outreach tracking in one place so nothing falls through the cracks.

## Subtabs

### Message Inbox

Real-time two-way SMS inbox for patient conversations. You can send and receive messages, use pre-loaded templates, and take action on a patient's account without leaving the inbox.

**Columns:**
- Patient name and contact information
- Section and subsection (Collect or Produce) the patient belongs to
- Unread message badge when new messages arrive

**Features:**
- Filter conversations by section (Collect or Produce)
- Search for a patient by name
- Send a message, make a call, or override/reassign from within the inbox

---

### Missing Contacts

Patients without a valid phone number or email address appear here. These patients cannot receive automated outreach until their contact information is updated in your Practice Management System (PMS).

**Filter options:** All Types, Missing Phone, Missing Email, Missing Both

**Columns:**

| Column | Description |
|--------|-------------|
| Patient | Searchable by name |
| Contact | Phone number and email on file |
| Address | Mailing address |
| Amount | Sortable — outstanding balance |
| Last Appt. | Sortable — most recent appointment date |
| Missing | Badge showing what contact info is missing (Phone, Email, or Both) |

---

### Write Off

The Collections Queue for write-off review. Shows accounts that have completed all outreach steps and are ready for write-off review.

> **Visible to L4 users only.**

A **Download CSV** button at the top exports the full list with guarantor details, patient info, addresses, balances, and SSN/chart numbers for external collections processing.

**Columns:**

| Column | Description |
|--------|-------------|
| Guarantor | Name and phone number |
| Patient | Name and date of birth |
| Practice | Practice name (searchable — L4 only) |
| Last Appt. | Filterable by date range |
| Patient Balance | Sortable |
| History | Sortable — outreach progress tracker |
| Action | Message, Call, Override, Reassign (visible to L4) |
| Write Off | Checkbox to confirm write-off — triggers a confirmation dialog before finalizing |

---

### Lifecycle

Shows all patients currently in the automated outreach sequence — either scheduled to receive a future message or waiting for their next step.

**Filter options:** Section (Collect / Produce), Message Type (SMS, Email, Mail, Call)

**Columns:**

| Column | Description |
|--------|-------------|
| Patient | Searchable by name |
| Contact | Phone number and email |
| Amount | Sortable — outstanding balance |
| Last Appt. | Sortable — most recent appointment |
| Last Sent | Date the most recent automated message was sent |
| History | Outreach progress tracker |
| Next | The type of the next scheduled outreach step (SMS, Email, Mail, Call) |
| Status | Delivery status of the last sent message |

---

### Schedule Requests

> This tab is enabled based on your practice configuration.

Displays incoming appointment schedule requests from patients. Use this view to review and manage requests submitted through patient-facing outreach.

---

---

---

---

# Schedule

## Overview

The Schedule tab gives your team visibility into patients who need follow-up to get back on the books. Each view surfaces a different category of scheduling gap so you can target outreach at the right patients.

## Subtabs

### VOB

An appointments view available to practices with the appointments feature enabled. This is the default view when you open the Schedule tab.

### No Reappointments

Patients who do not have a future appointment scheduled and need to be reappointed.

### No Shows

Patients who missed a scheduled appointment and have not yet been rescheduled.

### Reactivations

Patients who have not been seen in a significant period and need to be re-engaged to resume care.

### Overdue Appts

Patients who are overdue for an appointment based on their treatment plan or recall schedule. This view includes an extra **Procedure** column showing the specific procedure code and description driving the overdue flag.

---

## Role-Based Views

Each Schedule view is organized into sections based on your user level:

| Section | Visible to |
|---------|------------|
| Office | L2, L3 and above |
| All Patients | L1, L2, L3 |

---

## Table Columns

### No Reappointments / No Shows / Reactivations

| Column | Description |
|--------|-------------|
| OPALescence | Sortable — higher score = higher priority |
| Guarantor | Responsible party and phone number |
| Patient | Searchable by name |
| Last Appt. | Filterable by date range — most recent appointment date |
| History | Sortable — click to view outreach progress and task history |
| Action | Message, Call, Override, Reassign |

### Overdue Appts

| Column | Description |
|--------|-------------|
| OPALescence | Sortable — higher score = higher priority |
| Guarantor | Responsible party and phone number |
| Patient | Searchable by name |
| Last Appt. | Filterable by date range — most recent appointment date |
| Procedure | Procedure code and description driving the overdue flag |
| History | Sortable — click to view outreach progress and task history |
| Action | Message, Call, Override, Reassign |

---

---

# Produce

## Overview

Produce is designed to proactively generate appointments through automated patient outreach. The system handles the first contact attempts automatically. Patients only surface in the Produce tables after automation has been exhausted and manual follow-up is required.

## How Automation Works

When a patient matches one of the Produce categories, gOS automatically sends outreach messages over a defined period requesting that the patient schedule an appointment.

- If the patient schedules during the automated sequence → no further action needed, they do not appear in the table
- If the patient does not schedule after automation completes → they escalate to the Produce table for manual follow-up

## Subtabs

### Missed Appts.

Patients who missed or canceled a scheduled appointment and have not yet been rescheduled. This is the default view when you open Produce.

### Tx Follow Up

Patients with diagnosed treatment on record that has not been scheduled. Use this view to follow up on accepted or pending treatment plans and convert them into scheduled appointments.

---

## Role-Based Views

Each Produce view is organized into sections based on your user level:

| Section | Visible to |
|---------|------------|
| Office | L2, L3 and above |
| All Patients | L1, L2, L3 |

---

## Table Columns

Both Produce views share the same columns:

| Column | Description |
|--------|-------------|
| OPALescence | Sortable — higher score = higher priority |
| Guarantor | Responsible party and phone number |
| Patient | Searchable by name |
| Provider | Assigned provider |
| Last Appt. | Sortable — most recent appointment date, with days-ago indicator |
| History | Sortable — click to view outreach progress and full task history |
| Action | Message, Call, Override, Reassign |

---

---

---

---

# Collect

## Overview

Collect organizes outstanding patient balances into focused views so your team can efficiently identify, prioritize, and follow up on revenue. Navigate between views using the tabs at the top of the screen.

## Views

### Missed OTC
Patients who had an appointment yesterday and left with an unpaid balance. These are high-priority — timely outreach significantly increases the likelihood of successful collection.

### A/R - with Appt.
Patients who have an upcoming appointment and an outstanding balance. An ideal opportunity to resolve the balance before or during their scheduled visit.

### A/R - without Appt.
Patients who owe a balance but have no future appointment scheduled. Requires proactive outreach to resolve the balance and, when appropriate, schedule continued care.

### Aged A/R
Patients with balances that have remained outstanding over an extended period. Use this view to identify and prioritize long-standing accounts that require follow-up.

### Problem Claims
Insurance claims that require immediate attention due to submission issues, payer rejections, missing documentation, or unsupported claim types. This view is enabled based on your practice configuration.

---

## Role-Based Views

Within each Collect view, the patient list is organized into sections based on your user level:

| Section | Visible to |
|---------|------------|
| Corporate | L3 and above |
| Office | L2, L3 and above |
| All Patients | L1, L2, L3 |

---

## Table Columns

Each view has specific columns tailored to its workflow.

### Missed OTC

| Column | Description |
|--------|-------------|
| OPALescence | Sortable — higher score = higher priority |
| Guarantor | Responsible party for the account |
| Patient | Searchable by name |
| Provider | Assigned provider |
| Collected at Last Appt. | Amount collected during the most recent visit |
| Appointment | Sortable — most recent appointment time and last date of service |
| Patient Balance | Sortable — outstanding amount owed |
| History | Sortable — click to view outreach progress and full task history |
| Action | Message, Call, Override, Reassign |

### A/R - with Appt.

| Column | Description |
|--------|-------------|
| OPALescence | Sortable — higher score = higher priority |
| Guarantor | Responsible party for the account |
| Patient | Searchable by name |
| Provider | Assigned provider |
| Last Appt. | Filterable by date range — most recent appointment date |
| Next Appt. | Filterable — upcoming scheduled appointment date |
| Patient Balance | Sortable — outstanding amount owed |
| History | Sortable — click to view outreach progress and full task history |
| Action | Message, Call, Override, Reassign |

### A/R - without Appt.

| Column | Description |
|--------|-------------|
| OPALescence | Sortable — higher score = higher priority |
| Guarantor | Responsible party for the account |
| Patient | Searchable by name |
| Provider | Assigned provider |
| Last Appt. | Filterable by date range — most recent appointment date |
| Patient Balance | Sortable — outstanding amount owed |
| History | Sortable — click to view outreach progress and full task history |
| Action | Message, Call, Override, Reassign |

### Problem Claims

| Column | Description |
|--------|-------------|
| OPALescence | Sortable — higher score = higher priority |
| Guarantor | Responsible party for the account |
| Patient | Includes a button to open the EOB document |
| Payor | The insurance company associated with the claim |
| Claim Info | Sortable — claim amount and original submission date |
| Problem | Filterable — type of issue flagging the claim |
| Source | Sortable — click to open full task history |
| Action | Resubmit, Call, Override, Reassign |

---

## Problem Claims — Explanation of Benefits (EOB)

Each Problem Claim includes an EOB — a document issued by the insurance payer detailing how the claim was processed. Click the document icon next to the patient name to open it. The EOB shows:

- Services rendered
- Amount billed by the provider
- Amount approved and paid by insurance
- Remaining patient responsibility

The EOB is your primary source of truth for understanding claim outcomes, reconciling payments, and determining next steps for patient billing or follow-up.

---

## Queue Management

Collect patients can be moved between queues using the Override action button. Available actions include:

| Action | Description |
|--------|-------------|
| Move to Omission Queue | Exempt a patient from automated outreach — they will not receive automated messages |
| Move to Automation Queue | Return an omitted patient back to the automated outreach schedule |
| Move to Collections Queue | Flag a patient for external collections review — reviewed and finalized by L4 users |
| Move to Mailer | Send a patient to the USPS mail queue |

---

# Guided Workflows

## Overview

Every patient row across Relay, Collect, Produce, and Schedule includes a set of action buttons that guide your team through the correct workflow. These buttons ensure consistent, compliant, and effective outreach.

## Action Buttons

### SMS / Text (Message)

Opens a fully functional two-way chat interface with the patient.

| Feature | Detail |
|---------|--------|
| Message Templates | Preloaded templates organized by tonality |
| Text-to-Pay | Embedded payment link for easy patient payment |
| 3rd Party Financing | Embedded financing link |
| Real-time Updates | Messages sync instantly — both directions |
| Message History | Infinite scroll through full conversation history |
| Character Limit | 1,600 characters with a visible counter |

An unread message badge appears on the message button when the patient has replied and the message has not been read yet.

---

### Phone / VoIP (Call)

Opens a call interface integrated directly with the GoTo Phone system.

| Feature | Detail |
|---------|--------|
| GoTo Integration | Direct dial through your practice's phone system |
| Call History | Full log of previous call attempts |
| Call Notes | Mandatory notes field (150-character limit) after each call |

For Problem Claims, the call button opens a dropdown to choose between calling the patient/guarantor or calling the insurance company directly.

---

### Task Override

Removes a task from the active list. You must select a reason. Available reasons include:

| Reason | What Happens |
|--------|-------------|
| In Person | Patient came in to resolve the issue |
| Mailed | Triggers a balance-due letter via USPS |
| Collections | Flags the patient for collections |
| Write Off | Writes the balance off the ledger in the PMS |
| Snooze | Temporarily hides the task for a specified number of days (up to 30) |

---

### Task Reassign

Escalates a task or routes it to the USPS Mailer Queue. When reassigning, the team member must select the appropriate communication template before confirming.

| Level | Can Reassign To |
|-------|----------------|
| L1 | L2 or Mailer Queue |
| L2 | L3, back to L1, or Mailer Queue |
| L3 | Back to L1 or Mailer Queue |
| Mailer Queue | Triggers automated USPS mail request |

---

### Resubmit (Problem Claims only)

Available only in the **Problem Claims** view. Opens a workflow to resubmit an insurance claim that has been flagged for an issue.

---

## Patient Search

A real-time patient name search is available in:
- The **top navigation bar** — searches across the entire platform
- The **Patient column** in any table — filters results within that specific view

## Message Notification

Unread message badges appear directly on the message button in each patient row. When you have unread messages across all patients, a notification indicator appears in the top navigation.

---

---

---

---

# Opalescence — Scoring & Gamification

## What is Opalescence?

Opalescence is OPAL gOS's built-in scoring system. It assigns points to tasks based on their urgency and financial impact, helping your team prioritize the right work at the right time.

## How Scores Are Calculated

Each task is assigned an OPALescence score using OPAL's proprietary formula. Factors include:

- Age of the task
- Uncollected balance amount
- How quickly the task is addressed
- Number of contact attempts made
- Number of times the task has been reassigned
- Daily streaks and milestone achievements

Higher scores = higher priority. A task with a high OPALescence score has greater operational or financial impact and should be addressed first.

## Where You See It

- **Every patient row** in Collect, Produce, and Schedule tables shows the task's OPALescence score
- **Home screen** shows your cumulative personal score and team comparisons

## Home Screen Metrics

| Metric | Description |
|--------|-------------|
| OPALescence Points | Your total points earned from all completed tasks |
| Current Streak | Consecutive days you've earned points — also shows your all-time best streak |
| Month-to-Date (MTD) Trend | Cumulative OPALescence score for the current month |

## Leaderboards

| Leaderboard | Scope |
|-------------|-------|
| Practice Leaderboard | Rankings within your practice (top 3 shown on home screen) |
| Global Leaderboard | Rankings across all gOS users (top 3 shown on home screen) |

Leaderboards update in real time as tasks are completed. They encourage consistent daily engagement and highlight top performers across the team.

## OPAL Rush

Displayed on the Home screen. Surfaces your practice's highest-value opportunities in real time — the top patients with the greatest impact if addressed today. Up to 3 patients are shown.

---

---

---

---

# Settings

Settings are accessible via the gear icon in the top navigation bar. Visibility of each tab depends on your user role.

| Settings Tab | Minimum Role Required |
|-------------|----------------------|
| General | L3 |
| Users | L2 |
| Schedule | L3 |
| Produce | L3 |
| Collect | L3 |
| Quick Text | L3 |

---

## Practice Selector (L3+)

Allows L3 users to manage multiple practices from a single login:

- View all practices you are authorized to manage
- Switch between practices without logging out
- Access practice-specific data, workflows, and metrics

The currently active practice is always visible in the selector. You can also search across practices by name.

---

## A. General Settings

Controls core system behaviors for automation, escalation, and task engagement.

### Auto-Escalation Settings

| Setting | Description |
|---------|-------------|
| Maximum actions before auto-escalation | How many automated outreach attempts gOS makes before escalating to manual follow-up |
| Refresh time between actions | Minimum time between automated actions to prevent over-contacting patients |
| Maximum idle time before escalation | How long a task can stay inactive before being auto-escalated, even if the action limit hasn't been reached |

### Task Management Settings

| Setting | Description |
|---------|-------------|
| Daily task requirement | Number of tasks a user must complete per day to maintain their activity streak |

This setting directly affects streak-based engagement and OPALescence milestone tracking.

---

## B. User Settings

The User Management section is where authorized users (L2+) create, update, and maintain user accounts.

- Search users by name
- Filter users by role (L1, L2, L3, L4)
- Create new users with role assignment
- Edit existing users — update role, name, or practice associations
- Associate users with one or multiple practices
- Deactivate users when they leave

Role indicators are displayed directly in the user table.

---

## C. Schedule Settings

Configures the automated outreach workflow for each Schedule problem type. Select a problem type from the dropdown to view and edit its step configuration.

**Problem types available:**
- No Reappointments
- No Shows
- Reactivations
- Overdue Appts (supports per-disposition configuration — select a disposition after choosing this type)

For each problem type, you can configure the outreach timeline — which channel (SMS, Email, Mail, Call) is used at each step, and how many days after the trigger each step fires.

---

## D. Produce Settings

Configures the automated outreach workflow for each Produce problem type. Select a problem type from the dropdown to view and edit its step configuration.

Standard problem types are provided by default. You can also **create custom problem types** — up to the configured maximum — with their own name, description, procedure lookups, and outreach steps. Custom types can be edited or deleted from the same dropdown.

For problem types that support it, a **Procedure Lookup** selector appears to filter the configuration to a specific procedure category.

---

## E. Collect Settings

Configures how gOS manages patient balance follow-up communications. Defines when and through which channel patients are contacted as their balance ages.

Supported outreach channels and their configuration:

| Channel | Description |
|---------|-------------|
| Message (SMS) | Text message templates triggered at configured day thresholds |
| Call | Phone script steps triggered at configured day thresholds |
| Email | Email templates triggered at configured day thresholds |
| Mail | USPS mail templates triggered at later-stage balance age thresholds |

Each step in the timeline specifies the channel, the number of days after the trigger, and the message template. Steps are ordered automatically based on their day thresholds.

---

## F. Quick Text

Manage reusable text snippets that agents can insert when replying to patient messages in the Message Inbox.

- Search quick texts by name
- Add new quick text with a name and body
- Edit or delete existing entries
- List loads incrementally — scroll to load more

Quick texts are available to all users when composing a message reply.

---

## L4 User — Collections Queue

L4 users do not have access to Settings. Instead, their home screen opens directly to the **Collections Queue** — a list of accounts that have completed all outreach and escalation steps.

From the Collections Queue, L4 users can:

| Action | Description |
|--------|-------------|
| Write Off | Check the Write Off box to mark an account as written off — a confirmation dialog appears before finalizing |
| Download CSV | Export the full queue to a CSV file with patient details, addresses, balances, SSN, and chart numbers for external collections submission |

The Collections Queue is also accessible from **Relay > Write off**.