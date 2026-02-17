# Connectors

## How tool references work

Plugin files use `~~category` as a placeholder for whatever tool the user
connects in that category. For example, `~~chat` might mean Slack,
Microsoft Teams, or Discord — depending on what your team uses.

Plugins are tool-agnostic — they describe workflows in terms of categories
rather than specific products.

## Connectors for this plugin

| Category | Placeholder | Options |
|----------|-------------|---------|
| Chat | `~~chat` | Slack, Microsoft Teams, Discord |

## Data sources

This plugin reads from whatever sources are connected in Cowork. It works best with:

- **Google Calendar** or **Outlook Calendar** — for meeting activity
- **Gmail** or **Outlook** — for email threads and decisions
- **Notion** — for document and project tracking activity

The more sources connected, the richer the standup. But the plugin gracefully handles missing sources — it just works with whatever's available.
