---
name: meeting-notes
description: Turn raw meeting notes into a structured summary and save the result as a Google Doc using the user's existing Google Docs connection.
---

# Meeting Notes to Google Docs

## Purpose

Turn unstructured meeting notes into a useful document that can be reviewed and shared later.

## Input

The user provides raw notes in natural language.

The notes may contain:

- discussion points;
- decisions;
- action items;
- questions;
- deadlines;
- participants;
- follow-up information.

Use `USER.md`, `SOUL.md`, `AGENTS.md`, and `TOOLS.md` for the user's context and preferred working style.

## Processing

Organize the notes into:

1. Meeting title
2. Date
3. Summary
4. Decisions
5. Action Items
6. Open Questions
7. Next Steps

Do not invent information that was not present in the original notes.

If information is missing, omit the section or clearly mark it as unavailable.

## Google Docs

Use the existing Google Docs connection available to OpenClaw.

Do not modify:

- OAuth credentials;
- access tokens;
- existing authentication configuration;
- existing Google Docs integration scripts.

Create a new document containing the structured meeting notes.

## Output

After successful creation, report:

- document title;
- a short summary of what was recorded;
- the Google Docs link when available.

Never claim that the document was created unless the operation was successfully verified.

## Quality Rules

The final document should be:

- concise;
- organized;
- easy to scan;
- faithful to the original notes;
- focused on decisions and actions.

Do not add fictional participants, deadlines, decisions, or action items.

## Example

User:

"Today's meeting was about the website launch. Silvia will finish the homepage tomorrow. We decided to launch Friday. We still need to confirm the final images."

Expected document:

### Summary

The meeting focused on the website launch.

### Decisions

- The website launch is planned for Friday.

### Action Items

- Silvia will finish the homepage tomorrow.

### Open Questions

- Final images still need to be confirmed.

### Next Steps

- Confirm the final images.
- Complete the homepage.

