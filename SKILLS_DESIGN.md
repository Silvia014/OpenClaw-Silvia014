# SKILLS_DESIGN.md

## Skill 1 — Smart Calendar Events

### 1. What does this skill do?

The skill converts natural-language scheduling requests into structured Google Calendar events. It automatically determines the event title, date, start time, duration, and timezone from the user's request and available context.

### 2. What input does the agent need?

The user can describe an event naturally, for example:

"Study Next.js on Thursday afternoon for two hours."

The agent uses the user's timezone, preferences, calendar context, and information from `USER.md`, `SOUL.md`, `AGENTS.md`, and `TOOLS.md`.

The existing Google Calendar connection is used to perform the calendar operation. The skill must not modify the existing Google Calendar authentication or connection.

### 3. What does a good output look like?

A successful output is a Google Calendar event containing:

- a clear title;
- the correct date;
- the correct start time;
- the requested duration;
- the appropriate timezone.

The skill should avoid creating duplicate or conflicting events when calendar information is available.

The user should receive a concise confirmation containing the event details and, when available, a link to the created event.

---

## Skill 2 — Meeting Notes to Google Docs

### 1. What does this skill do?

The skill converts raw meeting notes into a structured and useful summary and saves the result as a Google Doc.

### 2. What input does the agent need?

The user provides raw meeting notes in natural language.

The notes may contain:

- discussion points;
- decisions;
- tasks;
- questions;
- deadlines;
- participants;
- follow-up information.

The agent uses the user's context and working preferences from `USER.md`, `SOUL.md`, `AGENTS.md`, and `TOOLS.md`.

The existing Google Docs connection is used to create the document. The skill must not modify the existing Google Docs authentication or connection.

### 3. What does a good output look like?

A successful output is a structured Google Doc containing:

- meeting title and date;
- summary;
- decisions;
- action items;
- open questions;
- next steps.

The document should be concise, organized, and easy to review later.

The user should receive confirmation that the document was created and, when available, a link to the document.