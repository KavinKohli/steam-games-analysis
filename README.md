# Steam Games Analysis

An exploratory data analysis of the Steam game catalog, digging into genres, platform support, pricing, playtime, and player reviews — all visualized with a dark, gaming-inspired aesthetic.

## About

This project analyzes a large dataset of games listed on Steam to answer questions like:

- Which genres dominate the platform, and which ones players actually spend time in?
- How does platform support (Windows / Mac / Linux) and pricing break down across the catalog?
- Which games have the highest average playtime?
- How do reviews and estimated ownership numbers relate to a game's success?
- What does the price distribution look like for paid titles?

The analysis is done entirely in a single Jupyter notebook using `pandas`, `numpy`, and `matplotlib`, styled with a custom dark "gaming" theme (neon greens, cyans, and pinks) instead of default matplotlib styling.

## 🗂️ Contents

| File | Description |
|---|---|
| `Notebook.ipynb` | Main analysis notebook — data cleaning, EDA, and visualizations |
| `LICENSE` | MIT License |
| `.gitignore` | Standard ignores |

## 🔍 Notebook Sections

1. **Data Cleaning** — loads the raw Steam dataset, drops irrelevant/high-null columns (screenshots, movies, support URLs, etc.), and filters out non-ASCII game titles
2. **Analysis of Most Popular Categories** — genre counts and average playtime by genre (recent vs. all-time)
3. **Comparing Games** — free vs. paid split, platform availability (Windows/Mac/Linux), and top 20 games by average playtime
4. **Review Analysis** — parses estimated owner ranges and cross-references them with genres and review data
5. **Price Analysis** — distribution of paid game prices with median price overlay

## 🛠️ Built With

- Python
- pandas / numpy
- matplotlib (custom dark theme via `cycler`)
- Jupyter Notebook

## 🚀 Running Locally

```bash
git clone https://github.com/KavinKohli/steam-games-analysis.git
cd steam-games-analysis
pip install pandas numpy matplotlib
jupyter notebook Notebook.ipynb
```

> **Note:** the notebook expects a `Steam_Games.csv` file in the same directory. Add your own copy of the Steam games dataset (e.g. from Kaggle) to run it end-to-end.
