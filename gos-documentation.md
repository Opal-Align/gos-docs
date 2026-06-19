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
| L2 | Senior Staff | Can escalate and reassign tasks |
| L3 | Practice Manager | Manages multiple practices, access to Settings |
| L4 | Revenue Cycle Manager | Highest authority, manages Collections Queue |

## Support

- **In-app chatbot:** gEMMAi — available at the bottom right of every screen
- **Email support:** Support@OpalAlign.com

---

# Relay

## Overview

Relay is your team's communication hub. It centralizes all patient messaging activity in one place so nothing falls through the cracks.

## Subtabs

### Message Inbox

Real-time SMS inbox for two-way patient conversations. Reply directly to patient messages from this view.

### Pending Outreach

Lists patients who are next in line to receive an automated outreach message. Shows what message they will receive and when.

### Contact History

A log of all patients who have already been contacted, showing when they were reached and at which step in the outreach lifecycle.

### Mail Queue

Lists patients scheduled to receive a physical mailed letter from your practice. Shows the template selected and the expected send date.

### Missing Contacts

Patients without a valid phone number or email address appear here. These patients cannot be reached through automated outreach until their contact information is updated in your Practice Management System (PMS).

---

# Schedule

## Overview

The Schedule screen gives your team a real-time view of today's patients and tools to verify upcoming insurance eligibility. It is designed to help you prepare for each patient encounter and resolve issues before the appointment.

## Subtabs

### Today

Displays all patients scheduled for today along with any outstanding issues that need attention before or during their appointment. Use this view to proactively identify:

- Outstanding balances
- Missing demographic information
- Insurance or payer-related errors

Resolving these before the patient arrives ensures a smoother experience for both staff and patients.

### Insurance Eligibility

Lists upcoming patients whose insurance needs to be verified for future appointments. Patients in this view typically have appointments scheduled for tomorrow or later.

The system flags any gaps or errors that must be addressed in advance to prevent eligibility-related claim denials or day-of delays.

---

## Patient Slip (Verification of Benefits)

The Patient Slip is a comprehensive, auto-generated document accessible by clicking on any patient's name in the Schedule screen. It consolidates all critical information into a single view.

### Patient Information
Essential demographic and contact details.

### Opal Alerts
System-generated flags for outstanding tasks, missing information, or account issues that require staff attention.

### Family Members
Linked household members for cross-referenced insurance, combined billing, or appointment coordination.

### Guarantor Information
The responsible party for the patient's financial obligations.

### Billing Information
The patient's current financial standing with the practice:

| Field | Description |
|-------|-------------|
| Last Statement Date & Amount | Most recent statement sent |
| Last Payment Date & Amount | Most recent payment received |
| Last Payer Paid Date & Amount | Most recent insurance payment |
| Current Balance | Total outstanding balance |
| Aging Buckets | >30, >60, >90, >120 days |
| Est PT Bal | Estimated patient portion |
| Est INS Bal | Estimated insurance portion |

### Appointment Procedure Detail
Procedures associated with the patient's current appointment.

### Treatment Plan
Any planned future treatments on record.

### Insurance Information

| Field | Description |
|-------|-------------|
| Insurance Name & Plan Name | Active insurance plan |
| Group Name & Number | Group identifier |
| Payer ID | Insurance payer identifier |
| Insurance Address & Phone | Payer contact details |
| Fee Schedule | Associated fee schedule |
| Effective Dates | Coverage start and end dates |

### Coverage Summary

| Field | Description |
|-------|-------------|
| Yearly Max | Annual maximum benefit |
| Deductibles | Individual and family deductible amounts |
| Deductible applies to preventive/diagnostic | Yes or No |
| Waiting Periods | Any applicable waiting periods |
| Missing Tooth Clause | Whether the plan excludes pre-existing missing teeth |
| Coordination of Benefits | Rules for patients with multiple insurance plans |

### General Benefit Details
Coverage breakdown by procedure category including code, description, frequency limits, coverage percentages, age limits, and historical usage.

### Specialty Benefit Details
Benefits for specialized services:
- Endodontics
- Periodontics
- Oral Surgery
- Orthodontics

---

# Produce

## Overview

Produce is designed to proactively generate appointments through automated patient outreach. The system handles the first three contact attempts automatically. Patients only surface in the Produce tables after automation has been exhausted and manual follow-up is required.

## How Automation Works

When a patient matches one of the Produce categories, gOS automatically sends up to three SMS messages over a defined period requesting that the patient schedule an appointment.

- If the patient schedules during the automated sequence → no further action needed, they do not appear in the table
- If the patient does not schedule after three messages → they escalate to the Produce table for manual follow-up

## Patient Categories

### Broken Appointments
Patients who missed or canceled an appointment and have not yet been rescheduled.

### Overdue Appointments
Patients who are past their recommended recall or follow-up window.

### Unscheduled Treatment
Patients with diagnosed treatment on record that has not been scheduled.

### Declined Treatment
Patients who previously declined recommended treatment and may be eligible for re-engagement.

### Reappointments
Patients who require a future appointment based on prior visits or treatment plans.

---

Each category allows your team to prioritize outreach based on the practice's operational goals. Higher Opalescence scores indicate higher-priority patients within each category.

---

# Collect

## Overview

Collect organizes outstanding patient balances into focused views so your team can efficiently identify, prioritize, and follow up on revenue. Navigate between views using the tabs at the top of the screen.

## Views

### Missed Collections
Patients who had an appointment yesterday and left with an unpaid balance. These are high-priority — timely outreach significantly increases the likelihood of successful collection.

### A/R - with Appt.
Patients who have an upcoming appointment and an outstanding balance. An ideal opportunity to resolve the balance before or during their scheduled visit.

### A/R - without Appt.
Patients who owe a balance but have no future appointment scheduled. Requires proactive outreach to resolve the balance and, when appropriate, schedule continued care.

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

### Missed Collections

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
| Patient | Searchable — includes a button to open the EOB document |
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

Every patient row across Collect, Produce, and Schedule includes a set of action buttons that guide your team through the correct workflow. These buttons ensure consistent, compliant, and effective outreach.

## Action Buttons

### SMS / Text

Opens a fully functional two-way chat interface with the patient.

| Feature | Detail |
|---------|--------|
| Message Templates | Preloaded templates organized by tonality |
| Text-to-Pay | Embedded payment link for easy patient payment |
| 3rd Party Financing | Embedded financing link |
| Real-time Updates | Messages sync instantly — both directions |
| Message History | Infinite scroll through full conversation history |
| Character Limit | 1,600 characters with a visible counter |

### Phone / VoIP

Opens a call interface integrated directly with the GoTo Phone system.

| Feature | Detail |
|---------|--------|
| GoTo Integration | Direct dial through your practice's phone system |
| Call History | Full log of previous call attempts |
| Call Notes | Mandatory notes field (150-character limit) after each call |

### Task Override

Removes a task from the active list. Select the reason that applies:

| Reason | What Happens |
|--------|-------------|
| In Person | Patient came in to resolve the balance |
| Mailed | Triggers a balance-due letter and statement via USPS |
| Collections | Flags the patient for collections |
| Write Off | Writes the balance off the patient ledger in the PMS (e.g., Dentrix) |

### Task Reassign

Escalates a task or routes it to the USPS Mailer Queue.

| Level | Can Reassign To |
|-------|----------------|
| L1 | L2 or Mailer Queue |
| L2 | L3, back to L1, or Mailer Queue |
| L3 | Back to L1 or Mailer Queue |
| Mailer Queue | Triggers automated USPS mail request |

When reassigning, the team member must select the correct communication template before confirming.

---

## Patient Search

A real-time patient name search is available from:
- The **Home / Relay** screen
- The **Patient** column in the Collect screen

## Message Notification Center

Located in the top-right corner of the application. Shows a count of all unread patient messages.

- Clicking the notification icon opens the Notification Center overlay
- Each entry shows the patient name and time of the most recent message
- Clicking **View** navigates directly to the patient's row on the relevant screen — no manual searching required

---

# Opalescence — Scoring & Gamification

## What is Opalescence?

Opalescence is OPAL gOS's built-in scoring system. It assigns points to tasks based on their urgency and financial impact, helping your team prioritize the right work at the right time.

## How Scores Are Calculated

Each task is assigned an Opalescence score using OPAL's proprietary formula. Factors include:

- Age of the task
- Uncollected balance amount
- How quickly the task is addressed
- Number of contact attempts made
- Number of times the task has been reassigned
- Daily streaks and milestone achievements

Higher scores = higher priority. A task with a high Opalescence score has greater operational or financial impact and should be addressed first.

## Where You See It

- **Every patient row** in Collect, Produce, and Schedule tables shows the task's Opalescence score
- **Home screen** shows your cumulative personal score

## Home Screen Metrics

| Metric | Description |
|--------|-------------|
| Opalescence Score | Total points earned from all completed tasks |
| Current Streak | Consecutive days you've earned points |
| Month-to-Date Opalescence | Cumulative score for the current month |
| Weekly Snapshot | Visual overview of your daily point totals for the week |

## Leaderboards

| Leaderboard | Scope |
|-------------|-------|
| Practice Leaderboard | Rankings within your practice |
| Global Leaderboard | Rankings across all gOS users |

Leaderboards update in real time as tasks are completed. They encourage consistent daily engagement and highlight top performers across the team.

## OPAL Rush

Displayed on the Home screen. Surfaces your practice's highest-value opportunities in real time — the tasks that will earn the most points and have the greatest impact if addressed today.

---

# Settings

Settings are available to L3 and L4 users. The Settings icon is located to the right of the Practice Selector in the top navigation.

---

## Practice Selector (L3+)

Allows L3 users to manage multiple practices from a single login:

- View all practices you are authorized to manage
- Switch between practices without logging out
- Access practice-specific data, workflows, and metrics

The currently active practice is always visible in the selector.

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

This setting directly affects streak-based engagement and Opalescence milestone tracking.

---

## B. User Settings

The User Management section is where authorized users create, update, and maintain user accounts.

- Assign roles (L1–L4) to control access and visibility
- Associate users with one or multiple practices
- Role indicators are displayed directly in the user table

---

## C. Collect Settings

Configures how gOS manages patient balance follow-up communications. Defines when and through which channel patients are contacted as their balance ages.

### SMS Templates
- Up to **6 templates** configurable
- Each template is triggered when a balance crosses a configured age threshold
- Current day thresholds are shown clearly in the interface

### Phone Call Thresholds
- Up to **3 call attempt thresholds** configurable
- The first call attempt triggers the automation workflow
- Each threshold defines when a call should occur relative to task age

### Email Templates
- Up to **6 templates** configurable
- Each triggered at a defined age milestone
- Provides a more detailed communication option for aging balances

### Mail Templates
- Up to **2 templates** configurable
- Reserved for later-stage collection efforts
- Triggered at later balance age thresholds

### Template Configuration
Administrators can manage the content of templates for each channel (SMS, Phone, Email, Mail) from the Template Configuration section within Collect Settings.

---

## L4 User Workflow — Collections Queue

L4 users have exclusive access to the Collections Queue, which contains accounts that have completed all outreach and escalation steps.

From the Collections Queue, L4 users can:

| Action | Description |
|--------|-------------|
| Send to Collections | Authorize the account for external collections |
| Address Directly | Personally engage with the patient to resolve the balance, apply adjustments, or determine an alternative resolution |
