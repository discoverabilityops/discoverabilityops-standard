# DiscoverabilityOps Standard

**DiscoverabilityOps™** is an open technical standard for measuring and improving how service businesses are detected, interpreted, and recommended inside AI-driven answer engines (ChatGPT, Gemini, Perplexity, Copilot, etc.).

Traditional SEO optimizes for clicks.  
DiscoverabilityOps optimizes for **answers**.

This repository hosts the canonical specification, example artifacts, and governance documents for the DiscoverabilityOps Standard.

---

## What This Standard Covers

The standard defines:

- **AI Discovery Rank (ADR)** — how reliably a business is surfaced by AI.
- **Visibility Evidence Rating (VER)** — strength, recency, and trust of proof signals.
- **Competitive Context** — how a business compares in its region/category.
- **Fix-Levers** — actionable interventions that move a business from invisible to discoverable.
- **Standardized Artifacts (DOA)** — JSON-based, interoperable audit outputs.

The standard is:

- **Open**
- **Practical**
- **Versioned**
- **Implementation-neutral**

---

## Who This Is For

Built for:

- Service businesses  
- Local/regional operators  
- Agencies  
- Product teams building AI visibility tools  

Not optimized for enterprise-only compliance frameworks.

---

## Repository Structure

discoverabilityops-standard/
│
├── README.md
├── VERSION
├── CHANGELOG.md
├── LICENSE
│
├── spec/
│ └── standard.md
│
├── docs/
│ ├── DiscoverabilityOps_Standard_v1.2.pdf
│ └── appendices.md
│
├── examples/
│ ├── example-artifact.json
│ └── example-adr-calculation.md
│
└── governance/
├── CONTRIBUTING.md
├── GOVERNANCE.md
└── CODE_OF_CONDUCT.md

yaml
Copy code

---

## Versioning

This standard uses semantic versioning.

Current version:

v1.2

pgsql
Copy code

---

## DiscoverabilityOps Artifact (DOA)

```json
{
  "version": "1.2",
  "entity": { "name": "Example HVAC Co.", "region": "Dallas, TX" },
  "metrics": { "adr": 78, "ver": 0.71 },
  "signals": {
    "profiles": ["GBP", "Yelp"],
    "content_sources": ["Website", "YouTube"],
    "citation_examples": ["chatgpt:gpt-4o", "perplexity:online"]
  },
  "fix_levers": ["entity_clarity", "review_distribution"],
  "scan_context": {
    "stage": "stage_0_field_scan",
    "query_set_version": "2025-11-default"
  }
}
License
Published under MIT.
See LICENSE.

How to Cite
“DiscoverabilityOps Standard v1.2”
https://github.com/discoverabilityops/discoverabilityops-standard

Contributing
See governance/CONTRIBUTING.md.
