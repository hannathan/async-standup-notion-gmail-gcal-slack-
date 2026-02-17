---
name: standup-formats
description: >
  This skill should be used when the user asks about "standup format",
  "standup best practices", "how to write a good standup", "status update tips",
  "async standup advice", or wants to customize how their standup updates
  are structured and worded.
version: 0.1.0
---

# Standup Formats & Best Practices

Domain knowledge for writing effective async standup updates and weekly recaps.

## Core Principles

A good async standup is **scannable, specific, and actionable**. It replaces a synchronous meeting, so it must communicate clearly without follow-up questions.

### The 3 Rules of Async Standups

1. **Outcomes over activities** — "Shipped the auth fix to staging" beats "Worked on auth." Describe what changed in the world, not what you did with your time.

2. **Specificity over vagueness** — Include ticket numbers, PR links, document names, or people's names. "Reviewed Sarah's RFC on caching" is useful. "Did some reviews" is not.

3. **Brevity over completeness** — A standup is not a journal. 3-5 bullets per section. If something takes more than one sentence to explain, it probably deserves its own conversation.

## Standard Format: Yesterday / Today / Blockers

The classic three-section format. Works for most teams.

```
Yesterday:
• Completed [specific deliverable]
• Met with [person/team] about [topic] — decided [outcome]
• Reviewed [PR/doc/ticket] — [approved/requested changes/left feedback]

Today:
• Focus on [specific task] — aiming to [concrete milestone]
• [Meeting] with [who] to [purpose]

Blockers:
• Waiting on [person] for [thing] since [date]
• [System/tool] is down, blocking [task]
```

## Writing Tips

### Good Bullets

- Start with a past-tense verb for "yesterday" items: Shipped, Completed, Reviewed, Finalized, Debugged, Drafted, Merged
- Start with a plan verb for "today" items: Continue, Start, Focus on, Meet with, Ship, Finalize
- Include context parenthetically when helpful: "Merged auth PR (#142 — fixes the login timeout bug)"

### Weak Bullets to Avoid

- "Worked on stuff" — too vague
- "Meetings all day" — which meetings? what happened?
- "Making progress on the project" — what project? what progress?
- "Fixing bugs" — which bugs? are they fixed?

### Blockers Section

Only list genuine blockers — things that are preventing progress, not just things that are hard. A blocker should name:
- What is blocked
- Who or what is blocking it
- How long it has been blocked

If there are no blockers, say "None." Do not write "No blockers!" with enthusiasm — it sounds performative.

## Weekly Recap Format

Weekly recaps serve a different purpose than dailies. They answer: "What moved forward this week, and what's the plan for next week?"

Prioritize **highlights** — the 3-5 most impactful things. A good test: would your manager mention this in their own status update? If yes, it's a highlight.

## Formatting for Chat Platforms

- Use `*bold*` for section headers (Slack-compatible)
- Use `•` for bullet points (cleaner than `-` in most chat apps)
- Keep total length under 200 words for daily, 350 for weekly
- Add a date stamp at the top so it's identifiable in scroll-back

## Additional Resources

For detailed reference on adapting formats to different team cultures and cadences, see `references/advanced-formats.md`.
