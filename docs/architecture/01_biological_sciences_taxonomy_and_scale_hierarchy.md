# Biological Sciences Taxonomy, Scale Hierarchy & Biophysical/Bioprocess Bridge (`sci-biology` — `E3`)

> **Epistemic Credibility Grade: `E3` (Canonical UNESCO/IUBS Life Sciences Architecture & Pure-to-Applied Bridge)**
>
> This architecture specification defines the 5 foundational branches of **`sci-biology`** (`canonical_trunk: "nature"`), its multi-scale organization (`Molecule -> Biosphere`), and its formal epistemic bridge to physical transport laws (`sci-physics`) and circular bioprocess engineering (`sci-engineering`, `dept-iso-bio`).

---

## 1. The 5 Canonical Pure Branches of `sci-biology` (`BIO-SCI-01..03` — `E3`)

Within the UNESCO/Frascati scientific taxonomy, **`sci-biology`** is the pure natural-science pillar (`nature` trunk) governing living matter, from which biophysics (`sci-physics`) and industrial biotechnology / bioprocess engineering (`sci-engineering`) derive their living-system first principles:

| Branch ID & Domain | Biological Scale | Core Principles & Governing Laws (`E3`) | Downstream Applications (`tutor-iso-lab`, `dept-iso-bio`, `sci-engineering` Bridge) |
| :--- | :--- | :--- | :--- |
| **`BIO-BR-01`: Biochemistry, Biophysics & Molecular Biology** | `0.1 nm – 100 nm` (*Molecules & Biopolymers*) | Central Dogma ($\text{DNA} \to \text{RNA} \to \text{Protein}$), Michaelis-Menten enzyme kinetics ($v = V_{\max}[S]/(K_m + [S])$), protein thermal denaturation, and lignocellulosic biopolymer architecture (*Cellulose*, *Hemicellulose*, *Lignin*, *Pectin*). | Biomaterial valorization, enzymatic hydrolysis, thermal dehydration windows (`[35.0°C, 40.0°C]` in `dept-iso-bio`), biopolymer composite mechanics (`sci-engineering`). |
| **`BIO-BR-02`: Cell Biology, Microbiology & Mycology** | `1 µm – 1 mm` (*Prokaryotes, Eukaryotes, Fungi*) | Cell theory, membrane osmotic potential ($\Psi_w = \Psi_s + \Psi_p$), Monod microbial growth ($\mu = \mu_{\max}[S]/(K_s + [S])$), and **Water Activity ($a_w = p/p_0$) Stasis Cut-Points**. | Solid-State Fermentation (`SSF`), moisture stasis (`< 10.0%` w/w, $a_w < 0.60$ preventing *Aspergillus*/*Penicillium* mycotoxins in `dept-iso-bio`), bioreactor sterility (`sci-engineering`). |
| **`BIO-BR-03`: Genetics, Epigenetics & Evolutionary Biology** | *Information & Generations* | Mendelian inheritance, Hardy-Weinberg equilibrium ($p^2 + 2pq + q^2 = 1$), natural selection, phylogenetic systematics, and genomic regulation. | Strain selection, biodiversity conservation, population genetics modeling (`sci-maths`). |
| **`BIO-BR-04`: Organismal Physiology, Botany & Zoology** | `1 mm – 100 m` (*Tissues, Organs, Organisms*) | Homeostasis, plant vascular transport (xylem/phloem cohesion-tension), photosynthesis ($6\text{CO}_2 + 6\text{H}_2\text{O} \xrightarrow{h\nu} \text{C}_6\text{H}_{12}\text{O}_6 + 6\text{O}_2$), and organ-system physiology. | Iberian/Mediterranean botanical sourcing (*Olea*, *Quercus*, *Vitis*, *Pinus*), plant tissue mechanics & transport (`sci-physics`). |
| **`BIO-BR-05`: Ecology, Biogeochemistry & Circular Bioeconomy** | `1 km – Biosphere` (*Populations & Ecosystems*) | Trophic energy transfer ($10\%$ Lindeman law), Carbon/Nitrogen/Phosphorus biogeochemical cycles, Lotka-Volterra dynamics, and endemic vs. invasive species exclusion (`RD 630/2013`). | Bioregional circular economy (`org-iso`, `dept-iso-bio` `BIO-04`), ecosystem biogeography (`geo-es` + `gov-es`). |

---

## 2. Orthogonal Bridge Between Pure `sci-biology` (`nature`), `sci-physics` (`nature`) and `sci-engineering` (`engineering`)

Rather than duplicating foundational life-science laws inside engineering or industrial repositories, the architecture enforces a clean `Trunk -> Branch` separation:

- **`sci-biology` (`nature` trunk — Pure Foundational Life Science)**: Owns cellular physiology, biochemistry, microbiology, genetics, botany, and ecology (`E3`).
- **`sci-physics` & `sci-engineering` (`nature` & `engineering` trunks — Biophysical Transport & Applied Bioprocess Engineering)**: Consume `sci-biology` `E3` physiological, botanical, and microbiological axioms via `citation_receipt` and add coupled heat/mass transfer (`sci-physics`), `AISI 316/316L` bioreactor metallurgy, `ISO 3310-1` granulometric sieving, and `ISO 10816` structural health monitoring (`sci-engineering` `E2`).
