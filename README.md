# DiscoverabilityOps Standard

**DiscoverabilityOps™** is an open technical standard for measuring and improving how service businesses are detected, interpreted, and recommended inside AI-driven answer engines (ChatGPT, Gemini, Perplexity, Copilot, etc.).

Traditional SEO optimizes for clicks.  
DiscoverabilityOps optimizes for **answers**.

This repository hosts the canonical specification, example artifacts, and governance documents for the DiscoverabilityOps Standard.

---

## What This Standard Covers

The standard defines:

- **AI Discovery Rank (ADR)** — a composite score that measures how reliably a business is surfaced and referenced by AI systems for relevant, real-world queries.
- **Visibility Evidence Rating (VER)** — an assessment of the strength, recency, and distribution of proof signals (reviews, citations, profiles, content, etc.).
- **Competitive Context** — how a given business compares to others in its region/category from an AI visibility perspective.
- **Fix-Levers** — a practical set of levers operators can pull to move from “AI-invisible” to consistently discoverable in under 90 days.
- **Standardized Artifacts** — JSON-based artifacts that describe scans, ADR outputs, and implemented fixes in a machine-readable way.

The standard is designed to be:

- **Open** — no proprietary lock-in, no paywall to read or implement.
- **Practical** — built for working operators, agencies, and SMBs.
- **Versioned** — explicit semantic versioning (v1.2, v1.3, etc.).
- **Implementation-neutral** — tools, agencies, and platforms can adopt it without adopting any specific vendor.

---

## Who This Is For

The DiscoverabilityOps Standard is purpose-built for:

- **Service businesses** (HVAC, roofing, plumbing, real estate, trades, consulting)
- **Local and regional operators**
- **Agencies** that want a repeatable AI visibility framework
- **Product teams** building tools that grade or improve AI visibility

It is **not** optimized for:

- Pure enterprise governance/compliance programs
- Closed internal risk frameworks
- Black-box “proprietary” AI visibility scores

If you want a governance-heavy, enterprise-only framework, see AIVO Standard.  
If you want a working, field-tested playbook for real businesses, you’re in the right place.

---

## Repository Structure

```text
discoverabilityops-standard/
│
├── README.md                # This file
├── VERSION                  # Current spec version (e.g., v1.2)
├── CHANGELOG.md             # Version history
├── LICENSE                  # MIT License
│
├── spec/
│   └── standard.md          # Markdown specification (core of the standard)
│
├── docs/
│   ├── DiscoverabilityOps_Standard_v1.2.pdf   # PDF version of the spec
│   └── appendices.md                          # Supplemental examples / notes
│
├── examples/
│   ├── example-artifact.json           # Sample DiscoverabilityOps Artifact
│   └── example-adr-calculation.md      # ADR calculation walkthrough
│
└── governance/
    ├── CONTRIBUTING.md
    ├── GOVERNANCE.md
    └── CODE_OF_CONDUCT.md
