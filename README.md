
---

## 🎬 **2. Movie Recommendation System**
```markdown
# 🎬 Movie Recommendation System
A content-based recommendation engine that suggests movies using similarity measures between features.

## 📘 Overview
This project builds a **content-based recommender system** using movie metadata (title, genre, keywords, cast, and crew).  
It helps users find similar movies based on their preferences.

## 📊 Dataset
- **Source:** Kaggle’s TMDB Movie Dataset  
- **Files:** `tmdb_5000_movies.csv` and `tmdb_5000_credits.csv`
- **Features Used:**
  - `genres`, `keywords`, `overview`, `cast`, `crew`

## ⚙️ Process
1. **Data Cleaning & Preprocessing**
   - Merged both CSVs on movie ID
   - Removed missing values
   - Selected relevant features
2. **Feature Engineering**
   - Created a new column combining key textual features
   - Used **CountVectorizer** to convert text into numerical vectors
3. **Similarity Computation**
   - Applied **Cosine Similarity** to measure closeness between movies
4. **Recommendation Function**
   - Built a function that outputs top similar movies given a movie name

## 🧰 Tools & Libraries
- `pandas`, `numpy`
- `scikit-learn`
- `nltk` (for text processing)
- `ast` (to parse strings as lists)

## 🚀 How to Run
```bash
pip install pandas numpy scikit-learn nltk
jupyter notebook movie_recommend_project.ipynb
