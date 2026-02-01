# Contributing

This list is generated from YAML. **Do not edit the generated file (e.g. `readme-sample.md`) directly.**

## How to contribute

1. **Add or edit entries** in `data/`. One file per item; filename = slug (e.g. `example.yml`).
2. **Categories** are in `meta/categories.yml`. Set `main_category` in each entry to an existing `id`.
3. **CI** runs [alternbits/opendata](https://github.com/alternbits/opendata) on push/PR. No compiler in this repo; the action validates and compiles.
4. **Commit** the generated file when it changes (CI will fail if it’s out of date).

## Data file (`data/{slug}.yml`)

Required: **name**, **slug** (match filename), **url**, **oneliner** (or **online_description**), **main_category**.  
Optional: description, position, categories, date_added, date_modified.

## Config (`config.yml`)

**output** — Generated filename (default `readme.md`). This template uses `readme-sample.md`.

## Full docs

Data format, meta options, badges, footer: [alternbits/opendata CONTRIBUTING](https://github.com/alternbits/opendata/blob/main/CONTRIBUTING.md).
