# Canon: Core Terminology

**Status:** Draft for scientific review  
**Review status:** Pending formal WFI scientific review  
**Review record:** Tracked through the WFI canon review workflow  
**Canonical source type:** Human-readable WFF terminology canon draft  
**Last updated:** 2026-05-15  
**Machine-readable definitions:** `glossary/wff_terms.yaml`  
**Deprecated terms:** `glossary/deprecated_terms.yaml`  
**Source registry:** `sources/source_registry.yaml`

This file defines core Welfare Footprint Framework (WFF) terms for human readers. Terms are grouped by conceptual role and by analytical module. The definitions are intended to preserve the WFF analytical chain:

`Circumstances → Biological Consequences → Affective Experiences → Welfare Metrics`

These levels are distinct and must not be conflated. Circumstances describe the internal and external conditions animals face; Biological Consequences describe organism-level physiological, anatomical, neurological, perceptual, or cognitive changes; Affective Experiences describe consciously felt states; Welfare Metrics express cumulative welfare impacts in standardized quantitative form.

**Citation convention:** This file uses source IDs from `sources/source_registry.yaml`, not full bibliographic citations. Full citations should remain in the source registry. When a source is not yet registered, the term should be marked as requiring source-registry update before final merge.

**Primary source basis:** `wff-methodological-foundations-2025`, `wfi-technical-definitions`

---

## 1. Core Framework Terms

**Default source basis for this section:** `wff-methodological-foundations-2025`, `wfi-technical-definitions`, `wfi-metrics-vs-indicators-2023`

### Welfare

All negative and positive affective states experienced over a period of interest.

### Welfare Footprint Framework (WFF)

A scientific methodology for quantifying animal welfare and estimating welfare impacts by measuring the intensity, duration, and population-level distribution of animals’ negative and positive Affective Experiences.

The framework comprises six core analytical modules and one optional interspecific module:

1. Module I — Zootechnical Description
2. Module II — Veterinary Inventory
3. Module III — Affective Quantification
4. Module IV — Epidemiological Review
5. Module V — Econometric Calculation
6. Module VI — Welfare Footprint Expression and Notation
7. Module Ψ — Interspecific Scaling / Interspecific Affect

Across all analyses, the WFF preserves the causal chain `Circumstances → Biological Consequences → Affective Experiences → Welfare Metrics`, distinguishing the conditions animals face, the biological or perceptual consequences those conditions produce, the consciously felt states that result, and the standardized metrics used to express their cumulative welfare impact.

### Welfare Footprint

A quantitative measurement of the impact that actions, practices, products, interventions, policies, or broader processes have on animal welfare. In the WFF, this impact is assessed by estimating the time animals spend in negative and positive Affective States of different intensities.

A Welfare Footprint incorporates three core dimensions of lived experience:

1. **Intensity** — how unpleasant or pleasant each Affective Experience is;
2. **Duration** — how long each experience lasts;
3. **Prevalence or population distribution** — what proportion of animals experience it, and how the experience is distributed across the Target Population.

Results are expressed as Cumulative Pain and Cumulative Pleasure, disaggregated by intensity category. They may be standardized per individual, per population, per unit of product such as kg of meat, liter of milk, or dozen eggs, per dollar spent, or per other decision-relevant denominator.

### Welfare Assessment — Guiding Principle

The guiding principle underlying WFF welfare assessments is a primary focus on the measurement of Affective Experiences. Health, biological function, and natural living are relevant within the framework to the extent that they influence, or are expected to influence, the subjective negative or positive Affective Experiences of individuals.

Subclinical health conditions, growth impairment, physical disabilities, or deprivations of resources or natural behaviors are not treated as welfare impacts in themselves unless they are associated with some form of unpleasantness, loss of positive experience, or other affective consequence over the period of interest.

### Welfare Indicator

A discernible trait, signal, or condition that, based on evidence, is correlated to a greater or lesser degree with an individual’s Affective Experience or Affective State. Welfare Indicators are not Welfare Metrics: they are pieces of evidence used to inform inferences about welfare, rather than standardized quantitative constructs for comparing welfare impacts.

Welfare Indicators may be animal-based or resource-based, and can include neurological, physiological, behavioral, environmental, pharmacological, immune, anatomical, and management-related factors.

### Welfare Metric

A quantitative construct used to evaluate and compare animal welfare across situations, populations, interventions, systems, or time periods. Welfare Metrics are informed by Welfare Indicators but are distinct from them: indicators are traits, signals, conditions, or measurements used as evidence about Affective Experiences, whereas metrics are standardized quantitative constructs used to express welfare impacts.

In the WFF, the primary Welfare Metrics are Cumulative Pain and Cumulative Pleasure, which estimate time spent in negative and positive Affective States of different intensities. These metrics can then be standardized per individual, population, unit of product, dollar spent, or other decision-relevant denominator to express a Welfare Footprint.

---

## 2. Cross-Cutting Concepts for WFF Assessments

**Default source basis for this section:** `wff-methodological-foundations-2025`, `wfi-technical-definitions`

### Analytical Boundaries

The defined scope of a Welfare Footprint assessment, specifying the Species, System or Production System, Life-Fates, Life-Phases, Circumstances, Affective Experiences, Target Population, geography, timeframe, and level of analysis included.

Analytical Boundaries must be defined before estimates are interpreted or compared. Estimates from assessments with different Analytical Boundaries are not directly comparable unless the differences are explicitly reconciled.

### Plausible Scenario

A structured set of assumptions or parameter values used to represent welfare impacts that are plausible given current knowledge of the System, Target Population, Analytical Boundaries, and evidence base. Plausible Scenarios are used when relevant inputs are uncertain, heterogeneous, incompletely observed, context-dependent, or contested.

Plausible Scenarios are not abstract best-case or worst-case bounds. They should be grounded in what is known about real operating conditions, biological mechanisms, analogous systems, expert judgment, or other relevant evidence.

### Sensitivity Analysis

A procedure for testing how WFF estimates and conclusions change across Plausible Scenarios and uncertain parameter values. Sensitivity Analysis may be applied to any parameter in the framework, including Circumstances, Biological Consequence severity, Affective Experience intensity, duration, prevalence, occurrence, Affective Episode Rate, Productivity Metrics, Life-Fate accounting, allocation assumptions, or interspecific scaling assumptions.

Its purpose is not to replace missing data, but to reveal whether missing or uncertain data matter for the conclusion at hand. If a conclusion holds across the relevant range of plausible values, it is robust to that source of uncertainty. If it does not, Sensitivity Analysis identifies which parameters most strongly influence the result and where additional empirical work would be most consequential.

### Traceability

The preservation of the full analytical pathway linking a Welfare Footprint estimate back to its underlying evidence, assumptions, parameters, and intermediate calculations.

Traceability requires that estimates remain linked, in auditable form, to their underlying Species, System or Production System, Life-Fates, Life-Phases, Circumstances, Biological Consequences, Affective Experiences, Target Populations, prevalence estimates, occurrence estimates, Affective Episode Rates, intensity estimates, duration estimates, Productivity Metrics, accounting procedures, allocation assumptions, standardization denominators, and uncertainty ranges.

In digital implementations, such as the Welfare Footprint Atlas, Traceability should be treated as a core design principle. The system should preserve the chain:

`Circumstances → Biological Consequences → Affective Experiences → Affective Quantification → Epidemiological Estimates → Econometric Calculation → Welfare Footprint Expression`

while allowing each final estimate to be decomposed back into its component assumptions, evidence sources, and calculation steps.

### Provenance

The structured record of the origin, authorship, evidence basis, version, timestamp, review status, and analytical context of a WFF object, parameter, assumption, or estimate.

Provenance is distinct from, but required for, Traceability. Traceability preserves the analytical pathway linking final estimates to their components; Provenance records where those components came from and how they have been created, modified, reviewed, accepted, superseded, or deprecated.

### Scope Qualifier

An explicit label appended to a Cumulative Pain, Cumulative Pleasure, or Cumulative Affect estimate that specifies the analytical level and time period to which the estimate applies. A Scope Qualifier is required because estimates with different Analytical Boundaries are not directly comparable.

Examples include:

- `Cumulative Pain [Episode]`
- `Cumulative Pleasure [Life-Phase]`
- `Cumulative Pain [Lifespan]`
- `Cumulative Pleasure [per liter of milk]`
- `Cumulative Pain [per kg of meat]`

### Cumulative Affect [Baseline]

The default form of Cumulative Affect estimation, in which each Affective Experience is analyzed independently and results are accounted for across experiences while preserving disaggregation by valence and intensity category.

Cumulative Affect [Baseline] should be interpreted as a transparent default accounting estimate, not necessarily as a precise estimate of what the animal is consciously attending to at every moment when multiple Affective Experiences occur concurrently.

### Cumulative Affect [Attention-Adjusted]

An optional post-quantification refinement of Cumulative Affect that accounts for competition between concurrent Affective States for limited attentional resources. More intense Affective States may capture a greater share of attention, potentially diminishing or blocking awareness of weaker concurrent states.

Applying this adjustment requires evidence about comorbidity patterns, the frequency with which specific Affective Experiences co-occur, and the attentional demand of different intensity levels. When used, the assumptions and data supporting the adjustment must be reported explicitly.

---

## 3. Module I: Zootechnical Description

**Default source basis for this section:** `wff-methodological-foundations-2025`, `wfi-technical-definitions`

### Species

The sentient species under examination in a given WFF assessment.

### System and Production System

The living context in which the population of interest exists. **System** is the broader term and may include farming systems, zoos, sanctuaries, laboratories, natural habitats, or socio-economic environments. **Production System** refers specifically to systems in which animals are bred, raised, kept, or used for productive purposes.

### Life-Fate

A category of individuals within a species or system that share a sufficiently similar life trajectory, defined by commonalities in their roles, exposures, critical life events, hazards, and welfare-relevant outcomes. Different Life-Fates within the same System or Production System are assessed separately when their Circumstances, Life-Phases, Biological Consequences, or Affective Experiences differ in welfare-relevant ways.

### Life-Phase

A major biological or operational stage within a given Life-Fate, characterized by distinct Circumstances, exposures, challenges, and welfare implications. Life-Phases are defined separately for each Life-Fate and provide the temporal structure for describing Circumstances and identifying Biological Consequences.

### Circumstance

The internal and external conditions that shape an animal’s life during each Life-Phase. **External Circumstances** include physical, social, environmental, procedural, and management-related conditions, such as housing design, space allowance, resource availability, social configuration, lighting schedule, enrichment access, feeding regime, and handling method. **Internal Circumstances** include animal attributes that shape vulnerability, response, or exposure, such as breed, line, genotype, sex, age, developmental status, and genetic predispositions.

**Critical distinction — Circumstances vs. Biological Consequences:** Circumstances do not directly constitute Affective Experiences. They influence welfare through the Biological Consequences they generate, modulate, or make more likely. For example, high stocking density, poor flooring, or a genetic predisposition are Circumstances; joint damage, skin lesions, impaired thermoregulation, or perceived lack of agency are Biological Consequences. Genetic predispositions and other animal attributes should therefore be treated as Circumstances when they shape vulnerability or response, not as Biological Consequences themselves.

### Species-Specific Needs

The nutritional, environmental, health-related, behavioral, social, and psychological requirements of a species or class of animals that shape how Circumstances are likely to affect them. Species-Specific Needs provide the reference against which Circumstances are interpreted: the same Circumstance may have different Biological Consequences depending on the needs, capacities, life stage, and phenotype of the animals involved.

Frameworks such as the Five Domains can help organize the identification of these needs. In the WFF, however, Species-Specific Needs are welfare-relevant to the extent that meeting or failing to meet them influences Affective Experiences.

### Productivity Metrics

The commercial output variables associated with the system under analysis that are needed to express welfare estimates per unit of commercial output. Examples include kilograms of meat, liters of milk, number or mass of eggs, live weight sold, carcass weight, or other commercially significant animal-derived outputs over a defined production period or cycle. Productivity Metrics are recorded in Module I because they are needed in Module V to express cumulative affective estimates per unit of commercial output.

Module I records population accounting separately from Productivity Metrics. Population accounting identifies the numbers or proportions of animals represented by each Life-Fate and, where needed, their movement through Life-Phases; it supports construction of the cumulative welfare-burden numerator. Life-Fates are pragmatic analytical partitions intended to capture the numerically significant and welfare-relevant portions of the population first. Residual animals or pathways not represented by the current Life-Fate partition should be recorded explicitly, with estimated percentage or count where available, or marked as unknown for later refinement.

Productivity Metrics are commercial output-denominator variables, such as eggs per year, kg liveweight sold, kg carcass, kg edible meat, kg retail cuts, litres milk, or kg processed product when processing is inside the analytical boundary. These support denominator selection for later Module V standardisation. Module I records candidate denominators; Module V determines allocation rules and performs standardisation.

### Processogram

A spatiotemporal process diagram that conveys a time-ordered description of the typical life stages, production phases, and welfare-relevant Circumstances experienced by a Life-Fate within a System or Production System. In a Processogram, spatial components are represented, where possible, in realistic proportion to real-life conditions and arranged along a horizontal time axis representing the passage of time.

**Source-registry note:** The Processogram source should be added to `sources/source_registry.yaml` before this term is treated as fully source-resolved.

---

## 4. Module II: Veterinary Inventory

**Default source basis for this section:** `wff-methodological-foundations-2025`, `wfi-technical-definitions`

Module II identifies the Biological Consequences arising from Circumstances and maps the Affective Experiences expected to emerge from those consequences. It therefore functions as the bridge between the description of living conditions in Module I and the quantification of felt experiences in Module III.

### Biological Consequence

A physiological, anatomical, neurological, perceptual, or cognitive change resulting from an organism’s exposure to internal or external Circumstances, or generated or modulated by prior Affective Experiences. Biological Consequences include physical manifestations, such as wounds, inflammation, lesions, disease processes, metabolic imbalances, dehydration, or malnutrition, as well as perceptual or cognitive states, such as detecting a threat, perceiving novelty, recognizing the absence of conspecifics, or perceiving lack of agency.

Biological Consequences are organism-level responses that may act as proximate precursors to Affective Experiences. They are not themselves the welfare endpoint quantified by the WFF unless they are consciously felt. Some Biological Consequences may be subclinical or intermediate, mattering only because they increase the likelihood, intensity, duration, recurrence, or complexity of downstream Affective Experiences.

### Physical Consequence Leading to Negative Affective Experiences

A physical Biological Consequence involving detrimental anatomical, physiological, neurological, or metabolic change that may give rise to, prolong, intensify, or increase vulnerability to negative Affective Experiences.

Examples include wounds, fractures, inflammation, infection, dehydration, malnutrition, metabolic imbalance, respiratory pathology, or tissue damage.

### Perceptual Consequence Leading to Negative Affective Experiences

A perceptual or cognitive Biological Consequence that may give rise to negative Affective Experiences without necessarily involving physical injury or bodily pathology.

Examples include perception of threat, perception of social isolation, perception of lack of agency, perception of environmental instability, exposure to aversive sensory stimuli, or perception that a highly motivated behavior is blocked or unavailable.

**Notation rule:** Terms for perceptual Biological Consequences should remain sensory, cognitive, or motivational. Emotionally loaded terms, such as “loneliness,” “fear,” “frustration,” or “distress,” should be reserved for the resulting Affective Experience.

### Physical Consequence Leading to Positive Affective Experiences

A physical Biological Consequence or bodily interaction involving restoration, improvement, or favorable change in the animal’s bodily or physiological state that may give rise to positive Affective Experiences.

Examples include ingestion of preferred food, drinking after thirst, relief of physical discomfort, successful thermoregulation, grooming-related tactile stimulation, or copulation.

### Perceptual Consequence Leading to Positive Affective Experiences

A perceptual or cognitive Biological Consequence that may give rise to positive Affective Experiences without necessarily depending on a prior physical deficit.

Examples include perception of safety, recognition of affiliative social partners, perception of environmental opportunity, successful expression of motivated behavior, access to novelty, play opportunities, exploration, or perceived control over the environment.

### Negative Affective Experience

An Affective Experience that is consciously felt as unpleasant. In the WFF, negative Affective Experiences are operationally grouped under **Pain**, broadly understood as any felt negative affective state, whether physical or psychological.

### Positive Affective Experience

An Affective Experience that is consciously felt as pleasant. In the WFF, positive Affective Experiences are operationally grouped under **Pleasure**, broadly understood as any felt positive affective state, whether physical or psychological.

### Affective Experience Mapping

The explicit linking of Circumstances, Biological Consequences, and the Affective Experiences expected to arise from them within the Veterinary Inventory. In Module II, Affective Experiences are identified, named, and linked to their Biological Consequences and Circumstances. Their intensity, duration, temporal segmentation, and cumulative burden are then estimated in Module III: Affective Quantification.

Affective Experiences should be described as specifically as the available evidence allows. Where feasible, they may be described using the structure:

`Affective Experience x due to Biological Consequence(s) y caused or modulated by Circumstance(s) z`

Examples include:

- `Physical Pain from joint inflammation caused by poor flooring and high body weight`
- `Fear from perception of threat caused by rough handling`
- `Frustration from blocked nesting motivation caused by absence of suitable nesting substrate`
- `Comfort from relief of thermal discomfort caused by access to shade or cooling`
- `Joy from affiliative social interaction enabled by compatible social grouping`

### Biological Consequence Pathway

A causal sequence through which one or more Biological Consequences give rise to one or more Affective Experiences. Biological Consequence Pathways may be simple or complex and may differ by severity, temporal course, recurrence, reversibility, treatment status, or outcome.

### Biological Consequence Severity

The magnitude, grade, or clinical scale of a Biological Consequence, defined using observable, clinical, anatomical, physiological, behavioral, or other evidence-based criteria.

Biological Consequence Severity is distinct from the intensity of the resulting Affective Experience. A more severe Biological Consequence may often increase the probability, intensity, duration, recurrence, or complexity of downstream Affective Experiences, but this relationship must be assessed rather than assumed.

### Degree of Deprivation

The extent to which a Circumstance fails to satisfy, partially satisfies, or blocks a Species-Specific Need or motivated behavior during a given Life-Phase. Different degrees of deprivation should be disaggregated when they are expected to produce distinct Biological Consequences or Affective Experiences.

### Degree of Fulfillment

The extent to which a Circumstance satisfies, partially satisfies, or fully satisfies a Species-Specific Need or motivated behavior during a given Life-Phase. Different degrees of fulfillment should be disaggregated when they are expected to produce distinct Biological Consequences or positive Affective Experiences.

---

## 5. Module III: Affective Quantification

**Default source basis for this section:** `wff-methodological-foundations-2025`, `wfi-technical-definitions`, `wfi-pain-intensities`, `wfi-positive-welfare-2024`

### Affective Experience

The complete, dynamic, consciously felt episode resulting from one or more Biological Consequences. Affective Experiences can be negative or positive and are characterized by valence, intensity, duration, and temporal evolution.

In the WFF, Affective Experiences are the welfare endpoints quantified by the framework. They may be described generally as **Pain from...** or **Pleasure from...**, while preserving more specific descriptions when useful.

### Affective State

The specific valence and intensity condition an animal is hypothesized to occupy at a given point or time segment within an Affective Experience. For example, during a negative segment, the animal may occupy states such as Annoying, Hurtful, Disabling, or Excruciating Pain; during a positive segment, it may occupy states such as Satisfaction, Joy, Euphoria, or Bliss.

Although many Affective Experiences are analyzed as predominantly negative or predominantly positive, an Affective Experience may, in some cases, contain temporal segments of different valence. When this occurs, the episode should be segmented accordingly, with negative segments contributing to Cumulative Pain and positive segments contributing to Cumulative Pleasure, while preserving separation by valence and intensity category.

### Temporal Segmentation

The decomposition of an Affective Experience into meaningful time segments, each characterized by a relatively stable hypothesized intensity. Segment boundaries should reflect expected changes in the felt experience, such as changes in the underlying Biological Consequence, behavioral expression, physiological response, treatment status, recovery stage, or external events.

### Pain

In the WFF, **Pain** is used broadly to refer to any felt negative affective state: any consciously experienced state that feels bad. This includes physical Pain, such as aches, hunger, injuries, breathlessness, nausea, thirst, or thermal discomfort, and psychological Pain, such as fear, anxiety, frustration, boredom, sadness, or distress.

The formal scientific definition of Pain may be given separately when needed, but the operational WFF usage should remain clear: Pain is the umbrella term for negative Affective Experiences in the framework.

### Pain Intensity

The estimated degree of unpleasantness, aversiveness, disruption, or attention capture experienced by an individual at a given point or time segment within a negative Affective Experience. Pain Intensity is not inferred directly from the magnitude of the physical stimulus or Biological Consequence; it is a hypothesis about the subjective severity of the felt experience, informed by behavioral, physiological, neurological, pharmacological, anatomical, evolutionary, and other relevant evidence.

The WFF Pain intensity categories, in canonical order, are:

1. **No Pain**
2. **Annoying**
3. **Hurtful**
4. **Disabling**
5. **Excruciating**

The four active negative intensity categories are: **Annoying → Hurtful → Disabling → Excruciating**. **No Pain** denotes periods in which no Pain is hypothesized to be experienced.

Full operational definitions of the Pain intensity categories are maintained in `canon/intensity_categories_pain.md`. PR #3 confirms category names and ordering only; full operational definitions will be populated in Phase 1.4.

**Source basis for Pain intensity categories:** `wfi-pain-intensities`.

### Pain-Track

A notation method for describing a negative Affective Experience according to its temporal evolution. In a Pain-Track, the horizontal axis represents time segments and the vertical axis represents Pain Intensity. For each segment, duration is expressed as a range where appropriate, and intensity may be expressed as a probability distribution across the defined Pain Intensity categories, reflecting uncertainty and biological variation.

### Cumulative Pain

The total estimated time an individual or population spends in negative Affective States of varying intensities over a period of interest. Cumulative Pain is calculated by estimating the duration of each time segment, assigning probabilities or estimates to each Pain Intensity category, and summing time spent within each category across segments.

Cumulative Pain is maintained as a disaggregated metric: time spent in Annoying, Hurtful, Disabling, and Excruciating Pain is reported separately unless an additional analytical layer explicitly applies weighting or transformation assumptions.

### Pleasure

In the WFF, **Pleasure** refers to any felt positive affective state: any consciously experienced state that feels good. Pleasure includes physical and psychological positive experiences, such as comfort, relief, satiety, Satisfaction, Joy, Euphoria, play-related Pleasure, affiliative Pleasure, exploratory Pleasure, and Pleasure from preferred food, grooming, or other rewarding experiences.

**Critical rule:** Pain and Pleasure are not assumed to sit on a simple common scale and are not automatically netted against each other in the WFF. Any attempt to aggregate or trade off Cumulative Pain and Cumulative Pleasure would require explicit additional assumptions and should not be treated as part of the baseline metric.

### Pleasure Intensity

The estimated degree of pleasantness, reward, engagement, or attention capture experienced by an individual at a given point or time segment within a positive Affective Experience. Pleasure Intensity categories are defined primarily by the degree of engagement with the positive experience and the extent to which the experience occupies attention or motivates continued interaction.

The WFF Pleasure intensity categories, in canonical order, are:

1. **No Pleasure**
2. **Satisfaction**
3. **Joy**
4. **Euphoria**
5. **Bliss**

The four active positive intensity categories are: **Satisfaction → Joy → Euphoria → Bliss**. **No Pleasure** denotes periods in which no Pleasure is hypothesized to be experienced.

Full operational definitions of the Pleasure intensity categories are maintained in `canon/intensity_categories_pleasure.md`. PR #3 confirms category names and ordering only; full operational definitions will be populated in Phase 1.4.

**Source basis for Pleasure intensity categories:** `wfi-positive-welfare-2024`.

**Valence rule:** Pain and Pleasure intensity categories are valence-specific and must not be treated as opposite points on a single common scale. Cumulative Pain and Cumulative Pleasure remain disaggregated by intensity category and are not netted against each other. See also the Cumulative Pain, Cumulative Pleasure, and Cumulative Affect entries.

### Pleasure-Track

A notation method for describing a positive Affective Experience according to its temporal evolution, analogous to the Pain-Track. In a Pleasure-Track, the horizontal axis represents time segments and the vertical axis represents Pleasure Intensity. For each segment, duration is expressed as a range where appropriate, and intensity may be expressed as a probability distribution across the defined Pleasure Intensity categories, reflecting uncertainty and biological variation.

### Cumulative Pleasure

The total estimated time an individual or population spends in positive Affective States of varying intensities over a period of interest. Cumulative Pleasure is calculated by estimating the duration of each time segment, assigning probabilities or estimates to each Pleasure Intensity category, and summing time spent within each category across segments.

Cumulative Pleasure is maintained as a disaggregated metric: time spent in Satisfaction, Joy, Euphoria, and Bliss is reported separately unless an additional analytical layer explicitly applies weighting or transformation assumptions.

### Cumulative Affect

An umbrella term for the joint representation of Cumulative Pain and Cumulative Pleasure over a period of interest. Cumulative Affect refers to the full disaggregated profile of estimated time spent in negative and positive Affective States of different intensities.

Cumulative Affect should not be interpreted as a single net welfare score or as a third primary Welfare Metric replacing Cumulative Pain and Cumulative Pleasure. In the baseline WFF, negative and positive affective estimates remain separately represented as Cumulative Pain and Cumulative Pleasure, disaggregated by intensity category.

Cumulative Affect estimates must specify a Scope Qualifier and must explicitly declare the calculation variant used, such as **Cumulative Affect [Baseline]** or **Cumulative Affect [Attention-Adjusted]**.

---

## 6. Module IV: Epidemiological Review

**Default source basis for this section:** `wff-methodological-foundations-2025`, `wfi-technical-definitions`

### Target Population

The specific group of animals to which an epidemiological estimate applies, defined by shared characteristics, Life-Fate, Life-Phase, System or Production System, geography, timeframe, and relevant living conditions.

### Prevalence

The proportion of a Target Population affected by a given Biological Consequence, or by a directly estimated Affective Experience where appropriate, during the analyzed timeframe.

Prevalence should normally be expressed as a range rather than a point estimate, to reflect natural variation across subpopulations and epistemic uncertainty arising from data limitations. Where possible, these sources of uncertainty should be distinguished.

### Occurrence

The number of times an affected animal typically experiences, develops, undergoes, or is exposed to a given Biological Consequence during the analyzed timeframe. Occurrence is distinct from Prevalence: Prevalence estimates how many animals are affected, whereas Occurrence estimates how often affected animals experience the condition, event, or exposure.

### Affective Episode Rate

The expected number of discrete Affective Experiences generated by each occurrence of a Biological Consequence. This parameter is needed because the relationship between Biological Consequences and Affective Experiences is not always one-to-one.

For continuous conditions, the total accumulated duration of the Affective Experience per occurrence or exposure period should be used directly rather than forcing the burden into discrete episodes.

### Population Distribution

The distribution of Biological Consequences and Affective Experiences across the Target Population, including variation by Life-Fate, Life-Phase, subgroup, geography, management condition, severity class, exposure level, or other relevant stratifier.

### Average Population Member

An analytical construct used to estimate the per-capita welfare burden of a Target Population. It represents the expected Cumulative Pain or Cumulative Pleasure assigned to an average member of the population, even when no real individual experiences exactly that profile.

The Average Population Member construct allows welfare burdens to be compared across Biological Consequences, Affective Experiences, Life-Fates, Life-Phases, Systems, and population groups while preserving disaggregation by valence and intensity category.

---

## 7. Module V: Econometric Calculation

**Default source basis for this section:** `wff-methodological-foundations-2025`, `wfi-technical-definitions`

The WFF module in which cumulative affective estimates are related to the productive, population, temporal, or decision-relevant units required by the assessment. In product-focused analyses, this module uses Productivity Metrics recorded in Module I, such as kilograms of meat, liters of milk, number or mass of eggs, carcass yield, or other product outputs over a defined production period, to express Cumulative Pain and Cumulative Pleasure per unit of product.

Econometric Calculation may involve accounting across multiple Life-Fates, Life-Phases, population groups, and Affective Experiences. This accounting must preserve disaggregation by valence and intensity category: Cumulative Pain and Cumulative Pleasure are not netted against each other, and time in different intensity categories is not collapsed into a single weighted score unless an explicit additional weighting or transformation assumption is introduced.

In this context, “econometric” refers broadly to the quantitative linking of welfare estimates to system outputs, population units, time periods, or decision-relevant denominators. It does not necessarily imply monetary valuation, willingness-to-pay estimates, or economic preference modelling.

### Life-Fate Accounting

The process of accounting for Cumulative Pain and Cumulative Pleasure across multiple Life-Fates included within the Analytical Boundaries of the assessment. In product-focused analyses, Life-Fate Accounting allocates the welfare burdens and benefits of different Life-Fates according to their contribution to the production system or product output.

### Welfare Footprint per Unit of Product

The standardized expression of Cumulative Pain and Cumulative Pleasure per unit of animal-derived product, such as per kilogram of meat, liter of milk, egg, dozen eggs, or other defined product unit.

This calculation divides the relevant system-level cumulative affective estimates by the corresponding Productivity Metrics. Where applicable, estimates should account for carcass yield, product yield, pre-slaughter mortality, culling, replacement rates, reproductive output, and losses across the production chain.

Examples include:

- `hours of Disabling Pain per kilogram of meat`
- `hours of Hurtful Pain per liter of milk`
- `hours of Satisfaction per dozen eggs`
- `hours of Excruciating Pain per egg`

### Alternative Denominators

Cumulative Pain and Cumulative Pleasure estimates may also be expressed relative to non-product denominators when these are relevant to the decision context. Examples include estimates per animal, per average population member, per population, per year, per person in a human population, per dollar spent, per intervention, per company, per region, per country, or per unit of GDP.

### Scope and Disaggregation Requirements

Outputs from Econometric Calculation must preserve the Analytical Boundaries and disaggregation required for interpretation. Estimates should identify the denominator used, the level of analysis, and whether the estimate refers to Cumulative Pain, Cumulative Pleasure, or Cumulative Affect.

Econometric Calculation must preserve Traceability. Final standardized estimates should remain linked to the underlying Circumstances, Biological Consequences, Affective Experiences, epidemiological parameters, Productivity Metrics, accounting procedures, allocation assumptions, and standardization denominators used to produce them.

---

## 8. Module VI: Welfare Footprint Expression and Notation

**Default source basis for this section:** `wff-methodological-foundations-2025`, `wfi-technical-definitions`

The WFF module that standardizes the presentation of welfare estimates to ensure interpretability, comparability, transparency, and auditability. Module VI does not create new welfare estimates; it specifies how estimates generated in the previous modules are expressed, labeled, documented, and communicated.

### Welfare Footprint Expression

The structured presentation of Cumulative Pain, Cumulative Pleasure, or Cumulative Affect estimates in a form that identifies what was measured, for whom, over what period or analytical unit, and relative to which denominator.

### Notation Requirements

The formal labeling conventions used to make WFF estimates interpretable and comparable. Every published WFF estimate should include an explicit Scope Qualifier and should identify the relevant unit of expression, such as episode, Life-Phase, lifespan, average population member, population, year, unit of product, or other decision-relevant denominator.

Where Cumulative Affect is reported, the notation must state whether the estimate is **Cumulative Affect [Baseline]** or **Cumulative Affect [Attention-Adjusted]**.

### Disaggregation Requirements

WFF outputs must preserve disaggregation by valence and intensity category. Cumulative Pain should remain disaggregated across Annoying, Hurtful, Disabling, and Excruciating Pain. Cumulative Pleasure should remain disaggregated across Satisfaction, Joy, Euphoria, and Bliss.

Where relevant, results should also remain disaggregated by Affective Experience, Biological Consequence, Circumstance, Life-Fate, Life-Phase, Target Population, population subgroup, geography, timeframe, and denominator.

### Uncertainty Expression

Uncertainty should be expressed transparently in the final presentation of estimates. Depending on the assessment and audience, uncertainty may be represented through ranges, probability distributions, confidence or credibility intervals, scenario-specific outputs, graphical uncertainty bars, or accompanying explanatory notes.

Uncertainty expression should distinguish, where possible, between natural variation, epistemic uncertainty, model assumptions, and scenario-based uncertainty. Final outputs should not present false precision when the evidence base does not support it.

### Supporting Documentation

Published or decision-relevant WFF estimates should be accompanied by the supporting materials needed to inspect, reproduce, update, or challenge the result. These may include Pain-Tracks, Pleasure-Tracks, prevalence estimates, occurrence estimates, Affective Episode Rates, Productivity Metrics, evidence sources, parameter ranges, assumptions, scenario definitions, and sensitivity analyses.

### Communication Formats

WFF results may be communicated in different levels of detail depending on the audience and purpose, including technical reports, regulatory submissions, certification materials, consumer-facing summaries, dashboards, tables, or graphical representations such as double bar charts of Cumulative Pain and Cumulative Pleasure.

Simplified communication formats should not remove distinctions that are necessary for interpretation. In particular, they should not collapse Pain and Pleasure into a single net score, obscure intensity categories, omit Scope Qualifiers, or conceal uncertainty and analytical assumptions.

---

## 9. Module Ψ: Interspecific Scaling / Interspecific Affect

**Status:** Optional module; provisional and under development  
**Default source basis for this section:** `wff-methodological-foundations-2025`, `wfi-technical-definitions`  
**Review note:** Some Module Ψ terms are still under active conceptual development and should remain marked as provisional unless and until source-registry entries are added for specific development documents.

The optional WFF module that addresses the unresolved challenge of comparing welfare estimates across species. The core modules of the WFF allow robust within-species assessment by classifying Affective Experiences relative to each species’ own behavioral, physiological, neurological, pharmacological, and functional indicators. Module Ψ is invoked only when an assessment requires explicit comparison across species.

### Species-Internal Intensity Categories

The unqualified intensity terms used within WFF analyses — Annoying, Hurtful, Disabling, Excruciating; Satisfaction, Joy, Euphoria, Bliss — refer by default to categories classifying time spent in Affective States within the species, taxon, or analytical population under assessment.

Species-internal categories support within-species or within-taxon welfare assessment without requiring interspecific assumptions. They do not automatically imply equivalence with the same named category in humans or in any other species.

### Human-Anchored Reference Categories

Explicitly marked intensity categories used when making interspecific comparisons. Human-anchored reference categories are identified with the suffix **(h)** and may be used for both negative and positive affective intensities.

For negative affect, the human-anchored reference categories are:

- **Annoying(h)**
- **Hurtful(h)**
- **Disabling(h)**
- **Excruciating(h)**

For positive affect, the human-anchored reference categories are:

- **Satisfaction(h)**
- **Joy(h)**
- **Euphoria(h)**
- **Bliss(h)**

Human-anchored reference categories do not replace species-internal WFF categories and do not modify within-species Welfare Footprint calculations. They operate only at the interspecific interface, when cross-species comparison is explicitly required.

### Affective Ceiling

The maximum intensity of affective experience that a species can plausibly reach, given current evidence about its sentience, neural architecture, behavioral complexity, physiological regulation, motivational systems, ecological pressures, and evolutionary history.

Affective Ceiling is a tentative and revisable inference, not a direct measurement. It is used to make explicit the upper bound of affective intensity that an assessment is willing to attribute to a species for interspecific comparison.

Affective Ceilings should be specified by valence when relevant. A species may have one inferred ceiling for negative affective experiences, such as Pain, and another for positive affective experiences, such as Pleasure.

Affective Ceiling analysis should distinguish sensitivity from capacity. Strong reactivity to noxious stimuli, rapid avoidance, or low trigger thresholds may indicate sensitivity to harmful conditions, but they do not by themselves establish a high maximum affective ceiling.

### Affective Ceiling Analysis

A structured assessment of a species’ maximum plausible affective intensity relative to explicit reference categories. Affective Ceiling Analysis should begin with a sentience plausibility assessment and then evaluate evidence relevant to affective capacity, including neural integration, behavioral flexibility, motivational trade-offs, pharmacological modulation, physiological regulation, ecological function, and evolutionary plausibility.

Affective Ceiling Analysis may be applied separately to negative and positive affect. When both Pain and Pleasure are considered, the analysis should state whether it is assessing a **Pain Ceiling**, a **Pleasure Ceiling**, or both.

Affective Ceiling Analysis should produce a bounded, provisional conclusion rather than a precise scalar value whenever evidence is limited or contested. Its purpose is to expose the assumptions behind interspecific comparison, not to settle sentience debates, compute moral weights, rank species, or produce prioritization recommendations.

### Interspecific Scaling Correction

An optional post-quantification adjustment that maps species-internal intensity categories to explicit interspecific reference levels. Interspecific Scaling Correction should only be applied when the assessment requires cross-species comparison and when the assumptions used for that mapping have been stated, justified, and preserved in the documentation.

### Time-Mapping Assumption

An explicit assumption about whether a unit of clock time corresponds to the same amount of subjectively experienced duration across species. Time-Mapping Assumptions are relevant only after the assessment has considered whether comparable affective intensities are plausible.

Time-mapping should not be used to compensate for unsupported intensity assumptions. If a species is not plausibly capable of reaching a given human-anchored intensity level, differences in subjective time perception cannot by themselves justify assigning that intensity level.

### Scaling Transparency Requirement

Any interspecific comparison using Module Ψ must clearly distinguish:

- the original species-internal WFF estimate;
- the human-anchored or other interspecific reference categories used;
- the Affective Ceiling assumptions;
- any Time-Mapping Assumptions;
- the evidence and reasoning supporting those assumptions;
- the uncertainty or contestability of the scaling procedure.

Module Ψ outputs should be treated as provisional and open to revision. They are intended to make interspecific assumptions explicit, inspectable, and criticizable, not to create false precision or obscure uncertainty.

---

## 10. Deprecated and Replaced Terms

See `glossary/deprecated_terms.yaml`.

Notable terminology deprecations:

- `Aggregation and Standardization` → use `Econometric Calculation` for Module V.

Notable tool-name replacements:

- `Pain-Track GPT` → use `Hedonic-Track GPT` for the tool name only. `Pain-Track` remains valid for the notation method.

---

## 11. Source IDs Used in This File

Full citations should be maintained in `sources/source_registry.yaml`. This section lists source IDs used in this human-readable file.

### `wff-methodological-foundations-2025`

Primary methodological source for the WFF until the Animal Sentience version is published.

### `wfi-technical-definitions`

Operational definitions of WFF terms and modules.

### `wfi-metrics-vs-indicators-2023`

Source for the distinction between Welfare Indicators and Welfare Metrics.

### `wfi-pain-intensities`

Source for Pain Intensity categories and associated criteria.

### `wfi-positive-welfare-2024`

Source for Pleasure, Pleasure Intensity categories, Pleasure-Track, and Cumulative Pleasure.

### `wfi-ai-tools-applications`

Source for current WFI AI tool names and scopes, including Hedonic-Track GPT.

---

## 12. Follow-up Source-Registry Updates

The following items are tracked follow-up tasks for subsequent PRs, not blockers to merging PR #3. They may be addressed incrementally, provided the terms or sections they reference remain clearly identified as provisional or follow-up items in the meantime:

1. Confirm that `sources/source_registry.yaml`, `review/source_conflicts.md`, `glossary/deprecated_terms.yaml`, and any Module V file all reflect the final terminology decision: `Aggregation and Standardization` → use `Econometric Calculation`.
2. If Processogram-specific terminology remains in this file, add a source-registry entry for the Processogram manuscript or approved Processogram source.
3. If Affective Ceiling development materials remain a source basis for Module Ψ terms, add a source-registry entry for the relevant approved internal or public source, or keep the Module Ψ terms explicitly provisional.
4. If the formal scientific definition of Pain is reintroduced or cited independently of the primary WFF source or Technical Definitions, add a source-registry entry for `A Novel Proposal for the Definition of Pain`, or ensure the definition is covered through registered sources.

---

## 13. Machine-Readable Glossary Note

This human-readable canon intentionally includes definitions, distinctions, constraints, examples, and methodological cautions. The machine-readable file `glossary/wff_terms.yaml` should not flatten all of this into a single `definition` field.

For future machine-readable implementation, each term should distinguish, at minimum:

- `id`
- `term`
- `status`
- `module`
- `conceptual_role`
- `wff_chain_level`
- `definition`
- `constraints`
- `examples`
- `non_examples`
- `related_terms`
- `deprecated_aliases`
- `source_ids`
- `review_status`
- `version`

This enrichment can be handled in a dedicated follow-up PR after the human-readable terminology canon has been reviewed.
