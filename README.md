# Leave Request and Approval System

A leave management solution built on the Microsoft Power Platform. Employees submit leave requests in a canvas app, approvers review them in two steps, and approved leave automatically updates the employee's balance and calendar.

## Features
- Submit leave requests (Annual, Sick, etc.) from a canvas app
- Two-step approval: Pending Manager → Pending HR → Approved
- Automatic update of the **Leave Balance** (used and remaining days) when leave is approved
- Automatic **Appointment** (calendar) entry for approved leave
- AI Builder category classification of the leave reason
- Power BI report on leave requests and balances

## Tech Stack
- **Microsoft Dataverse**: tables for Leave Request, Leave Balance and Appointment
- **Power Apps (Canvas)**: the Leave App
- **Power Automate**: cloud flows for approval updates and AI tagging
- **AI Builder**: category classification model
- **Power BI**: reporting

## Repository Contents
| File | Description |
|------|-------------|
| `LeaveManagement_1_0_0_1.zip` | Unmanaged Power Platform solution (app, flows, tables, AI model) |
| `Leave Management Report.pbix` | Power BI report |
| `Leave Request & Approval – Project Write-up.pdf` | Detailed write-up, including the demo video link |

## Demo Video
The demo video link is included in the project write-up PDF.

## How to Import the Solution
1. Go to [make.powerapps.com](https://make.powerapps.com) and select your environment.
2. Open **Solutions → Import solution** and upload `LeaveManagement_1_0_0_1.zip`.
3. Set up the connections requested during import (Dataverse and others).
4. After the import, open the solution and turn on the cloud flows.

**Requirements:** The environment needs AI Builder, because the solution depends on Microsoft's *AI Solution default templates*. The Power BI report needs Power BI Desktop to open.

## Author
Niya Benny
