# Async Standup

Generate daily standup updates and weekly recaps by reviewing your calendar, email, and Notion activity — no more staring at a blank text box trying to remember what you did yesterday.

## Commands

### `/standup`
Generates a daily async standup update. Scans your calendar, email, and Notion for activity since the last workday, then produces a clean Yesterday / Today / Blockers update formatted for your chat platform.

### `/standup-weekly`
Generates a weekly recap covering the past 5 business days. Produces a Highlights / In Progress / Collaboration / Next Week / Blockers summary — perfect for end-of-week updates or skip-level visibility.

## Skills

### standup-formats
Ask Claude about standup best practices, formatting tips, or how to customize your update style. Includes guidance for different team types (engineering, product, sales) and culture levels (casual vs. formal).

## Setup

1. Install the plugin in Cowork
2. Connect your data sources (Calendar, Email, Notion) via Cowork's connector settings
3. Run `/standup` to generate your first update

The plugin works with whatever sources are connected — more sources means richer standups, but it handles missing ones gracefully.

## Customization

This plugin uses `~~chat` as a placeholder for your team's chat platform. See `CONNECTORS.md` for details. When you install the plugin, you can customize it to reference Slack, Teams, or whatever your team uses.

## Tips

- Run `/standup` first thing in the morning to get a draft, then tweak before posting
- Run `/standup-weekly` on Friday afternoon to capture the full week
- The standup skill can help you refine your team's standup format — just ask about "standup best practices"
