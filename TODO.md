# TODO

## Chapter 2: Open Data

### High Priority

**Code examples needed**: The chapter remains entirely conceptual with no demonstrations. The book promises "replicable workflows" but this chapter doesn't show how to actually access any of the sources listed. If this is intentional framing before hands-on work in climate risk chapters, add a signpost like: "The following chapters demonstrate these concepts through concrete examples—accessing Copernicus climate data, querying OSM infrastructure, and combining multiple sources for risk analysis."

**Connection to Chapter 3 unclear**: This chapter lists generic repositories but doesn't preview what specific climate datasets they contain. Does Chapter 3 pull datasets from the sources listed here (GEE, Planetary Computer, etc.)? If so, add forward reference: "In Chapter 3, we'll use [specific datasets] from these repositories to assess [specific hazards]." If not, explain how open data concepts here relate to climate risk data there.

### Medium Priority

**Transition logic**: The flow from "how to find data" (Chapter 2) to "climate risk fundamentals" (Chapter 3) needs clearer bridging. Does Chapter 3 start with data discovery, or does it assume readers already have datasets identified? A sentence or two clarifying this would help readers understand the narrative arc.

## Chapter 3: Climate Risk Fundamentals

### Critical Priority

**Risk calculation methodology missing**: Lines 163-165 contain only a placeholder for how to actually calculate risk from the three components. This is the most fundamental operation readers need to perform. The cookbook chapters will demonstrate this with real data, but this section needs at least conceptual guidance: additive vs multiplicative approaches, normalization strategies, handling categorical vs continuous data, and what the output means (relative risk scores vs absolute probabilities).

**Hazard sections empty**: Urban flooding (lines 203-205), heat waves (207-209), intense storms (211-213), and sea level rise (215-217) are all TODO placeholders. These are the primary hazards facing cities. Each needs at least a paragraph defining the hazard, explaining why it's particularly relevant to urban contexts, and previewing what data is used to assess it. The cookbooks will show workflows, but readers need conceptual grounding here.

**Critical infrastructure placeholder**: Lines 197-199 flag this for cookbook treatment, but the fundamentals chapter should at least define what qualifies as critical infrastructure (water, power, hospitals, emergency services, transportation nodes) and why climate impacts on this infrastructure matter differently than impacts on general buildings.

### High Priority

**Data source specifics missing**: The chapter references GFDRR's compendium (lines 136-137) and global population datasets (GHSL, WorldPop at lines 52-53), but doesn't explain how to access them or what format they're in. Given Chapter 2's emphasis on cloud-native formats and data infrastructure, Chapter 3 should at least mention whether these hazard and exposure datasets are available via STAC, as cloud-optimized files, or through other access methods. This connects the abstract "open data" concepts to concrete climate datasets.

**"Use multiple methods" needs examples**: Lines 34 and 65 recommend using multiple approaches to measure exposure, but don't show what this looks like in practice. How do you combine census data with building footprints? What do you do when WorldPop and GHSL disagree? The cookbook will demonstrate this, but a concrete preview example would help readers understand the strategy.

**GFDRR guidance needs synthesis**: Lines 136-151 refer extensively to GFDRR's hazard dataset guidance but don't synthesize the key takeaways. What are the 2-3 most important questions from that list that a municipal user should always ask? This would make the guidance more actionable without requiring readers to independently digest GFDRR's full documentation.

**Connection to Chapters 1 & 2**: The chapter doesn't reference back to Chapter 1's La Plata example (which used Copernicus DEM, MapBiomas, and ARBA data) or forward to specific datasets from Chapter 2's repositories. Adding 2-3 sentences like "In Chapter 1, we used [X] as hazard data and [Y] as exposure data—that's an example of combining the three risk components" would anchor abstract concepts in concrete work readers have already seen.

### Medium Priority (Completed)

**Urban characteristics that increase risk**: Added comprehensive section covering impervious surfaces, drainage infrastructure, density, informal settlements, heat island effect, and aging infrastructure (lines 179-195).

**Climate change connection**: Added section explaining how climate change alters hazard profiles and the need for scenario-based planning rather than relying solely on historical data (lines 167-175).

**Gray vs green infrastructure distinction**: Expanded structural interventions section with clear definitions, examples, and hybrid approaches (lines 248-251).

### Notes

Many of the critical and high priority gaps are intentionally deferred to cookbook chapters, which will demonstrate actual workflows for flooding risk assessment, heat vulnerability mapping, and informal settlement exposure analysis. The fundamentals chapter provides conceptual grounding; the cookbooks will show the mechanics.
