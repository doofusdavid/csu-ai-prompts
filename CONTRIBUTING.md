# Contributing

Thanks for helping make AI at CSU thoughtful and useful.

## Ways to contribute

- Propose a **new prompt** via the "New Prompt" issue form.
- Improve an existing prompt (clarify instructions, add examples).
- Add tags or collections to improve discovery.

## PR checklist

- [ ] One new folder under `prompts/<domain>/<slug>/`
- [ ] `prompt.md` contains valid front‑matter (passes CI)
- [ ] At least one example in `examples.jsonl`
- [ ] Tags are from `TAGS.md` (or propose additions in the PR)
- [ ] If `ferpa_sensitive: true`, include `security_notes`

## Review standards

- Prompts should be **clear**, **actionable**, and **non‑leaky** (no unnecessary data requests).
- Prefer **principles + guardrails**, not brittle scripts.
- Keep it vendor‑neutral when possible; note model suggestions in `models`.