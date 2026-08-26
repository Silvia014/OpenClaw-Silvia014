# SKILLS_DESIGN.md

## Skill 1 — GitHub Daily Brief

### 1. What does this skill do?

The skill checks recent activity in my GitHub repositories and creates a short summary of relevant commits, issues, and pull requests. The summary is sent to me through Telegram.

### 2. What input does the agent need?

The agent needs to know which repositories to check and, when specified, the period of activity to analyze. If no period is provided, it should use recent activity.

The agent gets my personal context, projects, and preferences from `USER.md`, and behavioral rules from `SOUL.md` and `AGENTS.md`.

GitHub information and Telegram delivery are handled through the available Zapier connections.

### 3. What does a good output look like?

A good output is a short, structured Telegram message containing:

- relevant recent commits;
- important open or updated issues;
- relevant pull requests;
- possible blockers or actions requiring attention.

The most important actions should appear first.

The skill is successful when a relevant and up-to-date GitHub summary is delivered to Telegram.

---

## Skill 2 — Tasks to Calendar

### 1. What does this skill do?

The skill reviews pending Google Tasks and creates focused work blocks in Google Calendar for tasks that require dedicated time.

### 2. What input does the agent need?

The agent needs access to pending tasks and, when available, their priority, deadline, estimated duration, and context.

When the user provides additional constraints such as a specific date, available time, or duration, these should be used to determine when the task should be scheduled.

Personal context, projects, and preferences come from `USER.md`, while behavioral rules come from `SOUL.md` and `AGENTS.md`.

Google Tasks and Google Calendar are connected through Zapier.

### 3. What does a good output look like?

A good output consists of focused work blocks created in Google Calendar for the selected tasks.

Each block should contain:

- a clear task title;
- date and time;
- an appropriate duration;
- relevant context in the description when necessary.

The skill should avoid creating duplicate events and should respect existing calendar events.

The skill is successful when the selected tasks are correctly represented as work blocks in Google Calendar.