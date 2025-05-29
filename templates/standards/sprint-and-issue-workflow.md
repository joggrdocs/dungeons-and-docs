# 🎟️ Sprint & Issue Workflow

This guide outlines how we manage sprints, issues, and workflows using a ticketing system like Linear or Jira.

---

## 🧱 Ticket Lifecycle Overview

Every issue flows through these standard stages:

- **Backlog** – Created, unprioritized
- **To Do** – Prioritized and ready to work
- **In Progress** – Actively being worked on
- **In Review** – Awaiting code review or QA
- **Done** – Completed, deployed, and verified
- **Won’t Do** – Closed without action

---

## 🌀 Sprint Structure

- **Sprint Duration**: 2 weeks (Monday to Friday)
- **Sprint Goal**: Defined during planning
- **Capacity Planning**: Based on team availability
- **Scope Commitment**: Only "Ready" issues are pulled into the sprint

---

## 🧾 Issue Types

| Type     | Description                     |
|----------|---------------------------------|
| Story    | User-facing features            |
| Bug      | Defects or regressions          |
| Task     | Technical/internal work         |
| Spike    | Research or exploratory work    |
| Chore    | Maintenance and cleanup         |

---

## ✏️ Creating a Ticket

- Anyone can create tickets
- Use clear, concise titles and descriptions
- Add relevant labels or components
- Include "Definition of Done" or acceptance criteria if needed

---

## 🧹 Backlog Refinement

Occurs regularly (e.g., once a week):

- Clarify unclear requirements
- Estimate effort (story points or T-shirt sizing)
- Identify dependencies and blockers
- Prioritize with the Product Owner

---

## 📦 Sprint Planning

Held at the start of each sprint:

- Select issues from the top of the **Ready** list
- Align with the sprint goal and team capacity
- Assign owners or pairs
- Confirm that issues meet the team's "Ready for Dev" criteria

---

## 🔧 Working on Issues

Once in **In Progress**:

- Link branches or pull requests to the ticket
- Post comments for blockers, updates, or decisions
- Update status as you progress
- Move to **In Review** when the PR is ready

---

## 🧪 Review & QA

- Peer reviews are required for all code changes
- QA is done manually or via automated pipelines as needed
- Review feedback should be constructive and timely
- Only move to **Done** when all criteria are met

---

## ✅ Completing the Issue

Mark an issue as **Done** when:

- All acceptance criteria are satisfied
- Code is reviewed and merged
- Deployed to the appropriate environment
- A summary or outcome is noted in comments

---

## 📊 Metrics We Track

- Cycle time per issue
- Team velocity (story points per sprint)
- Time in each workflow stage
- Bug frequency and resolution time

---

## 📌 Best Practices

- Keep issues small and clearly scoped
- Regularly groom and prioritize the backlog
- Use clear commit messages and documentation
- Communicate openly in tickets (no silent work)
- Avoid “In Progress” overload – limit WIP

---

_“The board is our shared source of truth — keep it tidy, current, and actionable.”_
