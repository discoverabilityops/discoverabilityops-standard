# DiscoverabilityOps Standard

DiscoverabilityOps™ is an open technical standard for measuring and improving how service businesses are detected, interpreted, and recommended inside AI-driven answer engines (ChatGPT, Gemini, Perplexity, Copilot, etc.).

Traditional SEO optimizes for clicks.  
DiscoverabilityOps optimizes for *answers*.

This repository hosts the canonical specification, example artifacts, and governance documents for the DiscoverabilityOps Standard.

--------------------------------------------------

## What This Standard Covers

The standard defines:

- AI Discovery Rank (ADR)
- Visibility Evidence Rating (VER)
- Competitive context modeling
- Fix-Levers
- DiscoverabilityOps Artifact (DOA)
- A multi-stage assessment workflow

The standard is:

- Open
- Practical
- Versioned
- Implementation-neutral

--------------------------------------------------

## Who This Is For

Built for:

- Service businesses
- Local and regional operators
- Agencies
- Product teams building AI visibility or AEO tools

Not optimized for enterprise-only compliance frameworks.

--------------------------------------------------

## Repository Structure

discoverabilityops-standard/
│
├── README.md
├── VERSION
├── CHANGELOG.md
├── LICENSE
│
├── spec/
│   └── standard.md
│
├── docs/
│   ├── DiscoverabilityOps_Standard_v1.2.pdf
│   └── appendices.md
│
├── examples/
│   ├── example-artifact.json
│   └── example-adr-calculation.md
│
└── governance/
    ├── CONTRIBUTING.md
    ├── GOVERNANCE.md
    └── CODE_OF_CONDUCT.md

--------------------------------------------------

## Versioning

This standard uses semantic versioning.

Current version:
v1.2

--------------------------------------------------

## DiscoverabilityOps Artifact (DOA)

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

--------------------------------------------------

## License

This standard is published under the MIT License.  
See LICENSE.

--------------------------------------------------

## How to Cite

“DiscoverabilityOps Standard v1.2”  
https://github.com/discoverabilityops/discoverabilityops-standard

--------------------------------------------------

## Contributing

See governance/CONTRIBUTING.md
