# WFF Visualization Conventions

**Status:** Draft for scientific review
**Review status:** Pending formal WFI scientific review
**Review record:** Tracked through the WFI canon review workflow
**Canonical source type:** Human-readable WFF visualization conventions draft
**Last updated:** 2026-06-13
**Related canon files:** `canon/intensity_categories_pain.md`, `canon/intensity_categories_pleasure.md`, `visualization/intensity_colors.yaml`

---

## Intensity color gradients

The Welfare Footprint Framework uses canonical visualization color gradients for Pain and Pleasure intensity categories.

These colors are visualization conventions. They are not part of the scientific definitions of the intensity categories.

Pain uses a warm gradient from lower to higher intensity. Pleasure uses a cold gradient from lower to higher intensity.

## Pain gradient

| Category | Hex code | Notes |
|---|---:|---|
| Annoying | `#939238` | muted olive/yellow |
| Hurtful | `#B8923B` | ochre / amber-brown |
| Disabling | `#B53F2F` | burnt red |
| Excruciating | `#7A3A5F` | dark plum / deep suffering tone |

## Pleasure gradient

| Category | Hex code | Notes |
|---|---:|---|
| Satisfaction | `#ADD8E6` | light blue |
| Joy | `#40E0D0` | turquoise |
| Euphoria | `#008080` | teal |
| Bliss | `#483D8B` | deep indigo |

## Use rule

Pain and Pleasure are valence-specific scales and should not be merged into a single visual scale or netted against one another.

Tools, dashboards, slides, charts, and generated visualizations should use the machine-readable palette defined in:

`visualization/intensity_colors.yaml`

The source canon tables remain:

- `canon/intensity_categories_pain.md`
- `canon/intensity_categories_pleasure.md`
