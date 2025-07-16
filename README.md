# 🎬 Movie Recommendation System

A content-based movie recommendation web app built with **Flask**, **Pandas**, **scikit-learn**, and **HTML**. It analyzes movie metadata like **genres**, **cast**, **keywords**, **director**, and **tagline** to suggest similar movies using **TF-IDF vectorization** and **cosine similarity**.

---

## 🚀 Features

- 🔎 Recommend similar movies based on a movie you like
- 🧠 Uses TF-IDF + Cosine Similarity for content-based filtering
- 📁 Reads movie metadata from a CSV file
- 💡 Intelligent approximate matching with `difflib` for input tolerance
- 🌐 Simple and interactive Flask-based web interface

---

## 🧠 How It Works

1. **Input**: User enters the name of a movie
2. **Matching**: App finds the closest matching movie from the dataset using `difflib`
3. **Similarity**: Calculates similarity scores based on selected features:
   - `genres`, `keywords`, `tagline`, `cast`, `director`
4. **Output**: Top 30 similar movies are displayed on the same page

---

## 📁 Dataset

The system uses a CSV file named `movies.csv` with the following important columns:

- `index` (unique ID)
- `title`
- `genres`
- `keywords`
- `tagline`
- `cast`
- `director`

📝 **Note**: Ensure that all these fields exist and contain valid data (or are filled with empty strings if null).
