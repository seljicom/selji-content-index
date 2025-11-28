# SELJI Content Index

This repository maintains a structured, version-controlled index of canonical URLs published on **SELJI.com**. It is designed for documentation, research, SEO architecture analysis, and reproducible workflows used across SELJI tools and automation projects.

This repository does **not** contain article text or promotional material - only metadata such as URLs, categories, and update information.

---

## Purpose

- Track the evolution of SELJI’s content structure  
- Provide a stable public reference for research and automated tools  
- Enable reproducible tests (crawlability, metadata extraction, link validation, etc.)  
- Maintain a changelog of URL-level updates and rewrites  
- Support the `selji-tools` and `selji-workflow-engine` projects

---

## Directory Structure

```
urls/          JSON files listing live URLs grouped by month or function
notes/         Internal documentation and planning notes
tools/         Small utilities to validate or analyze URL lists
```

---

## How It’s Used

- **Crawlers** use `urls/*.json` as the source of truth  
- **Automated validators** test live status and canonical tags  
- **Content workflows** refer to previous update dates  
- **Researchers** can inspect changes over time

---

## File Formats

All URL lists follow this format:

```json
[
  {
    "url": "https://selji.com/example-article/",
    "images": 2,
    "lastmod": "2025-01-14"
  }
]
```

This keeps the data machine-readable and tool-friendly.

---

## Notes

This repository is intentionally minimal. It exists to ensure transparency, reproducibility, and consistency in how SELJI content is managed across related public tools.
