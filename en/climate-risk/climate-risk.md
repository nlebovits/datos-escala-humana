## Climate Risk for Cities

### Objectives

Understand the key concepts of exposure, vulnerability, hazard, risk, resilience, mitigation, and adaptation. Learn how to measure these concepts with data: approaches, relevant examples, and limitations of quantitative measurement.

### What is Climate Risk?

Climate risk is composed of three elements: exposure, vulnerability, and hazard.

You can think of risk as the intersection of three layers. Crossing these three layers allows you to generate areas of maximum risk, risk according to different scenarios, prioritization of resources for mitigation and adaptation, and quantification of probable losses (economic or otherwise).

Risk is complicated and multidimensional. You can have areas of high exposure (high population) but not super high risk because they are wealthy, like Puerto Madero in Buenos Aires or parts of Miami. Even within the same city like Miami, there are parts with much higher risk than others, even though they have relatively similar exposure and hazard, simply because they have different levels of vulnerability.

You have other places with lower population but very high vulnerabilities that can have high risk.

### Key Risk Indicators

- Total exposed population
- Total population in poverty conditions that is exposed
- Exposed critical infrastructure
- Exposed economic value
- Highest risk areas
- Areas that are growing toward higher risk zones

### Importance of Scale

The scale at which we measure has an impact on how we understand risk. There is a big difference between measuring at the census tract level versus at the 100-meter cell level versus at the building level.

Each has pros and cons in terms of the understanding it gives us of space. For example, a census tract assumes that population is distributed uniformly across a fairly large area, which is almost never true. In fact, we know from research that even assuming population is distributed uniformly across a 100-meter square pixel misrepresents exposure to flood hazard. [TODO: add link to paper]

On the other hand, building footprints, especially if they don't have associated height or use, are very difficult to use to estimate total population because you don't know if a building is one story or seven stories, residential or not.

What I recommend doing is using multiple methods (building footprints, raster, census data) to try to better estimate risk.

## Exposure

### Definition

According to UNDRR [TODO: add original citation]: The situation of people, infrastructure, housing, productive capacities, and other tangible human activities located in disaster-prone areas.

Population is the typical way we measure this in climate risk for cities, although also built environment, agriculture, etc.

### Ways to Measure Exposure

**Census data**

In Argentina, this is often done with the 2022 Argentine Census.

**Global population raster data**

- Global Human Settlement Layer (GHSL) 2025: 100-meter resolution
- WorldPop 2025: 100-meter resolution

**Building footprints**

Global building footprint data like those from Overture Maps Foundation.

**Land cover maps**

Like MapBiomas 2022 data for Argentina.

### Recommended Approach

Each of these is appropriate under various conditions. What I generally recommend doing is taking multiple approaches and presenting a range.

There are several reasons to do this. Mainly, the scale at which we do this really matters. The scale at which we measure has an impact on how we understand it.

### Infrastructure Data

Infrastructure data is typically better at local or national level. But there are global datasets like OpenStreetMap, which should be used with caution, but in the absence of other data can be effective. Or Overture Maps Foundation.

## Vulnerability

### Definition

According to UNDRR [TODO: add original 2019 citation]: The conditions determined by physical, social, economic, or environmental factors or processes that increase the vulnerability of a person, community, well-being, or systems to hazards.

GFDRR says: Socioeconomic conditions describe the susceptibility of different categories of people exposed to hazards.

Basically, poor people have more risk than wealthy people, but there can be other factors like age, race, health that can all influence vulnerability.

### Vulnerability Factors

These manifest differently. They are not identical: wealth, race, age, ethnicity are not perfectly correlated. It is important to consider these different factors.

However, these factors are often highly correlated. For example, in the United States we know that race and wealth are extremely correlated. So, by looking at wealth, you also get a fairly good measure of racial difference.

On one hand, it is important to consider these factors separately. On the other hand, in the absence of data, you can basically use wealth as a fairly effective proxy for vulnerability. That is typically what we end up doing at global level because we often don't have very good sociodemographic data outside of a handful of global north countries.

### Focus in This Course

In the absence of better data, wealth is a decent measure. In this particular course, we prioritize clear, transparent, and easily explainable metrics instead of complex tools like the socioeconomic vulnerability index that came out of the United States. So, we tend to prioritize measures like wealth.

### Limitation of Global Data

At global level, there are very few datasets that have socioeconomic vulnerability indicators, apart from the Relative Wealth Index, which again is far from a perfect measure.

These will improve in coming years, surely, but currently there are very few vulnerability indicators. This is another reason why we prioritize local data when available. And when we don't have them, we use the simplest possible metrics because there simply aren't that many.

## Hazard

### Definition

Any process or phenomenon that can cause loss of human life, injury, or other health impacts, property damage, social hazards, or economic or environmental degradation.

Hazard can be of natural, anthropogenic, or socionatural origin.

We are talking about things like flooding, drought, rain, heat waves, rising temperatures, sea level rise, glacial retreat, desertification, etc.

### Types of Hazard Data

**Deterministic Data**

Based on statistical indices like median, maximum, and mean. They are derived from historical events or reanalysis data to estimate hazard intensity. These come from historical events.

**Probabilistic Data**

Use simulations to generate different possible scenarios of hazard intensity, each associated with a different return period or occurrence. They account for uncertainty and frequency.

Probabilistic data often incorporate measures of deterministic data, but we are talking about two different things:

- Deterministic data are based exclusively on historical events
- Probabilistic data account for simulations and modeling

This is really important to keep in mind.

### Limitations of Historical vs Probabilistic Data

Historical data describe the past, but do not speak to future events.

Probabilistic data speak to future events based on scientific evidence. They reproduce physical processes and statistical distributions of events. In this way, probabilistic models can overcome the limitations of historical records to generate multiple possible synthetic scenarios that simulate possible future intensity.

### Data Sources

The Global Facility for Disaster Risk Reduction (GFDRR) offers an excellent compendium of the best global hazard datasets. Along with very good explanations of how to use them and what the strengths and weaknesses of each of these datasets are.

They do a very good job explaining the importance of being aware of the different ways to use this data. For example, resolution makes a big difference and you need to compare multiple datasets.

### Important Questions When Working with Climate Data

When you work with climate data, ask yourself:

- Is this data deterministic or probabilistic?
- What is the resolution?
- What is the time period?
- What is the return period?
- How does this data take uncertainty into consideration?
- Am I using this data according to the way it was supposed to be used?
- Are there local factors not represented in these global datasets, like flood defenses?
- How am I going to validate this data in some way?

### Important Warning

As GFDRR notes: when we talk about natural hazards, misinformation can be as bad or worse than lack of information. It is really important to make sure we are representing data accurately and reusing it responsibly.

## Risk

### Combining Factors to Obtain Impact

Risk is the intersection of exposure, vulnerability, and hazard.

### Risk Calculation

[TODO: Expand this section]

## Climate Change and Disaster Risk

Climate change alters the frequency, intensity, and spatial distribution of climate hazards. Hazards that historically occurred rarely now occur more frequently. Events that were considered extreme become more common. Areas that were previously safe become exposed.

For cities, this means that historical data alone is insufficient for planning. A 100-year flood based on historical records may now be a 50-year or 25-year event. Heat waves that occurred once per decade may now occur multiple times per year. Infrastructure designed for historical climate conditions faces conditions it was not built to handle.

Probabilistic modeling that incorporates climate projections helps address this limitation by simulating future scenarios. However, climate projections carry uncertainty—different models project different magnitudes of change, and local effects are harder to predict than global trends. This uncertainty doesn't eliminate the value of projections; it means we need to work with scenarios and ranges rather than single predictions.

For practical municipal planning, this typically means: use historical data to understand what has happened, use climate projections to understand the direction and approximate magnitude of change, and design interventions that are robust across a range of possible futures rather than optimized for a single prediction.

## Specific Effects in Cities

### Urban Characteristics that Increase Risk

Cities concentrate people, infrastructure, and economic activity in relatively small areas, which amplifies climate risk in several ways.

**Impervious surfaces**: Pavement, buildings, and other impervious surfaces prevent water infiltration, increasing runoff during storms and contributing to urban flooding. These surfaces also absorb and retain heat, creating the urban heat island effect where cities are significantly warmer than surrounding rural areas.

**Drainage infrastructure**: Urban drainage systems are designed for historical rainfall patterns. When precipitation intensity increases due to climate change, existing drainage capacity becomes inadequate. Many cities, particularly in the Global South, have incomplete or informal drainage networks that compound flooding risk.

**Density and exposure**: High population density means that a single climate event (flood, heat wave, storm) can affect large numbers of people simultaneously. This concentration increases both the number of people exposed and the complexity of emergency response.

**Informal settlements**: Many cities, especially in Latin America, Africa, and Asia, have substantial populations living in informal settlements. These areas typically occupy marginal land (floodplains, steep slopes, areas without formal drainage), have lower-quality housing that is more vulnerable to climate impacts, and lack basic infrastructure like stormwater management or cooling systems.

**Heat island effect**: Urban areas are typically 1-3°C warmer than surrounding rural areas due to heat absorption by buildings and pavement, lack of vegetation, and waste heat from vehicles and air conditioning. During heat waves, this effect intensifies, creating dangerous conditions for populations without access to cooling.

**Aging infrastructure**: Many cities rely on water, sewage, and electrical infrastructure built decades ago for different climate conditions and smaller populations. This infrastructure faces increased stress from more frequent extreme events.

Understanding these urban characteristics helps identify where interventions are most needed and what types of interventions are appropriate. Green infrastructure addresses multiple issues (heat, flooding, air quality). Informal settlement upgrading reduces vulnerability. Drainage improvements reduce flood risk. Each intervention targets specific urban characteristics that increase climate risk.

### Critical Infrastructure

[TODO: Expand this section - will be demonstrated in cookbooks]

## Common Types of Hazards for Cities

### Urban Flooding

[TODO: Expand this section]

### Heat Waves

[TODO: Expand this section]

### Intense Storms

[TODO: Expand this section]

### Sea Level Rise

[TODO: Expand this section]

## Resilience, Mitigation, and Adaptation

### Resilience

The capacity of a system, community, or society exposed to hazards to resist, absorb, adapt, transform, and recover from the effects of a hazard in a timely and efficient manner, including the preservation and restoration of its basic structures and functions through risk management.

Source: UNDRR [TODO: add original citation]

### Mitigation

Interventions to reduce emissions, reduce the effect of greenhouse gases, or increase their capture, reducing the effect or magnitude of climate change.

**Important**: Most of what we discuss in this course is adaptation, not mitigation. Unless you are talking about reducing emissions, you are not talking about mitigation. You are talking about adaptation.

### Adaptation

Changes to natural or human systems in response to current climate or anticipated climate and its effects to reduce risk and take advantage of opportunities.

Example: floating houses in the Netherlands.

### Adaptation Approaches

**Structural Interventions**

According to UNDRR: Physical constructions to avoid possible impacts or hazards. The application of engineering techniques or technology to achieve resistance or resilience against hazards in structures or systems.

Examples:

- Channels or other hydroengineering
- Gray infrastructure: Built infrastructure like concrete channels, flood walls, levees, and drainage pipes. Effective for controlling water flow but can be expensive to build and maintain, may transfer risk downstream, and doesn't address multiple co-benefits.
- Green infrastructure: Nature-based solutions like wetlands, permeable surfaces, urban forests, and rain gardens. Can address multiple issues simultaneously (flood management, heat reduction, air quality, biodiversity) and typically costs less to maintain than gray infrastructure, though may require more space and longer time to establish.

Many effective adaptation strategies combine gray and green infrastructure. For example, a drainage system (gray) supplemented with bioswales and rain gardens (green) that capture and infiltrate stormwater before it enters the drainage network.

**Non-Structural Approaches**

UNDRR definition: Approaches that do not involve physical construction and that use knowledge, practices, or agreements to reduce risks or disaster impacts, particularly through policies and laws, public education, capacity building, and education.

Examples:

- Flood early warning system
- Risk reduction plan
- Fire reduction plan
- Flood hazard zone where new structures are not permitted to be built
