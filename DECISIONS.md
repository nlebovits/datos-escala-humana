# Project Decisions

This document records significant decisions made during the development of Human Scale Data.

## Decision Template

When adding a new decision, use this format:

```markdown
## [Decision Title] - YYYY-MM-DD

**Context:** What situation prompted this decision?

**Decision:** What did we decide?

**Rationale:** Why did we make this choice?

**Consequences:** What are the implications of this decision?
```

---

## No Appendix with Definitions - 2026-01-28

**Context:** Educational materials often include appendices with definitions of technical terms used throughout the content.

**Decision:** We will not create an appendix with definitions for technical terms.

**Rationale:** Readers can easily search for unfamiliar terms using search engines or AI assistants. The effort required to maintain a comprehensive, accurate definitions appendix does not justify the return on investment, especially given the rapid evolution of terminology in data science and geospatial fields.

**Consequences:** Readers encountering unfamiliar terms will need to look them up independently. This keeps the content focused and reduces maintenance burden.

## Data Reproducibility - 2026-02-11

**Context:** Chapters load datasets from local copies and remote URLs. External users cloning the repo need access to these files.

**Decision:** Enforce reproducibility via two patterns:

1. **Local files**: Commit to git via LFS with a citation in references.bib
2. **Cloud-accessed data**: Keep remote URLs as-is; add CI workflow to detect broken links

**Rationale:** Local files ensure immediate reproducibility. Cloud URLs are generally stable; CI catches drift without duplicating large hosted datasets.

**Consequences:** All new datasets must follow this pattern. LFS increases repo size for local files. CI will alert when remote sources change.
