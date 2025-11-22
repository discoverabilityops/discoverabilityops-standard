DiscoverabilityOps Standard (v4.0.0)

Plain-English Edition
The Canonical Specification for AI Visibility & Authority

This Markdown file is the official standard.
PDF formatting is handled separately.

============================================================

1. Introduction

AI systems (ChatGPT, Gemini, Claude, Perplexity, Copilot, etc.) increasingly act as recommendation engines for everyday questions like:

“Who is the best plumber near me?”

“Top realtors in my county?”

“Best accountant for small businesses?”

This standard defines how AI chooses which businesses to recommend, and provides a consistent way to measure, evaluate, and improve that visibility.

DiscoverabilityOps exists for one purpose:

Make sure small businesses are visible, clear, and trusted inside AI models so they get recommended when it matters.

This document explains the entire model in plain English.

============================================================

2. Scope

This standard covers:

How AI identifies and evaluates local businesses

How DiscoverabilityOps measures visibility and authority

The unified scoring model (ADR v4)

The evidence confidence model (VER v4)

Identity, category, and noun-pattern rules

Velocity and decay mechanics

Contradiction penalties

The unified output schema (UCA v1.0)

The 10 Fix-Levers for improving visibility

How to evaluate competitors

How to run consistent audits

It applies to service businesses of any size, across any region, category, or platform.

============================================================

3. Terminology (Plain English)
AI Discovery Rank (ADR v4)

A 0–100 score representing how likely an AI model is to recommend a business for real-world queries.

Evidence Confidence Rating (VER v4)

A 0.00–1.00 score representing how reliable the supporting proof is across the web.

Entity Identity

The machine-readable representation of who the business is.

Dominant Noun Pattern

The nouns AI sees most often in reviews, listings, photos, content, and citations — this determines the real category of a business.

Unified Cognitive Artifact (UCA v1.0)

A structured JSON output containing the results of an AI visibility audit.

Fix-Levers

Ten standardized interventions used to improve AI visibility.

Contradiction

Any mismatch between reviews, services, content, listings, or schema.

============================================================

4. How AI Chooses Which Businesses to Recommend

AI doesn’t choose “the best.”
AI chooses the safest — the business with the clearest identity, cleanest footprint, and strongest supporting signals.

The AI’s primary behavior:

Reduce risk. Recommend only what is proven, clear, and consistent.

This standard defines the factors behind that choice.

============================================================

5. ADR v4 — Authority & Discovery Model

ADR v4 is powered by five forces:

Relevance

Velocity

Novelty

Impact

Forecast Confidence

These combine into a 0–100 score.

ADR Ranges:

0–39: Invisible

40–69: Partially visible

70–89: Strong visibility

90–100: High Authority / Dominant

============================================================

6. VER v4 — Evidence Confidence Model

VER evaluates the reliability of proof:

citations

listings

reviews

photos

content footprint

profiles

schema

consistency

VER ranges:

0.00–0.39: Weak

0.40–0.69: Moderate

0.70–1.00: Strong

============================================================

7. Entity Identity & Dominant Noun Pattern

AI determines “what you are” using noun patterns found across:

reviews

listings

schema

photos

website copy

GBP Products

citations

These nouns override the category a business chooses for itself.

Example:

A company claims “Electrician,”
… but 60% of reviews mention “generator installation”
… and product listings include “Standby generators”

AI rewrites the category as:

Standby Generator Specialist

Specialists rank higher than generalists.

============================================================

8. Velocity, Recency, and Decay

AI rewards fresh, fast-moving signals:

Signals within 18 hours get the highest boost.

Signals 18–72 hours still help, but less.

Signals older than 72 hours fade quickly.

Signals older than 30 days are stale.

Bursts beat drips.
Freshness beats history.

Velocity is a multiplier in ADR v4.

============================================================

9. Contradiction Penalties

AI punishes contradictions because contradictions create risk.

Examples:

Reviews mention “emergency service” but the site does not.

GBP lists “Electrician” but website says “HVAC.”

One listing shows a different address.

Schema lists services the site never mentions.

One contradiction can remove a business from recommendations.

ADR v4 includes:

a Contradiction Map

a Slashing Penalty applied before the final score

============================================================

10. Category Resolution & Rewrite Logic

AI evaluates:

What does this business actually do?

What is it known for?

What is the safest category match?

Category rewrites are driven by:

dominant nouns

review themes

GBP Products

content clusters

citation patterns

If unclear → AI lowers authority.
If consistent → AI may rewrite the business upward into a specialist identity.

============================================================

11. UCA v1.0 — Unified Cognitive Artifact
{
  "version": "1.0",
  "entity": {
    "name": "",
    "category": "",
    "region": "",
    "noun_pattern": [],
    "identity_notes": ""
  },
  "metrics": {
    "adr_v4": 0,
    "ver_v4": 0.0,
    "velocity_multiplier": 1.0,
    "contradiction_penalty": 0.0
  },
  "signals": {
    "profiles": [],
    "citations": [],
    "content_sources": [],
    "reviews": {
      "count": 0,
      "distribution": "",
      "themes": []
    }
  },
  "contradictions": [],
  "category_clusters": [],
  "competitors": [],
  "recommendations": {
    "fix_levers": [],
    "priority_actions": []
  },
  "scan_context": {
    "stage": "0 | 1 | 2 | 3",
    "date": "",
    "query_set": []
  }
}


============================================================

12. Evaluation Workflow
Stage 0 — Field Scan

Checks if the business appears in AI at all.

Stage 1 — Deep Mapping

Identifies contradictions, weak signals, and category drift.

Stage 2 — Fix-Lever Execution

Applies the 10 Levers to improve clarity, signals, and authority.

Stage 3 — Authority Expansion

Long-term footprint expansion.

============================================================

13. Fix-Levers (Updated)

Entity Identity Hardening

Category Tightening

Review Footprint Strengthening

Local Proof Density

Profile Unification

Topic Cluster Expansion

Regional Relevance

Structured Data Alignment

Content Depth & Authority

Platform Presence Consistency

============================================================

14. Competitive Context

AI visibility is competitive.

A business is evaluated relative to:

peers in same category

peers in same region

dominant national brands

directory proxies (Angi, Yelp, Thumbtack, etc.)

Competitive displacement affects ADR.

============================================================

15. Implementation Guidance (Non-Normative)

Recommended practices:

realistic query sets

validate citations

use UCA as the audit output

cluster updates within short windows

resolve contradictions first

align website → reviews → schema

adopt routine monitoring

============================================================

16. Versioning

Major = structural change
Minor = new examples
Patch = editorial fixes

Current version: v4.0.0

============================================================

17. Migration Notes (v1.2 → v4)

ADR unified into 5-force model

VER updated

DOA replaced by UCA

Contradiction penalties expanded

Category rewrite rules formalized

Noun pattern model added

Velocity multipliers added

Fix-Levers updated

Workflow unchanged

============================================================

END OF STANDARD