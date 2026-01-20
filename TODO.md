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

## Chapter 4: From Data to Action

### High Priority

**RDM framework needs resource-constrained guidance**: Lines 86-89 present the four-step robust decision-making framework but don't explain how a three-person planning department in a Global South city actually implements "identify possible future scenarios" or "explore a range of possible solutions." Even a single sentence acknowledging resource constraints would help: "Even with limited capacity, cities can identify 2-3 plausible scenarios (optimistic adaptation, business as usual, delayed action) without sophisticated modeling."

**Ostrich Paradox needs climate-specific application**: Lines 114-123 mention the six biases and list generic solutions (changing timelines, opt-out defaults, social incentives) but don't connect them to climate adaptation practice. Which biases are most relevant for climate decisions? How do they manifest in municipal planning? For example: "Myopia manifests when councils prioritize immediate infrastructure repairs over flood protection because benefits are visible now. Counter this by quantifying near-term co-benefits: green infrastructure reduces flooding but also provides immediate amenities."

**Disconnect between RDM framework and political realities**: The "Data in the Real World" section (lines 137-167) provides excellent guidance on working with politicians but doesn't connect to the robust decision-making framework presented earlier. Adaptive pathways are politically valuable precisely because they defer expensive commitments and preserve flexibility—this connection should be made explicit.

### Medium Priority

**Workshop preview unclear**: Line 173 references the Esperanza workshop integrating chapter concepts but doesn't preview what the workshop demonstrates. One sentence like "The Esperanza workshop demonstrates this framework by [brief description]" would show readers where they're headed.

**Learn More section needs annotations**: Lines 176-182 list excellent sources but don't guide readers on what each provides. Is the Climate Resilience Toolkit for technical uncertainty analysis? Is Meyer & Kunreuther for behavioral interventions? Brief annotations would help practitioners know where to go next.

**Structural connections between sections**: The chapter moves from uncertainty concepts to decision frameworks to behavioral barriers to political communication, but the connections between sections are weak. The robust decision-making framework doesn't explicitly reference the uncertainty types. The Ostrich Paradox discussion doesn't connect to the RDM framework. The sections feel like separate topics rather than building toward a unified argument.

**Resource-constrained example needed**: The Netherlands case study (lines 91-102) is the only worked example, and it reinforces that RDM is for well-resourced contexts. Adding one resource-constrained example would balance this. Even a paragraph: "In [city], planners used this approach with three staff and no consultants by..."

### Medium Priority (Completed)

**Non-stationarity implications**: Added sentence connecting non-stationarity to infrastructure planning—historical 100-year floods may occur more or less frequently in the future depending on local climate change effects (line 41).

**Social uncertainty implications**: Added sentence explaining that adaptation strategies should avoid rigid assumptions about future demographics, economic conditions, or technological capabilities (line 57).

**Four principles for planners**: Added complete four principles from Meyer & Kunreuther (2019) with brief explanations for each principle (lines 127-135).

**Reference added**: Added Meyer & Kunreuther (2019) Ostrich Paradox issue brief to references.bib with proper citation in text.
