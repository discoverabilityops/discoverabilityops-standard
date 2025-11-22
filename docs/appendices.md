Appendices – DiscoverabilityOps Standard (v4.0.0)

Additional Notes, Expanded Models, and Worked Examples

This appendix expands on concepts described in the main standard.

============================================================

A. ADR v4 Scoring Model (Expanded)

ADR v4 is built from five forces:

Relevance
How well the business matches the core intent of real-world queries.

Velocity
Freshness and speed of updates across listings, reviews, content, and citations.

Novelty
Differentiation compared to local competitors and directories.

Impact
Strength of citations, listings, reviews, profiles, and content.

Forecast Confidence
How predictable and stable the entity’s identity and behavior appear.

These forces produce a normalized 0–100 output.

ADR v4 is not a linear equation — velocity and contradictions apply multipliers and penalties after base scoring.

B. Velocity & Decay Curve

Velocity follows a simplified decay pattern:

0–18 hours: Full strength (1.5x multiplier)

18–72 hours: Partial strength (1.15x multiplier)

3–30 days: Minimal influence (1.0x baseline)

30–90 days: Weak influence (0.6x multiplier)

90+ days: Negligible influence

Bursts outperform drips.
Freshness outperforms history.

C. Contradiction Penalty Model

A contradiction is any mismatch between:

website vs. listings

services vs. reviews

schema vs. content

address or region mismatches

category confusion

photo evidence vs. claimed identity

Penalties:

Minor contradiction: −5 ADR

Moderate contradiction: −10 to −20 ADR

Major contradiction: −25+ ADR

Critical contradiction: AI may exclude the entity entirely

Contradiction penalties apply before the final ADR output.

D. Dominant Noun Pattern Examples

Noun patterns drive category rewrites.

Example 1 — Generator Installer

Reviews: “generator,” “install,” “backup power”
Photos: generator units
GBP products: “standby generators”
AI category rewrite: Standby Generator Specialist

Example 2 — Water Heater Specialist

Reviews: “water heater,” “tankless,” “replace”
Photos: water heater units
Content: install guides
AI rewrite: Water Heater Specialist

E. Category Cluster Formation

A category cluster forms when:

multiple content pieces reference the same theme

listings reinforce a common pattern

reviews mention repeated keywords

GBP Products align with the cluster

citations show the same wording

Three clusters in 45 days often trigger an AI rewrite.

F. VER v4 Expanded Factors

VER includes:

Citation strength

Listing completeness

Review footprint

Review distribution & themes

Schema & structured data alignment

Profile consistency

Freshness of activity

Category stability

Content footprint

Overall authority coherence

VER is a confidence score, not a sentiment score.

G. UCA v1.0 Example Fields

For clarity:

velocity_multiplier often ranges from 1.0 to 1.5

contradiction_penalty is typically −5 to −35

noun_pattern is a ranked list

category_clusters identify themes used for rewrites

H. Migration Differences (v1.2 → v4)
Area	v1.2	v4.0
ADR	component list	5-force model, multipliers
VER	evidence rating	confidence matrix
Artifact	DOA	UCA v1.0
Category	listed category	noun-pattern rewrite logic
Velocity	simple recency	full decay curve
Contradictions	minor factor	slashing penalties
Fix-Levers	basic	updated and aligned
END OF APPENDIX

============================================================