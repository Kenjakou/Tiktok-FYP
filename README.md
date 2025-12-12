# TikTok Ethical Recommender – Proof of Concept (PoC)
A lightweight prototype demonstrating how TikTok's “For You” feed can be redesigned to reduce algorithmic addiction by giving users **control over how recommendations are generated**.

This project implements:
- A simplified TikTok-style scoring algorithm
- Three user-selectable algorithm modes  
- Diversity visualizations  
- CSV output of recommended videos  
- A PDF PoC Paper  
- Optional Streamlit UI

---

## 📌 Project Overview
Most social media platforms optimize for **engagement**, causing:
- Filter bubbles  
- Repetitive content loops  
- Addictive scrolling  
- Reduced user autonomy  

This PoC shows how a small modification—**letting users choose how personalized their algorithm is**—can improve ethical outcomes.

---

## 🚀 Features
### **Three Recommendation Modes**
| Mode | Description |
|------|-------------|
| **High Personalization** | TikTok-like behavior. Strong category weighting. |
| **Balanced** | Mix of personalization + diversity. |
| **Explore Mode** | High diversity, new categories pushed forward. |

### Outputs Provided
- CSV files of top-12 recommendations for each mode  
- Bar graph distributions of categories  
- A complete PoC research paper (`PoC_Paper.pdf`)  
- `streamlit_app.py` for a simple UI  

---

## 📂 Project Structure
tiktok_poc/
│  
├── synthetic_tiktok_dataset.csv
├── recommender.py
├── streamlit_app.py
├── rec_high_personalization.csv
├── rec_balanced.csv
├── rec_explore.csv
│
├── hp_distribution.png
├── balanced_distribution.png
├── explore_distribution.png
│
├── PoC_Paper.pdf
└── README.md

### **1. Install Dependencies**
If using Colab:
```python
!pip install pandas numpy matplotlib reportlab streamlit
