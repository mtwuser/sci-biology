---
trigger: always_on
description: "Taxonomic Nomenclature, Biochemical/Microbial Homeostasis (Water Activity a_w), and Ecological Non-Invasiveness Rules (sci-biology)"
---

# Biological & Life Sciences Corpus Rules (`sci-biology`)

## Scope & Surface Target
- **Template Pack**: `templates/sci-biology/` (`context-stack`).
- **Knowledge Domain**: `scientific-epistemic` (`canonical_trunk: "nature"`, pure life-science foundation with formal biophysical and bioprocess bridges to `sci-physics` and `sci-engineering`, `E3..E1`).

## Normative Invariants (`BIO-SCI-01..03`)

1. **`BIO-SCI-01` (Binomial Taxonomic Precision & Multi-Scale Organization)**:
   - Every biological organism, tissue, or botanical substrate must be identified by its canonical italicized Linnaeus binomial name (*Genus species*, e.g. *Olea europaea*, *Quercus ilex*, *Vitis vinifera*, *Aspergillus niger*) and located on the biological scale hierarchy (`Molecule -> Organelle -> Cell -> Tissue/Organ -> Organism -> Ecosystem`).
2. **`BIO-SCI-02` (Biochemical Homeostasis, Water Activity $a_w$ & Enzymatic/Microbial Cut-Points)**:
   - Biological stability, fermentation, and preservation models must state exact physicochemical cut-points in SI units: temperature window ($^\circ\text{C}$ / $\text{K}$), pH, water activity ($a_w = p/p_0 \in [0, 1]$, where $a_w < 0.60$ enforces absolute microbial/fungal stasis), and Michaelis-Menten / Monod kinetic parameters ($V_{\max}, K_m, \mu_{\max}$).
3. **`BIO-SCI-03` (Ecological Non-Invasiveness, Biosafety & Bioprocess Bridge to `sci-engineering`)**:
   - Cross-reference regional flora against invasive-species catalogs (`gov-es` `RD 630/2013` & `geo-es` bioregions), enforce biosafety containment (`BSL-1..4`), and anchor applied bioprocess/biomaterial extensions (`sci-engineering`, `dept-iso-bio`) to `sci-biology::docs/...#<slug>@<digest16>:E3`.

## Verification & Sign-Off Gates
- [ ] Verify zero drift via `zcg diff-project`.
- [ ] Confirm binomial taxonomy, water activity ($a_w$), and temperature cut-points across all biological specifications.
