# Altern Open Data – Test Template

Standalone test template for [Altern Open Data](https://github.com/alternbits/opendata). Use this as a starter for a new awesome list or to try the compiler.

## What this is

- **data/** — One YAML file per list item (slug = filename).
- **meta/** — `info.yml` (title, badges, footer) and `categories.yml`.
- **config.yml** — Sets output file (e.g. `readme-sample.md`).
- **.github/workflows/validate.yml** — Runs [alternbits/opendata@v1](https://github.com/alternbits/opendata) on push/PR. No compiler in this repo.

## Use as a new project

1. Copy this folder into a new repo (or use as a template repo).
2. Edit **data/** and **meta/** for your list.
3. Push; CI validates and compiles. Commit the generated file (e.g. `readme-sample.md`) when it changes.

## Local testing

You need the compiler from the main repo. From the **opendata** repo root:

```bash
make build
cd template && ../compiler/bin/compile
```

Or use the action: push to a branch and open a PR; the workflow runs the compiler.

## Docs

- **CONTRIBUTING.md** — How to add entries and data format (summary).
- Full format and meta options: [alternbits/opendata CONTRIBUTING](https://github.com/alternbits/opendata/blob/main/CONTRIBUTING.md).
