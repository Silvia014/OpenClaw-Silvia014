---
name: smart-calendar
description: Turn natural-language scheduling requests into clear Google Calendar events using the user's existing calendar connection. Use when the user wants to schedule, book, block, or reserve time on their calendar.
---

# Smart Calendar Events

## Purpose

Make calendar scheduling easier by allowing the user to describe an event naturally instead of providing technical calendar fields.

## Input

The user can provide a natural-language request such as:

"Study Next.js Thursday afternoon for two hours."

Extract:

- event title;
- date;
- start time;
- duration or end time;
- timezone;
- any additional useful context.

Use `USER.md`, `SOUL.md`, `AGENTS.md`, and `TOOLS.md` for user-specific context and preferences.

## Scheduling Rules

- Use `Europe/Madrid` as the default timezone unless the user specifies another timezone.
- If the user gives a duration, calculate the end time.
- If the user gives an end time, use it directly.
- If the user gives an ambiguous time such as "afternoon", choose a reasonable time or ask when the exact time materially matters.
- Check existing calendar information when available before creating an event.
- Avoid creating duplicate events.
- Do not modify or replace the existing Google Calendar authentication.

## Execution

Use the existing Google Calendar connection available to OpenClaw.

Do not modify:

- OAuth credentials;
- access tokens;
- existing authentication configuration;
- existing Google Calendar integration scripts.

## Confirmation

After successful creation, report:

- event title;
- date;
- start time;
- end time;
- timezone;
- event link when available.

Never claim that an event was created unless the calendar operation was successfully verified.

## Safety

Creating a calendar event is an external action.

When confirmation is required by the connected calendar tool, obtain confirmation before performing the write operation.

Never delete or modify existing events as part of this skill unless explicitly requested.

## Example

User:

"Schedule two hours of Next.js study Thursday afternoon."

Expected behavior:

1. Interpret the request.
2. Determine the appropriate Thursday date.
3. Choose an appropriate afternoon start time if no exact time is given.
4. Calculate the two-hour end time.
5. Create the event using the existing Calendar connection.
6. Return a concise confirmation.
