# IT Operations – Command Center Reference
*Last Updated: May 26, 2026*

---

## 👤 Director
**Ezra** – Director of IT Operations

---

## 👥 Teams

### Infrastructure Operations
Kyle, Reema, Maurice, Isaac, Ezra, Imran, Daniel

### Windows Team
Joe, Taylor, Eric

### Linux Team
Wasim, Julian, Venkat, Lonnie

---

## 🗂️ Notion Workspace Structure

**Primary Tool:** Notion (free plan)
**Workspace:** Ezra McClendon's Workspace
**Top-Level Page:** 🖥️ IT Operations
**IT Operations Page ID:** 36c27749-5702-81be-8aad-ed521db72fcb

| Section | Database |
|---------|----------|
| 📋 All Active Projects | Combined — all 3 teams |
| 🎫 All Tickets & Changes | Combined — all 3 teams |
| 🏖️ PTO Tracker | Shared — all 12 members |
| ✅ To Do List | Ezra's personal tasks |
| 📁 Document Library | SOPs, Runbooks, Policies, References, Templates |
| 📊 IT Ops Dashboard | Linked views of all databases |

### Key Data Source IDs
| Database | Data Source ID |
|----------|---------------|
| All Active Projects | 3f9cf6dd-c7fa-4549-9395-d9e6ae71907e |
| All Active Projects (URL ID) | 16178ce8063f4ff7bb0b9861bed7cac3 |
| All Tickets & Changes | 188eb34d-d88a-4488-a053-7f0761ef7b7a |
| PTO Tracker | 75e2ac81-f902-4691-b37e-048183e9944f |
| To Do List | 9b9f85a5-34ab-446c-bba0-0e82b3632b2c |
| Document Library | 1494bb36-7e8a-4f1a-b64c-6562dbc54fdc |

### Database Fields
**All Active Projects:** Name, Team, Team Member, Status, Priority, Due Date, Notes
**All Tickets & Changes:** Name, Team, Team Member, Type (Ticket/Change), Status, Priority, Due Date, Notes
**PTO Tracker:** Name, Team Member, Team, Start Date, End Date, Notes
**To Do List:** Task, Status, Priority, Due Date, Notes
**Document Library:** Document Name, Category (Runbook/SOP/Policy/Reference/Template/Other), Team, Last Updated, Notes

### Team Member Dropdowns (All databases)
- **Infrastructure Operations:** Kyle, Reema, Maurice, Isaac, Ezra, Imran, Daniel
- **Windows Team:** Joe, Taylor, Eric
- **Linux Team:** Wasim, Julian, Venkat, Lonnie

---

## 📊 IT Ops Dashboard

**URL:** https://www.notion.so/36c27749570281a388e5f75526db1d82

Contains 3 live views (auto-filtered, real-time, flat list — no empty team sections):
- 📋 **All Open Projects** — Status ≠ Completed, sorted by Team then Due Date
- 🎫 **All Open Tickets & Changes** — Status ≠ Resolved/Closed, sorted by Team then Priority
- 🏖️ **Open PTO** — sorted by Start Date

---

## 🏖️ PTO Tracker

**Data Source ID:** 75e2ac81-f902-4691-b37e-048183e9944f

### Naming Convention
```
PTO – [First Name] | [Month Day–Day]
```
**Due Date:** Set to the **first day** of PTO

### Current PTO Entries
| Name | Team | Start | End |
|------|------|-------|-----|
| Maurice | Infrastructure Operations | May 28, 2026 | May 28, 2026 |
| Eric | Windows Team | May 26, 2026 | Jun 3, 2026 |
| Taylor | Windows Team | Jun 1, 2026 | Jun 2, 2026 |
| Venkat | Linux Team | Jun 1, 2026 | Jun 5, 2026 |
| Eric | Windows Team | Jun 8, 2026 | Jun 11, 2026 |
| Reema | Infrastructure Operations | Jun 25, 2026 | Jun 29, 2026 |
| Taylor | Windows Team | Jun 29, 2026 | Jul 6, 2026 |
| Joe | Windows Team | Jul 6, 2026 | Jul 17, 2026 |
| Reema | Infrastructure Operations | Jul 22, 2026 | Jul 27, 2026 |

---

## ✅ To Do List

**Data Source ID:** 9b9f85a5-34ab-446c-bba0-0e82b3632b2c

### Current Items
| Task | Status | Priority | Due Date |
|------|--------|----------|----------|
| Confirm if Agent 2 is working in SkippyAI | Not Started | Normal | — |

---

## 📋 Active Projects

| Project | Team Member | Team | Due Date | Status |
|---------|-------------|------|----------|--------|
| Deploy Skippy AI Servers in Prod Tenant | Kyle | Infrastructure Operations | May 29, 2026 | Not Started |
| Install DevOps Servers in Prod Tenant | Reema | Infrastructure Operations | May 29, 2026 | Not Started |

---

## 🎫 Open Tickets & Changes

| Ticket | Team Member | Team | Type | Status |
|--------|-------------|------|------|--------|
| RITM0021267 – Align Skippy Test Environment to Prod Standards | Ezra | Infrastructure Operations | Ticket | Open |

---

## 📅 Calendar Setup

**Primary Calendar:** EzraMcC
**Calendar ID:** E7B236E6-CB1E-4DB0-B4B7-ED3C58D51FDA

> All events created by Claude go into EzraMcC.

### Recurring Events
| Event | Schedule | Notes |
|-------|----------|-------|
| 🏖️ Weekly PTO Check – Who's Out This Week? | Every Monday at 8:00 AM | Check Notion PTO Tracker |

---

## 🔗 Tools & Integrations

| Tool | Status | Purpose |
|------|--------|---------|
| Notion | ✅ Connected | Projects, Tickets, PTO, To Do tracking |
| GitHub | ✅ Connected | Hosts this .md file |
| EzraMcC Calendar | ✅ Active | All calendar events |
| Make (Integromat) | ✅ Active | Daily email digest |

**GitHub Repo:** [github.com/webguru-emcc/ITOpsProjects](https://github.com/webguru-emcc/ITOpsProjects)

### Make Scenario (Daily Email Digest)
**Flow:** Schedule → Notion (Search All Active Projects) → Text Aggregator → Gmail

- Queries All Active Projects for non-completed items
- Text Aggregator consolidates results into single trigger (prevents duplicate emails)
- Sends one daily email to ezramcc@gmail.com with link to Notion dashboard
- Notion URL ID used in Make: `16178ce8063f4ff7bb0b9861bed7cac3`
- Filter: Status (Select) does not equal Completed
- **Make IT Ops** integration must be connected to all Notion databases

---

## 🔄 How to Resume Context in a New Chat

If you ever need to start a new chat, paste this entire .md file at the top of the conversation and say:

> *"You are Ezra, Director of IT Operations. Here is our reference doc — pick up where we left off."*

**What persists without the .md (saved to Claude memory):**
- EzraMcC calendar preference
- Team rosters and structure
- Notion workspace IDs and data source IDs
- GitHub repo and dashboard URL
- PTO naming convention

**What requires the .md to restore:**
- Full database field details
- Active project and ticket list
- Make scenario details
- Pending to-dos

---

## 🔧 Notes & Conventions

- Use this chat as the ongoing IT Ops command center
- Notion is the primary tracking tool — team members tracked via dropdown (no accounts needed)
- Always set Team AND Team Member fields when creating projects/tickets so dashboard works correctly
- GitHub token: stored privately — do not commit to repo. Paste into chat when needed.
- Voice input: use device dictation (iOS mic on keyboard, Mac Dictation) to speak into this chat
