# UXEC — User Experience Emotional Cartography

📍 **UXEC** is a lightweight, reproducible pipeline for analyzing and mapping the emotional landscape of user experiences based on geolocated reviews. Designed for tourism and urban UX research, the project leverages natural language processing (NLP), clustering, and spatial visualization to generate actionable emotional heatmaps from free-text feedback.

---

## 🧠 What is UXEC?

**UXEC** transforms raw user reviews into meaningful emotional maps, helping researchers, data scientists, and destination managers answer questions like:

- Where do users feel **joy, anger, or neutrality** in a city or destination?
- Can we identify **emotional hotspots** or zones of friction from public feedback?
- How can we align **spatial experience design** with emotional traces?

UXEC combines:
- 🗺️ **Geospatial analytics**
- 💬 **Lightweight NLP (MiniLM, VADER)**
- 📊 **Density-based clustering (GA-DBSCAN)**
- 🔥 **Interactive heatmaps (Folium/Leaflet)**

---

## 📦 Folder Structure

```bash
UXEC/
│
├── data/                    # Raw and processed hotel review data
│   ├── raw/
│   └── processed/
│
├── notebooks/               # Jupyter notebooks for each step
│   ├── 01_preprocessing.ipynb
│   ├── 02_emotion_extraction.ipynb
│   ├── 03_clustering.ipynb
│   ├── 04_mapping.ipynb
│
├── output/                  # Figures and maps generated
│   ├── joy_heatmap.png
│   └── cluster_stats.csv
│
├── utils/                   # Utility scripts and helpers
│   └── geo_utils.py
│   └── clustering.py
│
├── requirements.txt         # List of Python dependencies
├── README.md                # This file
└── LICENSE
