# Post samples — drop zone for brand-voice

Drop posts here, then invoke the **`brand-voice`** skill to analyze them into `brand/voice-profile.md`.

## Convention

- **One post per file** (`.md` or `.txt`).
- **Source is decided by the subfolder:**
  - `own/` — Bugra's own posts. These define the **voice** (tone, vocabulary, rhythm, signature moves).
  - `others/` — other people's posts. These contribute **technique only** (hooks, formatting, pacing). Their voice is never copied.
- A file dropped directly in `samples/` with no subfolder is treated as **own**.

## Optional per-file frontmatter

Helps the analysis; inferred or asked for if absent.

```yaml
---
platform: linkedin        # linkedin | x | threads | blog | video | ...
metrics: "1.2k likes, 80 comments, 340k impressions"
note: "posted 9am ET"
---
```

## Running it

- **Whole folder:** invoke `brand-voice` with no argument — analyzes every `.md`/`.txt` file that doesn't already have a report in `brand/analysis/`. Already-analyzed samples are skipped; ask to re-run to force one.
- **Single file:** invoke `brand-voice <filename>` — analyzes just that file.

Every run writes a per-post report to `brand/analysis/`. The voice profile is updated only after the skill asks and you confirm.
