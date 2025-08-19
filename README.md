# CSU AI Prompts

A campus-wide, curated collection of prompts for teaching, research, student services, and IT. Each prompt lives in its own folder with metadata (YAML front‑matter) and a human-readable body.

- **Browse:** `prompts/` by domain (teaching, research, admin, it, student-life)
- **Contribute:** open a **New Prompt** issue (guided form) or a PR
- **Validate:** CI checks schema, tags, and safety notes
- **Export:** machine‑readable catalog builds to `exports/catalog.jsonl`

## Quick start

1. Open a **New Prompt** issue (Issues → New → *New prompt*).
2. A maintainer will help place it in the right folder and tag it.
3. Or submit a PR adding a folder under `prompts/<domain>/<slug>/` with:
   - `prompt.md` (front‑matter + body)
   - `examples.jsonl` (at least 1 input/output example)

## Front‑matter (required fields)

See `schema/prompt.schema.json` for the exact spec. Minimal example:

```yaml
---
title: Socratic Check-ins for Weekly Problem Sets
slug: socratic-checkins
version: 1.1.0
status: active
audience: undergraduate
domain: teaching
tags: [socratic, tutoring, subject/math]
license: CC-BY-4.0
ferpa_sensitive: false
---
````

## Safety & privacy

- Do **not** include student PII (personally identifiable information).
- Prompts that may touch student data must set `ferpa_sensitive: true` and include `security_notes` explaining how to anonymize.

## License

- **Prompt content:** Creative Commons **CC BY 4.0** (see `LICENSES/CC-BY-4.0.txt`).
- **Scripts & CI snippets:** **MIT** (see `LICENSES/MIT.txt`).

See `LICENSE` for the summary.