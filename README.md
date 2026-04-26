
# EU Pesticide Rejection Pattern Analysis
### RASFF alert analysis + market routing tool for Kenyan agricultural exporters

---

## What This Project Does

Analyzes 902 EU pesticide rejection alerts (2018–2026) from the RASFF database to identify patterns in which countries, crops, and chemicals get flagged most — then builds a simple market routing tool that tells Kenyan exporters which chemicals are high risk depending on their target market (EU, UK, or Gulf).

---

## Why It Exists

Most of the chemicals dominating EU rejection alerts — chlorpyrifos, chlorothalonil, carbendazim — are still registered and actively used in Kenya. This project maps that risk using real data.

---

## Key Findings

- **Chlorpyrifos** is the most flagged pesticide globally (302 alerts) — banned in EU since 2020
- **Turkey, India, Egypt** dominate rejections — each with distinct chemical risk profiles
- **Kenya's 4 alerts** involve chlorpyrifos (avocado) and chlorothalonil (sugar snap peas, thyme, basil) — the same chemicals at the top of global rejection lists
- **EU and UK MRLs are nearly identical** post-Brexit — the real gap is EU/UK vs Gulf (Codex standards)

---

## Market Routing Tool

```python
compare_markets('Avocado')
# EU  → 🔴 HIGH risk: chlorpyrifos, chlorothalonil
# UK  → 🔴 HIGH risk: chlorpyrifos, chlorothalonil  
# Gulf → 🟢 None
```

---

## Stack

Python · pandas · matplotlib · seaborn · Jupyter

---

## Structure

```
├── data/RASFF_window_results.xlsx
├── notebooks/rasff_analysis.ipynb
├── charts/
└── README.md
```

---

## Author

Agronomist + data science learner. This project sits at the intersection of both — using EU food safety data to surface insights relevant to Kenyan export agriculture.
