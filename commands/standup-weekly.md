---
description: Generate a weekly recap of your work activity
allowed-tools: Read, Write, Bash, Grep, Glob, WebSearch, Task, mcp__*
---

Generate a weekly recap summarizing the user's work over the past 5 business days. This is a higher-level view than the daily standup — think "what would my manager or teammates want to know about my week?"

## Step 1: Determine the time window

Look back over the current or most recent work week (Monday through Friday). If today is not Friday, cover Monday through today.

## Step 2: Gather activity from all available sources

Run these in parallel where possible:

**Calendar**: Pull all meetings from the week. Categorize them:
- Planning/strategy sessions
- 1:1s and syncs
- External meetings (clients, vendors, cross-team)
- Interviews or other special events

**Email**: Search sent emails and replies from the week. Identify:
- Major threads or decisions
- Cross-team collaboration
- Requests completed or received
- Any escalations

**Notion**: Search for pages created or significantly edited during the week. Look for:
- Documents drafted or finalized
- Database entries added (tasks, bugs, specs)
- Project pages updated

Skip any source that is not connected — do not mention missing sources.

## Step 3: Synthesize into weekly recap format

Organize into this structure:

**Highlights** (3-5 items):
- The most impactful things accomplished this week
- Focus on outcomes: shipped features, closed deals, decisions made, docs finalized
- Combine related activities into single cohesive bullets

**In Progress**:
- 2-4 items that are underway but not yet complete
- Include expected completion or next milestone

**Collaboration**:
- Notable cross-team or external interactions
- Key meetings and their outcomes (not just "attended standup")
- Only include meetings where something meaningful happened

**Next Week**:
- 2-3 priorities for the coming week
- Infer from calendar, ongoing threads, and incomplete work

**Blockers / Risks**:
- Anything that slowed progress or could impact next week
- "None" if nothing identified — do not invent problems

## Step 4: Format for ~~chat

Format as a polished message for ~~chat:

```
*Weekly Recap — [Date Range]*

*Highlights:*
• [item]
• [item]
• [item]

*In Progress:*
• [item]

*Collaboration:*
• [item]

*Next Week:*
• [item]

*Blockers:*
• [item or "None"]
```

Keep it under 350 words. Use bold (*text*) compatible with ~~chat formatting.

Present the recap to the user and ask if they want to adjust anything.
