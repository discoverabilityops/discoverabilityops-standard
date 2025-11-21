# DiscoverabilityOps Standard (v1.2)

This is the canonical Markdown version of the DiscoverabilityOps Standard.  
The PDF version (“DiscoverabilityOps Standard.pdf”) contains the formatted specification.  
This Markdown file exists so tools, contributors, and implementers can work with a plain-text version of the standard.

------------------------------------------------------------
## 1. Purpose & Scope
The DiscoverabilityOps Standard defines how to measure, analyze, and improve the visibility of a service business inside AI-driven answer engines such as ChatGPT, Gemini, Perplexity, and Copilot.

This standard covers:
- AI Discovery Rank (ADR)
- Visibility Evidence Rating (VER)
- DiscoverabilityOps Artifact (DOA)
- Ten Fix-Levers for improving visibility
- A multi-stage workflow for assessment
- Competitive context interpretation
- Standardization of audit outputs

This document is implementation-neutral.  
Any vendor, platform, or agency may adopt it.

------------------------------------------------------------
## 2. Core Definitions

### **AI Discovery Rank (ADR)**
A composite score (0–100) estimating how reliably an AI model surfaces a business for real-world queries.

### **Visibility Evidence Rating (VER)**
A confidence rating (0.00–1.00) describing the strength, consistency, and distribution of supporting signals.

### **DiscoverabilityOps Artifact (DOA)**
A JSON-based, machine-readable output summarizing:
- entity metadata
- ADR and VER
- supporting signals
- competitive insights
- fix-levers to apply

### **Fix-Levers**
Ten standardized interventions used to strengthen visibility inside AI systems.

### **Stages (Workflow)**
A structured process for evaluations:
- Stage 0: Field Scan
- Stage 1: Deep Visibility Mapping
- Stage 2: Fix-Lever Execution
- Stage 3: Authority Expansion

------------------------------------------------------------
## 3. AI Discovery Rank (ADR)

ADR answers a simple question:  
**“How often will an AI model recommend or reference this business for relevant queries?”**

Components typically include:
- Detectability of the entity
- Category clarity
- Regional relevance
- Supporting evidence signals
- Competitive displacement pressure
- Consistency of appearance across models

ADR ranges:
- **0–39:** Invisible  
- **40–69:** Partially visible  
- **70–89:** Strong visibility  
- **90–100:** Dominant authority  

Exact formulas may vary, but ADR must remain a 0–100 normalized value aligned with this spec.

------------------------------------------------------------
## 4. Visibility Evidence Rating (VER)

VER represents **confidence** in the evidence supporting AI visibility.

Factors:
- Strength of citations
- Recency of updates
- Review footprint & distribution
- Content footprint
- Profile completeness and alignment
- Third-party trust signals

VER ranges:
- **0.00–0.39:** Weak evidence  
- **0.40–0.69:** Moderate evidence  
- **0.70–1.00:** Strong evidence  

VER is not a “review score.”  
It is an evidence confidence multiplier.

------------------------------------------------------------
## 5. Stages (Workflow Overview)

### **Stage 0 — Field Scan**
Purpose: Determine if the business appears *at all* in AI-driven answers.  
Outputs:
- ADR estimate
- Competitor list
- DOA (Stage 0)

### **Stage 1 — Deep Visibility Mapping**
Purpose: Identify limiting factors and signal weaknesses.  
Outputs:
- Expanded DOA
- VER calculation
- Fix-Lever recommendations

### **Stage 2 — Fix-Lever Execution**
Purpose: Implement changes that directly impact ADR and VER.  
Examples:
- Entity clarity hardening
- Review footprint expansion
- Topic cluster coverage
- Local proof density
- Structured data improvements

### **Stage 3 — Authority Expansion**
Purpose: Expand the brand’s total surface area for long-term dominance.  
Examples:
- Multi-modal content
- Strategic citations
- Geographic/entity expansion

------------------------------------------------------------
## 6. The Fix-Levers (10)

These levers represent the standardized interventions used across industries:

1. **Entity Clarity**
2. **Category Alignment**
3. **Review Footprint & Distribution**
4. **Local Proof Density**
5. **Profile Unification**
6. **Topic Cluster Coverage**
7. **Regional Relevance Signals**
8. **Structured Data & Schema Signals**
9. **Content Authority & Depth**
10. **Platform Presence Consistency**

Implementations may include additional steps but must map to these ten to remain compliant.

------------------------------------------------------------
## 7. DOA Schema (DiscoverabilityOps Artifact)

A DOA must include:

- `version` — spec version used  
- `entity` — name, category, region  
- `metrics` — ADR, VER  
- `signals` — profiles, citation examples, content sources  
- `fix_levers` — list of recommended levers  
- `scan_context` — stage, date, query set used  
- `competitors` (optional) — list with ADR estimates  

Example DOA is available in `/examples/example-artifact.json`.

------------------------------------------------------------
## 8. Competitive Context

AI visibility occurs in a competitive landscape.  
This section defines:

- how competitors are selected  
- how comparative ADR scoring works  
- how displacement pressure is interpreted  
- how “dominant entities” influence recommendations  

Implementations must:
- Assess competitors in the same category + region  
- Document ADR spread  
- Represent competitor data in the DOA when possible  

------------------------------------------------------------
## 9. Implementation Guidance (Non-Normative)

This section provides practical but optional guidance for:

- Agencies performing audits  
- Product teams integrating ADR/VER scoring  
- SMB operators using manual processes  
- Cross-model evaluation  

Guidance may include:
- Example workflows  
- Recommended query sets  
- Signal-building strategies  
- Reporting best practices  

------------------------------------------------------------
## 10. Versioning

DiscoverabilityOps uses semantic versioning:

- **MAJOR** — conceptual / structural changes  
- **MINOR** — new examples, clarifications  
- **PATCH** — editorial fixes  

Current version: **v1.2**

------------------------------------------------------------
## 11. References

Normative:
- None at this time.

Non-Normative:
- Example artifacts  
- Appendices  
- External AEO research papers  
