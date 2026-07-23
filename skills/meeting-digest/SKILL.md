---
description: Turn a Gemini meeting transcription into a sharp topic-based summary with decisions and action items. Optionally saves to second brain.
author: Dana Harel
---

You are processing a meeting transcription. The input is a Gemini auto-transcription — expect it to be garbled, repetitive, or incomplete in places. Read through the noise and extract what actually happened.

---

## Step 1 — Read the transcription

The user has pasted or attached a Gemini transcription. Read it in full.

Work with what's there — do not ask for clarification unless something critical is completely unreadable.

---

## Step 2 — Extract the substance

Identify:
- **Meeting title / participants / date** — from the transcription or context
- **Topics discussed** — the real agenda, not the small talk
- **Decisions made** — anything agreed on or resolved
- **Action items** — concrete next steps, with owner if mentioned
- **Open questions** — things left unresolved or flagged for follow-up

---

## Step 3 — Check for second brain

Check if the user has a second brain wiki at `~/Documents/second-brain/wiki/`.

If it exists:
- Read `wiki/index.md` to find the relevant project page
- Update that page with what's new and load-bearing from this meeting: decisions, status changes, new context, resolved or new open questions
- Do not duplicate existing info. Do not record ephemeral discussion.
- Format meeting entries as: `**[Date] — [Participants]:** one-line summary of what changed or was decided.`

If it doesn't exist: skip this step silently.

---

## Step 4 — Output the digest

Produce clean formatted text directly in the chat. Structure it by topic — not chronologically.

```
Meeting: [title or participants] — [date if known]

─────────────────────────────────

[Topic 1 name]
[2–4 tight bullets on what was discussed/decided on this topic]

[Topic 2 name]
[2–4 tight bullets]

... (as many topics as needed — skip topics with nothing meaningful)

─────────────────────────────────

Decisions
• [Decision] — [rationale or owner if mentioned]
• ...

Action items
• [Verb + action] — [Owner if known]
• ...

Open questions
• [Question or unresolved issue]
• ...
```

**Adapt the structure:**
- Skip "Decisions", "Action items", or "Open questions" entirely if there are none
- If the meeting was purely informational, say so in one line instead of forcing the format
- Topics should reflect the actual meeting — name them clearly, don't invent structure that wasn't there

---

## Style rules

- English always, even if the meeting was in Hebrew
- Bullets are tight — one idea each, no padding
- Action items start with a verb and are specific enough to act on
- If something was ambiguous in the meeting, note it briefly rather than resolving it artificially
- No trailing summaries, no meta-commentary
