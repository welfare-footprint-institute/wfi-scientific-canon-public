# Module II: Veterinary Inventory

**Status:** Scaffold for scientific review
**Review status:** Pending formal WFI scientific review
**Review record:** Tracked through the WFI canon review workflow

---

## Purpose

Identify and catalogue the **Biological Consequences** that arise from the
interaction between the animal's Species-Specific Needs and the Circumstances
described in Module I.

Module II bridges Circumstances to Affective Experiences by mapping the
intermediate anatomical, physiological, neurological, perceptual, and cognitive
changes through which living conditions become consciously felt states:

`Circumstances → Biological Consequences → Affective Experiences → Welfare Metrics`

Module II does not quantify affective intensity or duration. It identifies
Biological Consequences and candidate Affective Experiences that Module III
will later quantify.

---

## Core entities

> Authoritative WFF definitions and resolved methodological decisions are
> maintained in `canon/`, `glossary/`, the relevant canon files, and
> `review/resolved_methodological_decisions.md`. This section identifies the
> entities used by this module and their module-specific role; it is not an
> independent glossary.

### 1. Biological Consequences

Canonical WFF entity (see `canon/terminology.md`, Biological Consequence
entries). **Module II role:** organism-level changes or states — physical,
physiological, neurological, perceptual, or cognitive — inferred from
Module I Circumstances and Species-Specific Needs, and passed forward as
candidate sources of Affective Experiences. They include physical
manifestations (wounds, inflammation, lesions, disease processes, metabolic
imbalances, dehydration, malnutrition) as well as perceptual or cognitive
states (detecting a threat, perceiving novelty, recognizing the absence of
conspecifics, perceiving lack of agency). Biological Consequences that are
proximate precursors to Affective Experiences are the primary Module II
outputs.

### 2. Negative Biological Consequences

Module II valence-pathway grouping (corresponds to canonical groupings in
`canon/terminology.md`: "Physical Consequence Leading to Negative Affective
Experiences" and "Perceptual Consequence Leading to Negative Affective
Experiences"). **Module II role:** detrimental bodily, physiological,
perceptual, or cognitive changes likely to generate negative Affective
Experiences. Examples include:

- **Injuries:** wounds, fractures, burns, lesions, mutilation sequelae
- **Diseases and disorders:** infections, parasitic burdens, metabolic
  disorders, respiratory disease, gastrointestinal disease
- **Physiological imbalances:** dehydration, undernutrition, hyperthermia,
  hypothermia, hypoxia, exhaustion
- **Neurological or sensory changes:** nociceptive activation, sensory
  irritation, impaired proprioception
- **Perceptual or cognitive consequences:** perception of threat, social
  isolation, maternal absence, lack of agency, inability to perform highly
  motivated behaviours, exposure to aversive stimuli

### 3. Positive Biological Consequences

Module II valence-pathway grouping (corresponds to canonical groupings in
`canon/terminology.md`: "Physical Consequence Leading to Positive Affective
Experiences" and "Perceptual Consequence Leading to Positive Affective
Experiences"). **Module II role:** bodily, physiological, perceptual, or
cognitive changes likely to generate positive Affective Experiences. These
should be phrased as organism-level consequences, not merely as external
opportunities or Circumstances. Examples include:

- Satiety, hydration, thermal comfort, relief from discomfort
- Rewarding sensory stimulation or consummatory contact with preferred
  foods or resources
- Successful engagement in play, exploration, grooming, mating, nesting, or
  other motivated behaviours
- Perception of safety, social contact, maternal contact, environmental
  control, novelty, or access to preferred resources

### 4. Indicators, symptoms, and responses

Module-specific classification guidance (not a canonical WFF entity).
**Module II role:** behavioural abnormalities, physiological stress markers,
gait scores, vocalizations, stereotypies, lethargy, anorexia, and escape
attempts are not automatically Biological Consequences. Their causal role
must be specified. They may function as:

- **Indicators** of an underlying Biological Consequence
- **Symptoms** of a disease or syndrome
- **Responses** to an Affective Experience (e.g., pain behaviour following
  injury)
- **Downstream Biological Consequences** (e.g., self-directed injurious
  behaviour resulting from frustrated motivation)
- **Practical proxy categories** when the underlying cause is uncertain

Do not list behavioural observations under Biological Consequences without
specifying which of these roles they occupy.

---

## Inputs

- Module I output: Species, Production System, Life-Fates, Life-Phases,
  Species-Specific Needs, and Circumstances
- Veterinary and animal science literature
- Ethology, affective neuroscience, physiology, and comparative cognition
  literature
- Production-system health and welfare surveillance data
- Clinical classifications, lesion scores, gait scores, body condition scores,
  disease staging systems, and other severity classification schemes
- Evidence on perceptual and cognitive responses to Circumstances
- Available epidemiological literature where useful for identifying conditions
  known to occur in the target system

---

## Outputs

An inventory of Biological Consequences relevant to the target population,
including for each entry:

- Biological Consequence name and description
- Type: physical, physiological, neurological, perceptual, or cognitive
- Valence pathway: negative, positive, mixed, or uncertain
- Related Circumstance(s) from Module I
- Related Species-Specific Need(s)
- Candidate Affective Experience(s) arising from the Biological Consequence
- Pathway classification where relevant: acute / chronic; fatal / non-fatal;
  recurrent / non-recurrent; reversible / irreversible
- Biological severity classification, if available (e.g., lesion score,
  gait score, BCS, disease stage)
- Evidence sources and confidence level
- Notes on uncertainty, unresolved aetiology, or alternative causal pathways
- Flag for Module IV prevalence and occurrence estimation

---

## Required distinctions

- **Biological Consequences ≠ Circumstances.** A stocking density, a housing
  type, or a restriction regime is a Circumstance. The resulting physiological
  stress, injury, or frustrated motivation is a Biological Consequence.
- **Biological Consequences ≠ Affective Experiences.** A lesion score is a
  Biological Consequence; the Pain it causes is an Affective Experience.
  Do not carry affective inferences from this module — those belong in Module III.
- **Biological severity ≠ affective intensity.** A more severe Biological
  Consequence may often increase the probability, intensity, duration, or
  complexity of downstream Affective Experiences, but this relationship must
  be assessed rather than assumed.
- **Indicators ≠ welfare metrics.** Observations such as corticosteroid levels,
  gait scores, and behavioural measures are welfare indicators — evidence about
  Affective Experiences — not welfare metrics. See `canon/terminology.md`.
- **Presence ≠ prevalence.** This module catalogs what Biological Consequences
  exist and their plausible affective pathways; Module IV establishes how common
  they are.
- **Aetiology may be uncertain.** A Biological Consequence should not be
  excluded from the inventory merely because its precise cause or mediating
  mechanism is not fully established.

---

## Common failure modes

- Treating a veterinary measure (e.g., gait score 3) as a direct welfare metric
  without bridging to Affective Experience in Module III.
- Listing behavioural observations (stereotypies, lethargy, vocalizations,
  injurious behaviours) as Biological Consequences without specifying their
  causal role.
- Omitting perceptual and cognitive Biological Consequences, thereby excluding
  the major pathways for psychological Pain and positive welfare from the
  inventory.
- Omitting positive Biological Consequences and focusing only on injury,
  disease, or deprivation.
- Conflating biological severity with affective intensity without evidence.
- Excluding Biological Consequences merely because aetiology is uncertain or
  because the condition is subclinical.
- Including conditions without a plausible connection to Module I Circumstances,
  Species-Specific Needs, or documented occurrence in the target system.

---

## Related tools

[PLACEHOLDER — list relevant WFI tools or external databases when confirmed]

---

## Open questions

[PLACEHOLDER — document species-specific or condition-specific open questions
when identified]
