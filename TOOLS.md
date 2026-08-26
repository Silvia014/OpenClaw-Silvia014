# TOOLS.md - Local Notes

Skills define _how_ tools work. This file is for _your_ specifics — the stuff that's unique to your setup: camera names and locations, SSH hosts and aliases, preferred TTS voices, speaker/room names, device nicknames, anything environment-specific.

## Examples

```markdown
### Cameras

- living-room → Main area, 180° wide angle
- front-door → Entrance, motion-triggered

### SSH

- home-server → 192.168.1.100, user: admin

### TTS

- Preferred voice: "Nova" (warm, slightly British)
- Default speaker: Kitchen HomePod
```

## Why Separate?

Skills are shared. Your setup is yours. Keeping them apart means you can update skills without losing your notes, and share skills without leaking your infrastructure.

---

Add whatever helps you do your job. This is your cheat sheet.

## Automation Platform

The external service integrations for this workspace use Zapier.

Do not assume Composio is the integration platform for this workspace.

## Google Calendar

Use Google Calendar for:

- appointments;
- meetings;
- study sessions;
- work blocks;
- reminders and scheduled activities.

Default timezone: `Europe/Madrid`

Before creating an event:

- check for relevant existing events;
- avoid duplicate events;
- respect existing commitments;
- use the requested duration when provided.

## Google Docs

Use Google Docs when the user asks to create, read, or update structured documents.

Prefer clear titles and organized sections.

## Gmail

Use Gmail for reading, drafting, organizing, and sending emails.

Before sending an email externally, verify the recipient, subject, content, and intended action.

## Google Drive

Use Google Drive to find, organize, and manage project documents.

Do not delete or move files unless the requested action is clear.

## Google Tasks

Use Google Tasks for actionable items.

When creating tasks, use concise titles and useful descriptions.

When turning tasks into Calendar blocks, check for existing equivalent events first.

## GitHub

The main OpenClaw repository is:

`Silvia014/OpenClaw-Silvia014`

Before repository modifications:

1. Check the current branch.
2. Run `git status`.
3. Inspect the relevant files.
4. Make the smallest appropriate change.
5. Test when possible.
6. Check `git status` again.

## Telegram

Telegram is used for communication and notifications from the agent.

Use it for concise:

- status updates;
- GitHub summaries;
- reminders;
- automation results.

Avoid unnecessary notifications.

## Secrets

Never include credentials, tokens, API keys, passwords, or private keys in workspace documentation or Git commits.

## Related

- [Agent workspace](/concepts/agent-workspace)
