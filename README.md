![version](https://img.shields.io/github/v/release/discoverabilityops/discoverabilityops-standard)
![license](https://img.shields.io/github/license/discoverabilityops/discoverabilityops-standard)
![stars](https://img.shields.io/github/stars/discoverabilityops/discoverabilityops-standard)

DiscoverabilityOps Standard

DiscoverabilityOps™ is an open technical standard for understanding how service businesses are detected, interpreted, and recommended inside AI-driven answer engines such as ChatGPT, Gemini, Claude, Perplexity, and Copilot.

Traditional SEO optimizes for clicks.
DiscoverabilityOps optimizes for answers — the only currency AI models understand.

This repository hosts the canonical specification, appendices, examples, and governance documents for the DiscoverabilityOps Standard.

What This Standard Covers (v4.0.0)

The v4 release introduces a modern, plain-English framework for how AI recommendation systems evaluate businesses.

The standard defines:

AI Discovery Rank (ADR v4)
A 0–100 authority & visibility score based on relevance, velocity, novelty, impact, and confidence.

Visibility Evidence Rating (VER v4)
A 0.00–1.00 confidence score measuring trust in the evidence footprint.

Entity Identity & Dominant Noun Pattern Model
How AI determines what a business actually is based on reviews, content, photos, and citations.

Velocity & Decay Rules
Why fast, fresh signals matter more than history.

Contradiction Penalties
How mismatches remove businesses from AI recommendations.

Unified Cognitive Artifact (UCA v1.0)
The structured JSON output replacing the older DOA schema.

Fix-Levers (Updated 10-Lever Model)
The standardized interventions for improving real AI visibility.

Competitive Context
How AI compares local businesses, directories, and proxies.

This standard is:

Open

Practical

Versioned

Implementation-neutral

Written in plain English

Designed for agencies, operators, and AI visibility practitioners

Who This Is For

The DiscoverabilityOps Standard is built for:

Service businesses

Local and regional operators

Agencies and consultants

Product teams building AI visibility, AEO, or recommendation tools

Researchers studying AI discovery behaviors

It is not written for bureaucratic compliance frameworks or enterprise-only usage.
This is a practical standard for real people solving real visibility problems.

Repository Structure
discoverabilityops-standard/
│
├── README.md
├── VERSION.md
├── CHANGELOG.md
├── LICENSE
│
├── spec/
│   └── standard.md                 # DiscoverabilityOps Standard (v4.0.0)
│
├── docs/
│   ├── appendices.md               # Expanded models, details, examples
│   ├── DiscoverabilityOps_v1.2.pdf # Legacy PDF (kept for historical reference)
│
├── examples/
│   ├── example-artifact.json       # UCA v1.0 example
│   └── example-adr-calculation.md  # ADR v4 calculation example
│
└── governance/
    ├── CONTRIBUTING.md
    ├── GOVERNANCE.md
    └── CODE_OF_CONDUCT.md

Versioning

This standard uses semantic versioning.

Current version:
v4.0.0

This release introduces:

ADR v4

VER v4

UCA v1.0

Noun-pattern identity model

Category rewrite rules

Velocity multipliers

Contradiction slashing penalties

Updated Fix-Levers

A new standardized document structure

See CHANGELOG.md for full details.

Unified Cognitive Artifact (UCA v1.0)

(Replaces the old DOA schema)

{
  "version": "1.0",
  "entity": { "name": "Sample Business", "region": "Bartow County, GA" },
  "metrics": { "adr_v4": 83, "ver_v4": 0.74 },
  "signals": {
    "profiles": ["GBP", "Yelp"],
    "content_sources": ["Website", "YouTube"],
    "citations": ["localchamber.com"]
  },
  "fix_levers": ["category_tightening", "structured_data_alignment"],
  "scan_context": {
    "stage": "stage_1_deep_mapping",
    "query_set_version": "2025-11-default"
  }
}


Full schema located in:

spec/standard.md

examples/example-artifact.json

License

This standard is published under the MIT License.
See LICENSE.

How to Cite

“DiscoverabilityOps Standard v4.0.0”
https://github.com/discoverabilityops/discoverabilityops-standard

Contributing

See governance/CONTRIBUTING.md.
