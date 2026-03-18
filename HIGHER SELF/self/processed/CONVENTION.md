# Processed Files — Naming Convention

## Format

```
processed-NNN_YYYY-MM-DD_type_title-slug.md
```

### Components

| Component | Description | Example |
|-----------|-------------|---------|
| `processed-NNN` | Sequential ID, zero-padded to 3 digits | `processed-001`, `processed-028` |
| `YYYY-MM-DD` | Date of the original content (not when processed) | `2026-02-13` |
| `type` | One of: `intake`, `video`, `session` | See below |
| `title-slug` | Kebab-case human-readable title | `karpathy-llm-deep-dive` |

### Types

- **intake** — Processed external content (YouTube videos, articles, podcasts, transcripts)
- **video** — Your own recorded videos
- **session** — AI conversation synthesis (Cursor or ChatGPT)

### Separator Logic

- **Underscores** (`_`) separate the four major components
- **Hyphens** (`-`) are used within the title slug and inside `processed-NNN`

### Assigning the Next ID

No counter file. Scan the directory, find the highest `processed-NNN`, increment by one. The files ARE the registry.

### Examples

```
processed-001_2026-03-18_session_first-higher-self-conversation.md
processed-002_2026-03-18_intake_naval-ravikant-how-to-get-rich.md
processed-003_2026-03-19_video_001-my-first-recording.md
```
