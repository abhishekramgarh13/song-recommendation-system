# 🎵 Song Recommendation System

A hybrid music recommendation engine combining **Content-Based Filtering** and **Collaborative Filtering**, with end‑to‑end data versioning, preprocessing, model training, and a Streamlit web UI.

---

## 🔍 Features

- **Content-Based Filtering** (`content_based_filtering.py`):  
  - TF‑IDF vectorization of song metadata (genre, artist, lyrics)  
  - Cosine similarity search  

- **Collaborative Filtering** (`collaborative_filtering.py`):  
  - User–item interaction matrix  
  - K‑Nearest Neighbors for user‑based recommendations  

- **Hybrid Recommendations** (`hybrid_recommendations.py`):  
  - Weighted blending of content and collaborative scores  

- **Data Pipeline & Versioning**:  
  - DVC for dataset/version control (`dvc.yaml`, `.dvc`, `dvc.lock`)  
  - Pre‑processing & transformations (`data_cleaning.py`, `transform_filtered_data.py`)  

- **Streamlit App** (`app.py`):  
  - Interactive UI for “Recommend me a song”  
  - Slider controls for weighting hybrid scores  

- **Testing & CI**:  
  - Environment checks (`test_environment.py`)  
  - `tox.ini` for multi‑environment testing  

---

## 🚀 Quick Start

### 1. Clone & Install
```bash
git clone https://github.com/abhishekramgarh13/song-recommendation-system.git
cd song-recommendation-system
pip install -r requirements.txt


