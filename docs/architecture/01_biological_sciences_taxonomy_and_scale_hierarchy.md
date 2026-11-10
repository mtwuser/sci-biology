---
epistemic_grade: E3
---

# Biological Sciences Taxonomy, Quantitative Scale Hierarchy & Pure-to-Applied Bridge (`sci-biology` — `E3`)

> **Epistemic Credibility Grade: `E3` (Canonical UNESCO / IUBS Life Sciences Architecture)**
>
> This architecture specification defines the five foundational branches of **`sci-biology`** (`canonical_trunk: "nature"`), its quantitative scale and bioenergetic hierarchy (`0.1 nm -> Biosphere`), and its orthogonal epistemic bridges to `sci-physics`, `sci-engineering`, `geo-es`, and `gov-es` ([01_biochemistry_microbial_stasis_and_botanical_substrates.md](../reference/01_biochemistry_microbial_stasis_and_botanical_substrates.md)).

---

## 1. The 5 Canonical Pure Branches of `sci-biology` (`IUBS`) [E3]

> **Summary [E3]:** *Within the UNESCO/Frascati natural-science trunk, `sci-biology` organizes living systems across five spatial and informational branches (`BIO-BR-01..05`), supplying foundational biochemical, microbiological, physiological, and ecological truth to downstream bioprocess and environmental nodes ([01_biochemistry_microbial_stasis_and_botanical_substrates.md](../reference/01_biochemistry_microbial_stasis_and_botanical_substrates.md)).*

The table below maps each life-science branch to its characteristic spatial scale, governing laws, and downstream consumers:

| Branch ID & Domain | Biological Scale | Primary `E3` Governing Laws & Invariants | Downstream Consumers |
| :--- | :--- | :--- | :--- |
| **`BIO-BR-01`: Biochemistry, Structural & Molecular Biology** | `0.1 nm – 100 nm` (*Biomolecules & Polymers*) | Molecular sequence transfer ($\text{DNA} \to \text{RNA} \to \text{Polypeptide}$), Michaelis-Menten kinetics ($v = V_{\max}[S]/(K_m + [S])$), protein denaturation, lignocellulosic biopolymers. | Enzymatic valorization, `[35.0 °C, 40.0 °C]` phytochemical drying windows (`sci-engineering`, `dept-iso-bio`). |
| **`BIO-BR-02`: Cell Biology, Microbiology & Mycology** | `1 µm – 1 mm` (*Prokaryotes, Fungi, Protists*) | Cell theory, water potential ($\Psi_w = \Psi_s + \Psi_p + \Psi_m$), Monod growth ($\mu = \mu_{\max}[S]/(K_s + [S])$), **Water Activity ($a_w$) Stasis Cut-Points**. | Moisture stasis (`a_w < 0.60`, `< 10.0% w/w`), `BSL-1..4` biosafety, mycotoxin prevention (`dept-iso-bio`). |
| **`BIO-BR-03`: Genetics, Genomics & Evolutionary Systematics** | *Generations & Phylogenies* | Mendelian segregation, Hardy-Weinberg allele equilibrium ($p^2 + 2pq + q^2 = 1$), phylogenetic taxonomy (`ICN` / `ICZN`), mutation-selection balance. | Strain characterization, taxonomic authentication, population biostatistics (`sci-maths`). |
| **`BIO-BR-04`: Organismal Physiology, Botany & Zoology** | `1 mm – 100 m` (*Tissues, Organs, Organisms*) | Physiological regulation, xylem cohesion-tension ($\Delta \Psi_w$), C3/C4/CAM photosynthesis ($6\text{CO}_2 + 6\text{H}_2\text{O} \to \text{C}_6\text{H}_{12}\text{O}_6 + 6\text{O}_2$), metabolic scaling. | Iberian botanical substrate selection (*Olea*, *Quercus*, *Vitis*, *Pinus*), agronomic physiology (`geo-es`). |
| **`BIO-BR-05`: Ecology, Biogeochemistry & Circular Bioeconomy** | `1 km – Biosphere` (*Ecosystems & Biomes*) | Trophic transfer efficiency (`~10%` Lindeman rule), C:N:P biogeochemical mass balances, Lotka-Volterra dynamics, invasive species exclusion (`RD 630/2013`). | Bioregional circular bioeconomy (`org-iso`), statutory biodiversity compliance (`gov-es` `Ley 42/2007`). |

---

## 2. Quantitative Bioenergetic & Stoichiometric Hierarchy [E3]

> **Summary [E3]:** *Living cells operate as open non-equilibrium thermodynamic systems (`sci-physics` `PHYS-03`) coupling exergonic `ATP` hydrolysis ($\Delta G^{\circ\prime} \approx -30.5\text{ kJ}\cdot\text{mol}^{-1}$) and redox potentials ($\Delta G^{\circ\prime} = -nF\Delta E^{\circ\prime}$) to maintain low internal entropy while exporting heat and metabolic byproducts ([01_biological_systems_and_bioprocess_foundations.md](../guides/01_biological_systems_and_bioprocess_foundations.md)).*

The table below codifies canonical biochemical and ecological reference invariants across biological scales:

| Bioenergetic / Stoichiometric Quantity | Standard Biochemical Condition (`pH 7.0`, `298.15 K`, `1 atm`) | Quantitative Reference Value | Governing Coupled Law |
| :--- | :--- | :--- | :--- |
| **`ATP` Hydrolysis Standard Free Energy** | $\text{ATP}^{4-} + \text{H}_2\text{O} \rightleftharpoons \text{ADP}^{3-} + \text{P}_i^{2-} + \text{H}^+$ | $\Delta G^{\circ\prime} = -30.5\text{ kJ}\cdot\text{mol}^{-1}$ (cellular $\Delta G \approx -50\text{ to }-54\text{ kJ}\cdot\text{mol}^{-1}$) | Endergonic biosynthesis coupling ($\Delta G_{\text{net}} < 0$). |
| **Biochemical Redox Coupling** | Electron transport ($\text{NADH} \to \text{O}_2$, $n = 2$, $\Delta E^{\circ\prime} = +1.14\text{ V}$) | $\Delta G^{\circ\prime} = -n F \Delta E^{\circ\prime} \approx -220.0\text{ kJ}\cdot\text{mol}^{-1}$ | Faraday constant $F = 96\,485.33\text{ C}\cdot\text{mol}^{-1}$ (`sci-physics`). |
| **Water Potential Equilibrium ($\Psi_w$)** | Isothermal water transport between compartments $A \to B$ | $\Psi_w = \frac{RT}{\bar{V}_w} \ln(a_w)$ ($\Psi_w = 0\text{ MPa}$ pure water; $a_w = 0.60 \implies \Psi_w \approx -70.4\text{ MPa}$ at $25\,^\circ\text{C}$) | Water flows passively from higher $\Psi_w$ to lower $\Psi_w$; extreme negative $\Psi_w$ desiccates microbial cytoplasm. |
| **Canonical Biomass Elemental Ratios** | Marine phytoplankton (`Redfield`) vs. Terrestrial lignocellulose | Marine `C:N:P = 106:16:1` (molar) · Woody biomass `C:N = 200:1 to 500:1` | Composting / `SSF` requires `C:N` adjustment (`25:1 – 35:1` optimal microbial growth vs. `> 60:1` nitrogen-limited). |

---

## 3. Orthogonal Separation Between `sci-biology`, `sci-physics` & `sci-engineering` [E3]

> **Summary [E3]:** *`sci-biology` owns foundational life-science axioms (`E3`), while `sci-physics` owns continuum heat/mass transport (`E3`) and `sci-engineering` owns equipment metallurgy, unit-operation sizing, and `SIL` interlocks (`E2`), eliminating cross-repository duplication.*

1. **Pure Life Science (`sci-biology`)**: Defines *why* microbial metabolism halts at $a_w < 0.60$, *why* thermolabile enzymes/polyphenols denature above $42.0\,^\circ\text{C}$, and *which* Iberian botanical species are native vs. invasive.
2. **Physical & Engineering Realization (`sci-physics` + `sci-engineering`)**: Consumes `sci-biology` `citation_receipt` thresholds to size convective dehydrators (`[35.0 °C, 40.0 °C]`), `AISI 316/316L` non-catalytic contact surfaces, and `ISO 3310-1` milling/sieving lines.
