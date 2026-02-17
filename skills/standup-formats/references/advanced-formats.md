# Advanced Standup Formats

## Format Variations by Team Type

### Engineering Teams

Engineering standups benefit from technical specificity:

```
Yesterday:
• Merged PR #247 — adds rate limiting to /api/users endpoint
• Pair-debugged flaky CI with Alex — root cause was race condition in test setup
• Reviewed RFC: "Migrate to event-driven auth" — left comments on retry strategy

Today:
• Ship rate limiting to production (behind feature flag)
• Start spike on WebSocket connection pooling (ticket ENG-891)

Blockers:
• Waiting on DevOps to provision staging Redis cluster (requested Tue)
```

### Product / Design Teams

Focus on decisions, user impact, and stakeholder alignment:

```
Yesterday:
• Finalized onboarding flow wireframes — shared in #design-reviews
• User interview with Enterprise Acme Corp — key insight: they need bulk import
• Aligned with Eng on scope for v1 settings page (cut advanced permissions)

Today:
• High-fidelity mockups for onboarding steps 1-3
• Prep for Thursday's design review

Blockers:
• Need copy from Marketing for empty states (asked Mon)
```

### Sales / Business Teams

Emphasize pipeline, relationships, and revenue signals:

```
Yesterday:
• Discovery call with Acme Corp (50-seat opportunity) — scheduling demo for Fri
• Closed Contoso renewal ($48k ARR, 2-year term)
• Updated Q2 forecast in CRM — pipeline at 127% of target

Today:
• Prep demo environment for Acme Corp
• Follow up on Northwind proposal (sent last Wed, no response)

Blockers:
• Need updated pricing sheet from RevOps for enterprise tier
```

## Adapting Tone

### Casual / Startup Culture
- Emojis are fine but don't overdo it
- First names, abbreviations, internal slang OK
- "Shipped the thing!" is acceptable

### Formal / Enterprise Culture
- Full sentences, professional tone
- Reference ticket/project IDs consistently
- "Completed deployment of authentication service update"

### Remote-First Teams
- Extra specificity since there's no hallway context
- Mention timezone-relevant details ("Will be offline 2-4pm PT for dentist")
- Link to artifacts instead of describing them

## Anti-Patterns

### The Novel
A standup that reads like a diary entry. If it's more than 8 bullets total, consolidate or move details to a separate update.

### The Performative Update
Writing to look busy rather than to communicate. "Attended 6 meetings" tells your team nothing useful.

### The Copy-Paste
Identical standup every day. If your work hasn't changed, something might be wrong — or your standup isn't specific enough.

### The Ghost Blocker
Listing something as a blocker but never following up or escalating. If it's been a blocker for 3+ days, it needs a different approach.
