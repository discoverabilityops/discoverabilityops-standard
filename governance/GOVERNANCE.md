# Governance Model — DiscoverabilityOps Standard

This document describes how the DiscoverabilityOps Standard is maintained, updated, and evolved.

------------------------------------------------------------
## Stewardship

The standard is maintained by **DiscoverabilityOps**.

While community contributions are welcomed,  
final editorial authority remains with the maintainers.

------------------------------------------------------------
## Principles

1. **Openness**  
   The standard is free to read, implement, and extend.

2. **Practicality**  
   Recommendations focus on real-world use by SMBs, agencies, and product teams.

3. **Transparency**  
   All changes appear in `CHANGELOG.md` and the GitHub issue history.

4. **Interoperability**  
   Implementations should be compatible with the DOA schema and core metrics.

------------------------------------------------------------
## Change Process

### **1. Proposal**
Changes begin as:
- GitHub Issues, or
- Draft Pull Requests

Proposals must:
- Define the problem  
- Explain why a change is needed  
- Provide clear examples or alternatives  

### **2. Discussion**
Discussion happens via:
- Issue comments  
- PR comments  
- Maintainer notes (when required)

### **3. Decision**
Maintainers decide to:
- Accept  
- Modify  
- Request more detail  
- Reject  

Accepted changes:
- are merged into `main`
- are documented in `CHANGELOG.md`
- appear in the next tagged version

------------------------------------------------------------
## Versioning

The standard follows semantic versioning:

- **MAJOR** — Breaking conceptual changes  
- **MINOR** — New examples, clarifications  
- **PATCH** — Editorial fixes  

The current version is found in `VERSION`.

------------------------------------------------------------
## Extensions and Vendor Implementations

Vendors may:
- Extend the standard  
- Add custom fields  
- Build proprietary scoring models  

To remain DiscoverabilityOps-compatible:
- Standard fields must remain intact  
- Custom fields should be namespaced  
- ADR must remain a 0–100 normalized score  

------------------------------------------------------------
## Deprecations

Deprecated elements:
- are listed in `CHANGELOG.md`
- remain for at least one MINOR version
- may be removed in the next MAJOR release

------------------------------------------------------------
## Feedback

The standard evolves with:
- field experience  
- community contributions  
- changes in AI model behavior  

Submit feedback via GitHub Issues.
