# fashion-niche-analysis


This project investigates the Try-Hard Paradox in fashion: how people signal originality and niche taste in a culture where trends move too fast to hold their value.

We use three case studies that capture different sides of the fashion cycle:

**Maison Margiela Tabis** – an avant-garde shoe turned internet meme.

**Issey Miyake Pleats Please / Homme Plissé** – once an insider’s uniform, now widely adopted as quiet-luxury shorthand.

**Le Labo Santal 33** – a fragrance that shifted from cult niche to global cliché.

The aim is to build a Niche Authenticity Score (NAS), a data-driven metric that distinguishes between niche authenticity and trend-hopping.

The final deliverable is an interactive Streamlit dashboard that evaluates items against the NAS framework and visualizes their chic inflation curves, dupe ecosystems, and subcultural anchors.

## Motivation

Fashion’s value often lies in its perceived rarity. But in an accelerated trend economy, even highly niche pieces can become overexposed within months. This raises questions like:

When does a garment or fragrance still read as authentic?

At what point does it collapse into trend uniformity or “try-hard” signaling?

Can we measure the half-life of chic?

This project approaches those questions through a mix of data science, cultural analysis, and visualization.

## Methodology

### Data Sources

Outfit and styling images from Pinterest, TikTok, Reddit, and forums

Resale data from Grailed, eBay, TheRealReal (price floors, volatility)

Google Trends for temporal exposure curves

Fragrantica for perfume note pyramids and dupe networks

### Feature Engineering

Visual uniqueness: CLIP embeddings → cluster density and silhouette rarity

Textual rarity: TF-IDF on hashtags/captions

Market stability: resale median and volatility

Temporal signals: lead/lag between niche vs mainstream adoption

Perfume dupe density: number of “similar to” edges in fragrance graphs

Scoring Framework

## Trend Exposure

NAS=0.3⋅(Hashtag Rarity)+0.3⋅(Visual Uniqueness)+0.2⋅(Resale Stability)+0.2⋅(1−Trend Exposure)
Planned Deliverables

Streamlit dashboard: upload an outfit/perfume → returns NAS with breakdown

Visualizations:

UMAP scatterplots of niche vs mainstream clusters

Chic Inflation curves for Tabis, Pleats, Santal 33

Perfume dupe networks

Case study writeups: each item analyzed for its chic inflation trajectory

## Roadmap

 Define scope and repo structure

 Collect seed dataset (Tabis, Pleats, Santal 33)

 Engineer baseline features

 Implement NAS formula and first model

 Build dashboard with visualization modules

 Write report with case study findings