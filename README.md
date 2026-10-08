# 🎬 CineMatch — Movie Recommender System

A content-based movie recommendation system that recommends movies similar to a selected movie using **machine learning, text similarity, and the TMDB API**.

The project is built with **Python, Pandas, Scikit-learn, Streamlit**, and **TMDB API**.

---

## 🚀 Live Demo

🌐 **[CineMatch — Movie Recommender](https://movie-recommender-system-shr.onrender.com/)**

> The application is deployed using Render.

---

## 📌 Project Overview

CineMatch recommends movies based on the content and characteristics of a movie selected by the user.

The recommendation system uses information such as:

- 🎭 Genres
- 🔑 Keywords
- 📝 Movie Overview
- 👨‍🎬 Top Cast
- 🎥 Director

These features are combined into a single **tags** representation.

The tags are then converted into numerical vectors using **CountVectorizer**, and **Cosine Similarity** is used to find movies with similar content.

---

## 🧠 How It Works

The recommendation pipeline follows these steps:

```text
Movie Dataset
     ↓
Data Cleaning
     ↓
Merge Movies + Credits Dataset
     ↓
Select Important Features
     ↓
Create Tags
     ↓
Text Vectorization
     ↓
Cosine Similarity
     ↓
Find Similar Movies
     ↓
Fetch Movie Posters using TMDB API
     ↓
Display Recommendations
