---
epistemic_grade: E3
---

# Enzyme & Microbial Kinetics, Water Activity ($a_w$) Stasis, Lignocellulose & Iberian Flora (`sci-biology` — `E3/E2`)

> **Epistemic Credibility Grade: `E3/E2` (Primary Biochemical, Microbiological & Statutory Botanical Reference)**
>
> Quantitative reference tables for enzyme/microbial kinetics, water-activity ($a_w$) preservation cut-points (`N` vs. `N ± 1`), biosafety levels, lignocellulosic cell-wall fractions, and native vs. `RD 630/2013` invasive Iberian flora consumed via `make consult LAYER=sci-biology` ([01_biological_sciences_taxonomy_and_scale_hierarchy.md](../architecture/01_biological_sciences_taxonomy_and_scale_hierarchy.md)).

---

## 1. Enzyme (`Michaelis-Menten`) & Microbial (`Monod`) Kinetic Cut-Points (`BIO-SCI-01`) [E3]

> **Summary [E3]:** *Saturable biological catalysis ($v = V_{\max}[S]/(K_m + [S])$) and microbial specific growth ($\mu = \mu_{\max}[S]/(K_s + [S])$) transition from first-order substrate limitation (`[S] << K_m`) through the exact half-saturation cut-point (`[S] = K_m`) to zero-order saturation (`[S] >> K_m`), bounded sharply by thermal denaturation ([01_biological_systems_and_bioprocess_foundations.md](../guides/01_biological_systems_and_bioprocess_foundations.md)).*

$$v = \frac{V_{\max}[S]}{K_m + [S]} = \frac{k_{\text{cat}}[E]_0[S]}{K_m + [S]}, \qquad \mu = \frac{1}{X}\frac{dX}{dt} = \frac{\mu_{\max}[S]}{K_s + [S]}$$

The table below defines exact kinetic and thermal-stability cut-points (`N` vs. `N ± 1`):

| Biochemical Parameter | Sub-Threshold Regime | Exact Cut-Point (`N` vs. `N ± 1`) | Super-Threshold Regime |
| :--- | :--- | :--- | :--- |
| **Substrate Saturation Ratio ($[S]/K_m$)** | $[S] \le 0.05\,K_m$: Pseudo-first-order ($v \approx \frac{k_{\text{cat}}}{K_m}[E]_0[S]$) | $[S] = K_m \iff v = 0.50\,V_{\max}$ | $[S] \ge 20\,K_m$: Zero-order active-site saturation ($v \ge 0.952\,V_{\max}$). |
| **Phytochemical & Enzyme Thermal Window ($T$)** | $T \in [35.0\,^\circ\text{C}, 40.0\,^\circ\text{C}]$: Native pectin/polyphenol & enzyme retention | $T = 40.0\,^\circ\text{C}$ (upper preservation bound) / $T = 42.0\,^\circ\text{C}$ (unfolding onset) | $T > 42.0\,^\circ\text{C}$ progressive protein denaturation; $T \ge 60.0\,^\circ\text{C}$ rapid vegetative inactivation + Maillard browning. |
| **Chemostat Dilution Washout ($D = F/V$)** | $D < \mu_{\max}\frac{S_{\text{in}}}{K_s + S_{\text{in}}}$: Stable steady-state biomass $X^* > 0$ | $D_{\text{crit}} = \mu_{\max}\frac{S_{\text{in}}}{K_s + S_{\text{in}}}$ | $D \ge D_{\text{crit}}$: **Complete bioreactor cell washout ($X \to 0$)**. |

---

## 2. Water Activity ($a_w$) Microbial Stasis & Biosafety Cut-Points (`BIO-SCI-02`) [E3]

> **Summary [E3]:** *Water activity $a_w = p / p_0 \in [0, 1]$ governs thermodynamic water availability for cellular metabolism; reducing substrate equilibrium below the strict cut-point $a_w < 0.60$ (`< 10.0% w/w` moisture in lignocellulose) guarantees complete bacterial, yeast, and fungal stasis without chemical preservatives ([01_biological_sciences_taxonomy_and_scale_hierarchy.md](../architecture/01_biological_sciences_taxonomy_and_scale_hierarchy.md)).*

The table below maps minimum $a_w$ proliferation cut-points across microbial classes:

| Water Activity Cut-Point ($a_w = p/p_0$) | Lignocellulose Moisture (`% w/w`, `25 °C`) | Limiting Organism Group | Biological & Mycotoxin Risk State |
| :---: | :---: | :--- | :--- |
| **`a_w >= 0.95`** | `> 25.0%` | Gram-negative rods (*Pseudomonas*, *Escherichia*, *Salmonella*) | Rapid bacterial spoilage and endotoxin accumulation. |
| **`0.91 <= a_w < 0.95`** | `20.0% – 25.0%` | Most Gram-positive bacteria (*Bacillus*, *Lactobacillus*) | Bacterial proliferation; *Staphylococcus aureus* aerobic down to `0.86`. |
| **`0.80 <= a_w < 0.91`** | `15.0% – 20.0%` | Fermentative yeasts (*Saccharomyces*) & mycotoxigenic molds (*Aspergillus flavus*, *Penicillium*) | **High aflatoxin / ochratoxin biosynthesis hazard**. |
| **`0.60 <= a_w < 0.80`** | `10.0% – 15.0%` | Xerophilic molds (*Aspergillus restrictus*, *Xeromyces bisporus* `0.61`) & osmophilic yeasts (*Zygosaccharomyces rouxii* `0.62`) | Slow xerophilic spoilage over multi-week storage (`REJECT` batch stasis). |
| **`a_w < 0.60` (`Strict Cut-Point`)** | **`< 10.0% w/w`** | **Zero replicating microorganisms (`0` Bacteria, Yeasts, Molds)** | **Absolute Microbial & Fungal Stasis** ($a_w = 0.59$ `PASS` vs. $a_w = 0.60$ `HOLD/RE-DRY`). |

- **Biosafety Containment Levels (`RD 664/1997` / `EU Directive 2000/54/EC`, `E3`)**: `BSL-1` (non-pathogenic *GRAS* strains, e.g., *Saccharomyces cerevisiae*), `BSL-2` (moderate individual risk, Class II biosafety cabinet), `BSL-3` (serious aerosol-transmissible pathogens, negative-pressure HEPA containment), `BSL-4` (high-consequence life-threatening agents without treatment). Circular biomaterial valorization nodes operate strictly on **`BSL-1` / Food-Grade Plant Substrates**.

---

## 3. Lignocellulosic Biopolymer Stoichiometry & Thermal Transitions (`BIO-SCI-03`) [E3]

> **Summary [E3]:** *Plant secondary cell walls comprise crystalline cellulose, branched hemicellulose, cross-linked aromatic lignin, and pectic polysaccharides whose distinct hydrophilicity and thermal decomposition intervals govern drying, milling, and anoxic carbonization.*

1. **Cellulose ($\text{(C}_6\text{H}_{10}\text{O}_5\text{)}_n$, `35% – 50%` dry mass)**: Linear $\beta(1 \to 4)$-D-glucan hydrogen-bonded microfibrils; tensile reinforcement; main endothermic volatilization window `315 °C – 400 °C`.
2. **Hemicellulose (`20% – 35%` dry mass)**: Amorphous branched pentosans/hexosans (xylans, glucomannans); highest moisture sorption capacity; thermal cleavage window `200 °C – 315 °C`.
3. **Lignin (`15% – 32%` dry mass)**: Cross-linked phenylpropanoid network (*p-hydroxyphenyl*, *guaiacyl*, *syringyl* units); confers hydrophobicity, decay resistance, and primary fixed-carbon biochar yield across `250 °C – 650 °C`.
4. **Pectin & Polyphenolic Extractives (`3% – 18%` dry mass)**: Galacturonic acid hydrocolloids, oleuropein, hydroxytyrosol, and tannins preserved intact within `[35.0 °C, 40.0 °C]` (`Fe`-free `AISI 316` contact prevents oxidative darkening).

---

## 4. Authorized Native Iberian Botanical Substrates vs. `RD 630/2013` Exclusion Registry (`BIO-SCI-04`) [E2]

> **Summary [E2]:** *All botanical feedstocks sourced in Spain must cross-check taxonomic binomials against `Real Decreto 630/2013` (`BOE-A-2013-8565`, Catálogo Español de Especies Exóticas Invasoras), authorizing native/cultivated Mediterranean and Atlantic agro-forestry co-products while strictly blocking invasive taxa.*

The table below classifies primary Iberian agro-forestry substrates and statutory invasive exclusions:

| Binomial Name (*Genus species*) | Family | `geo-es` Bioregions | Typical Lignin (`% dry`) | Statutory Status (`Ley 42/2007` & `RD 630/2013`) |
| :--- | :--- | :--- | :---: | :--- |
| ***Olea europaea*** *(Olive pomace, leaf, pruning, pit)* | `Oleaceae` | Mediterranean (`ES-AN`, `ES-CM`, `ES-EX`, `ES-CT`, `ES-VC`) | `24% – 30%` | **Authorized (`Native / Traditional Crop`)** |
| ***Quercus ilex*** / ***Quercus suber*** *(Holm & Cork Oak)* | `Fagaceae` | Mediterranean & Dehesa (`ES-EX`, `ES-AN`, `ES-CL`, `ES-CM`) | `26% – 32%` | **Authorized (`Native Silviculture Pruning Only`)** |
| ***Vitis vinifera*** *(Grape marc, stalk, cane)* | `Vitaceae` | All Iberian wine regions (`ES-RI`, `ES-CL`, `ES-CM`, `ES-CT`, `ES-GA`) | `22% – 26%` | **Authorized (`Native / Traditional Crop`)** |
| ***Pinus pinaster*** / ***Pinus pinea*** *(Maritime & Stone Pine)* | `Pinaceae` | Atlantic & Mediterranean (`ES-GA`, `ES-CL`, `ES-AN`) | `27% – 32%` | **Authorized (`Sustainable Forestry Management`)** |
| ***Prunus dulcis*** / ***Citrus sinensis*** *(Almond shell, Citrus peel)* | `Rosaceae` / `Rutaceae` | Mediterranean (`ES-VC`, `ES-MC`, `ES-AN`, `ES-AR`) | `8% – 30%` | **Authorized (`Agro-Industrial Co-Product`)** |
| ***Ailanthus altissima*** / ***Cortaderia selloana*** / ***Acacia dealbata*** | `Simaroubaceae` / `Poaceae` / `Fabaceae` | Ruderal / Coastal / Atlantic invasive zones | — | **PROHIBITED (`RD 630/2013` Possession, Transport & Valorization Ban)** |
