# ncl-mutation-landscape
Python data visualization of the mutational landscape across CLN1–CLN8 genes in neuronal ceroid lipofuscinoses (NCL)
# NCL Mutational Landscape Visualizer 🧬

A Python data analysis project visualizing the mutational landscape of **Neuronal Ceroid Lipofuscinoses (NCL)** — a group of rare, inherited neurodegenerative disorders caused by mutations in *CLN* genes.

---

## What this project does

Generates a 4-panel figure from curated variant data across 7 NCL-associated genes (CLN1–CLN8):

| Panel | Chart type | What it shows |
|-------|------------|---------------|
| Top-left | Stacked bar chart | Variant count broken down by mutation type per gene |
| Top-right | Donut chart | Clinical significance classification across all NCL variants |
| Bottom-left | Heatmap | Mutation type density across all CLN genes |
| Bottom-right | Horizontal stacked bar | Disease onset profile (early / juvenile / adult) per gene |

---

## Why NCL?

NCL is the most common group of inherited childhood neurodegenerative disorders, with a collective incidence of 1 in 100,000 live births. Mutations in *CLN6* — one of the genes analyzed here — cause a transmembrane protein defect associated with progressive myoclonus epilepsy and rapid neurological decline.

This project was built alongside an ongoing review article on **the pathophysiological link between CLN6 mutations and progressive myoclonus epilepsy**.

---

## Tech stack

- **Python 3.9+**
- `pandas` — data structuring
- `matplotlib` — bar charts, donut chart, figure layout
- `seaborn` — heatmap
- `numpy` — array math for stacking bars

---

## Getting started

```bash
# Clone the repo
git clone https://github.com/yourusername/ncl-mutation-landscape.git
cd ncl-mutation-landscape

# Install dependencies
pip install pandas matplotlib seaborn numpy

# Run the analysis
python ncl_variant_analysis.py
```

The figure is saved as `ncl_mutation_landscape.png` in the project directory.

---

## Data sources

Variant data curated from:
- **ClinVar** (NCBI) — accessed 2023
- Mole et al. (2019). *Neuronal ceroid-lipofuscinoses.* Biochim Biophys Acta Mol Basis Dis.
- Schulz et al. (2013). *NCL disease mechanisms.* J Inherit Metab Dis.

> Note: Values represent approximate variant counts and proportions reported in the literature. This is a summary visualization, not a live database query.

---

## Project structure

```
ncl-mutation-landscape/
│
├── ncl_variant_analysis.py   # Main analysis script
├── ncl_mutation_landscape.png # Output figure (auto-generated)
└── README.md
```

---

## Future directions

- [ ] Pull live ClinVar data via the **NCBI E-utilities API**
- [ ] Add protein domain annotation track for CLN6
- [ ] Interactive dashboard using **Plotly / Dash**
- [ ] Expand dataset to include CLN10–CLN14

---

## Author

Tamana Javed — BSc Biotechnology, final year  
Research focus: CLN6 neuronal ceroid lipofuscinosis | Bioinformatics

---

## License

MIT License — free to use, adapt, and build on.
