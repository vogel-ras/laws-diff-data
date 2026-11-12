# laws-diff-data

Corpus for the laws-diff runners. One directory per law series.

- `laws/<prefix>/<series>/meta.json` — name, keywords, dates, version list
- `laws/<prefix>/<series>/text.json.gz` — article text, opened only for that series
- `ordinances/<prefix>/<municipality>/` — the same pair for one municipality
- `index/laws/<prefix>.jsonl` and `index/ordinances/<prefix>.jsonl` — one line per law

A new law adds one index line and one series directory. A new version rewrites that directory and its index line.

The `data` release still carries `laws.db.gz` and `si-gap.tar.gz` for the builder's working copy.
