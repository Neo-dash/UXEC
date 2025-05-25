# 🧭 UXEC — User Experience Emotional Cartography

> A lightweight, reproducible AI pipeline for emotion-aware UX mapping in tourism and urban space.

UXEC transforms geolocated hotel reviews into **interactive emotional heatmaps**, uncovering patterns of joy, anger, and neutrality across cities.  
It is ideal for researchers and practitioners interested in **spatial UX**, **tourism marketing**, and **experience design**.

---

## 🌐 Overview

UXEC combines:

- 🧠 Lightweight **Natural Language Processing** (MiniLM + VADER)
- 📌 Emotion-aware **spatial clustering** with GA-DBSCAN
- 🗺️ Interactive **heatmap generation** (Folium/Leaflet)
- 🔬 Academic-grade methodology for tourism UX analysis

> Applied on 12,000 hotel reviews from London 🇬🇧

---

## 📁 Project Structure

```text
UXEC/
├── data/                # Raw and processed hotel review data
│   ├── raw/
│   └── processed/
│
├── notebooks/           # Jupyter notebooks for each processing step
│   ├── 01_preprocessing.ipynb
│   ├── 02_emotion_extraction.ipynb
│   ├── 03_clustering.ipynb
│   └── 04_mapping.ipynb
│
├── utils/               # Utility scripts (clustering, mapping, geocoding)
│   └── geo_utils.py
│   └── clustering.py
│
├── output/              # Figures and exported maps
│   ├── joy_heatmap.png
│   └── cluster_stats.csv
│
├── requirements.txt     # Python dependencies
├── README.md            # You are here!
└── LICENSE
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/UXEC.git
cd UXEC
```

### 2. Create a Python environment

```bash
python -m venv venv
source venv/bin/activate   # or venv\Scripts\activate on Windows
pip install -r requirements.txt
```

### 3. Run the notebooks

Open the `notebooks/` directory and run each step in sequence:

- 📦 `01_preprocessing.ipynb` — Load, clean, and structure data  
- 💬 `02_emotion_extraction.ipynb` — Apply VADER & MiniLM for emotion tagging  
- 📍 `03_clustering.ipynb` — Apply GA-DBSCAN for spatial segmentation  
- 🔥 `04_mapping.ipynb` — Generate Folium-based interactive maps  

---

## 🧾 Dataset Description

> Dataset: [Kaggle - Hotel Reviews in Europe](https://www.kaggle.com/datasets/jiashenliu/515k-hotel-reviews-data-in-europe)

We use a sample of **12,000 hotel reviews** from London with the following fields:

| Field               | Description                                  |
|--------------------|----------------------------------------------|
| Hotel\_Name         | Name of the hotel                            |
| lat / lng          | Latitude and longitude                       |
| Review\_Date        | Date of the review                           |
| Positive\_Review    | Positive part of the comment (free text)     |
| Negative\_Review    | Negative part of the comment (free text)     |
| Reviewer\_Score     | Global score given by the customer (1–10)    |

This dataset is ideal for spatial UX research because it combines rich **free-text content** with **geographic precision**.

---

## 🧠 Techniques & Models

| Technique                     | Purpose                                 |
|------------------------------|-----------------------------------------|
| `VADER` Sentiment Scoring    | Extract base emotions (joy, anger, etc.)|
| `MiniLM` Embeddings          | Semantic similarity across comments     |
| `GA-DBSCAN`                  | Density-based clustering (spatial)      |
| `Folium` / `Leaflet.js`      | Interactive map rendering                |

> All models are CPU-optimized — no GPU required.

---

## 🗺️ Example Output

### 📌 Joy Heatmap (London)

![Joy Heatmap](output/joy_heatmap.png)

This map highlights zones where visitors consistently expressed **positive emotions** such as satisfaction or delight.  
It enables experience designers and destination managers to:

- Identify **emotional hotspots**
- Validate high-performing areas
- Inform tour planning and spatial storytelling

---

## 🔬 Use Cases

- Tourism & destination experience audits  
- Emotion-aware smart city planning  
- AR-enhanced itinerary design  
- Urban UX & sentiment research  
- Public feedback spatial analytics

---

## 📚 Citation

If you use UXEC in your research or academic project, please cite:

```bibtex
@inproceedings{uxec2024,
  title     = {De l’émotion à la décision : cartographie de l’expérience client touristique par l’intelligence artificielle},
  author    = {Kdayem, Moetez and Collaborator, X.},
  booktitle = {Proceedings of the XX Conference on UX and Spatial Marketing},
  year      = {2024}
}
```

---

## 🤝 Contributing

We welcome:

- 🔍 Testing on new datasets (e.g., Yelp, Google Maps, OSM)  
- 🧠 Adapting to other domains (retail, culture, transportation)  
- 🛠️ Feature suggestions & PRs  
- 🌍 City-specific forks  

Feel free to star ⭐, fork 🔀, or open an issue 🐛.

---

## 📬 Contact

Achraf KACEM  
📧 kacem.achraf[at]outlook.com


---

## 📝 License

Licensed under the MIT License.  
See [`LICENSE`](LICENSE) for full details.

---

> UXEC — Mapping Emotions, Enhancing Experiences 🌍💙
