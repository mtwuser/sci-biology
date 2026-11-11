# sci-biology — Sovereign Epistemic Knowledge Corpus (`v1.0.0`)

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](VERSION)
[![ZeroCloudGravity](https://img.shields.io/badge/ZeroCloudGravity-v1.0.0-0F766E.svg)](https://github.com/mtwuser/zero-cloud-gravity)
[![Epistemic Grade](https://img.shields.io/badge/epistemic_grade-E3..E1-1D4ED8.svg)](docs/README.md)
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

> **Biological Sciences Knowledge Corpus (`IUBS`: Biochemistry, Enzyme/Microbial Kinetics, Water Activity Stasis & Iberian Flora)** (`layer_role: knowledge`, `precedence: 20`, `stewardship_stage: public-community`).

## 1. Epistemic Corpus Index (`1:1:1` Progressive Disclosure)

All sections expose deterministic `rcap1` (`L0 -> L3`) capsules and cryptographic `citation_receipt` anchors (`<layer>::<file>#<slug>@<sha256_16>:<E3..E0>`):

| Tier | Credibility | Document |
| :--- | :--- | :--- |
| **Index** | `E2` | [`docs/README.md`](docs/README.md) |
| **Guide (`M1 -> M4`)** | `E1` | [Biological Systems, Microbial Stasis & Bioprocess Foundations Guide (`M1 -> M4` — `E1`)](docs/guides/01_biological_systems_and_bioprocess_foundations.md) |
| **Architecture & Taxonomy** | `E3` | [Biological Sciences Taxonomy, Quantitative Scale Hierarchy & Pure-to-Applied Bridge (`E3`)](docs/architecture/01_biological_sciences_taxonomy_and_scale_hierarchy.md) |
| **Primary Reference** | `E3/E2` | [Enzyme & Microbial Kinetics, Water Activity ($a_w$) Stasis, Lignocellulose & Iberian Flora (`E3/E2`)](docs/reference/01_biochemistry_microbial_stasis_and_botanical_substrates.md) |

## 2. Mounting & Querying from Any `ZeroCloudGravity` Node

Link or mount this corpus into a personal (`<persona>-pc`, `<persona>-tutor`), research, or enterprise node without cloud dependencies:

```bash
zcg link <your-node-dir> --target https://github.com/mtwuser/sci-biology.git --relation knowledge-feed
zcg consult-layer <your-node-dir> --layer sci-biology --query "<topic>" --tier flash
```

## 3. Layer Setup Blueprint (`State U2: configured`)

- **Node ID & Role**: `sci-biology` (`knowledge`, `precedence: 20`, `surface_veracity_mode: full-open-source`)
- **1-Hop Upstream Engine**: [`mtwuser/zero-cloud-gravity`](https://github.com/mtwuser/zero-cloud-gravity)
- **Active Template Packs**: `science-base`, `scientific-methodology`, `sci-biology`, `knowledge-stewardship-portal`
- **Mission, Scope & Core Invariants**: Quantitative biological sciences corpus (`E3..E1`) covering `IUBS` scale hierarchy, Michaelis-Menten and Monod kinetics, water-activity ($a_w$) microbial stasis cut-points, and botanical substrates.
- **Downstream Topology**: Consumed read-only via `knowledge-feed` links or `layers/*` subtrees across academic, scientific, public-sector, and enterprise nodes.
- **Authorized Layer Steward**: `sci-biology Knowledge Steward <mtwuser@users.noreply.github.com>`
