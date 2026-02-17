---
description: Generate a daily async standup update
allowed-tools: Read, Write, Bash, Grep, Glob, WebSearch, Task, mcp__*
---

Generate a daily standup update for the user by gathering their recent activity. Follow these steps:

## Step 1: Determine the time window

Today is the standup date. Look back to the previous workday:
- If today is Monday, look back to Friday.
- Otherwise, look back to yesterday.

## Step 2: Gather activity from all available sources

Run these checks in parallel where possible:

**Calendar**: Search for meetings and events from the previous workday through today. Note meeting titles, attendees, and any patterns (e.g., recurring 1:1s, planning sessions).

**Email**: Search for email threads the user sent or replied to during the window. Focus on threads with substantive content — skip newsletters, automated notifications, and marketing emails. Look for decisions made, requests completed, or blockers raised.

**Notion**: Search for Notion pages the user recently created or edited during the window. Look for document updates, database entries, and project pages that indicate meaningful work.

If a source is not connected, skip it silently — do not ask the user to connect it.

## Step 3: Synthesize into standup format

Organize findings into this structure:

**Yesterday** (or **Last Friday** if Monday):
- 3-6 bullet points summarizing what was accomplished
- Emphasize outcomes and deliverables, not just "had a meeting"
- Group related items (e.g., "Finalized Q2 roadmap in planning session and updated the Notion tracker")

**Today**:
- 2-4 bullet points on likely focus areas
- Infer from today's calendar, ongoing email threads, and incomplete work from yesterday
- Be specific: "Continue reviewing PR #142" is better than "Code review"

**Blockers**:
- Any blockers or dependencies identified from email threads or meeting context
- If none found, write "None" — do not fabricate blockers

## Step 4: Format for ~~chat

Format the output as a clean message ready to paste into ~~chat:

```
*Daily Standup — [Date]*

*Yesterday:*
• [item]
• [item]

*Today:*
• [item]
• [item]

*Blockers:*
• [item or "None"]
```

Use bold markers (*text*) compatible with ~~chat formatting. Keep the total length under 200 words — standups should be scannable, not essays.

Present the standup to the user and ask if they want to adjust anything before posting.
