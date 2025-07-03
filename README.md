# 🎵 Spotify Audio Features Analysis 📊

Welcome to the **Spotify Audio Features Analysis** project! 🎧

This project performs in-depth exploratory data analysis (EDA), statistical modeling, and machine learning to predict song popularity using audio features from Spotify.

---

## 📁 Project Overview

This notebook covers:

- 🔍 **EDA & feature exploration**
- 📈 **Linear & Logistic Regression** models
- 🧪 **Statistical testing** (e.g., ANOVA)
- 🎯 **Evaluation metrics** (ROC, AUC, Confusion Matrix)
- 🧠 **Sampling and balancing strategies**

---

## 📥 Dataset Source

📦 **Dataset:** [Spotify Audio Features April 2019](https://www.kaggle.com/datasets/zaheenhamidani/ultimate-spotify-tracks-db)  
Downloaded from Kaggle. It contains thousands of songs with Spotify’s extracted audio attributes and metadata.

---

## 🎼 Audio Feature Terms Explained

| Feature | Description |
|--------|-------------|
| **danceability** | Describes how suitable a track is for dancing (0.0–1.0). 💃 |
| **energy** | A perceptual measure of intensity and activity (0.0–1.0). 🔋 |
| **valence** | Musical positivity. High valence = happy, cheerful songs. 😊 |
| **acousticness** | Confidence measure of whether a track is acoustic. 🎸 |
| **instrumentalness** | Predicts the presence of vocals. Higher = more instrumental. 🎻 |
| **liveness** | Presence of an audience. Higher values mean live performance. 🎤 |
| **speechiness** | Amount of spoken words in a track. 🗣️ |
| **loudness** | Overall loudness (in dB). 📢 |
| **tempo** | Speed of the song in beats per minute (BPM). 🕒 |
| **key** | The musical key (0–11) representing C to B. 🎶 |
| **mode** | Major (1) or Minor (0) key. 🌕🌑 |
| **time_signature** | Beats per measure (e.g., 4/4, 3/4). 🎵 |
| **popularity** | Spotify's internal score (0–100). 🌟 |

---

## 📊 Visualization Techniques Used

The project uses rich plots to uncover patterns:

- 🔹 **Scatter Plots**: Explore relationships between features (e.g., `danceability` vs `popularity`).
- 🔹 **Pair Plots**: Show pairwise relationships and correlations using Seaborn.
- 🔹 **Histograms**: View the distribution of `popularity` and other continuous variables.
- 🔹 **Violin Plots**: Compare distribution shapes of features across `Popular` and `Not_Popular` categories.
- 🔹 **Heatmap**: Visual correlation matrix between features to spot multicollinearity.
- 🔹 **ROC Curve**: Plots true vs false positive rates for classification performance.
- 🔹 **Confusion Matrix**: Summarizes classification predictions with true/false positives and negatives.

---

## 🧠 Modeling Strategy

Two major approaches are used:

### 🔹 Linear Regression
Used to predict the continuous `popularity` score.

### 🔹 Logistic Regression
Used to classify whether a song is **Popular** (e.g., popularity > 80).

#### Balanced Sampling
To reduce bias, undersampling is used so the model sees a balanced number of popular and not-popular tracks.

#### Metrics Used:
- **Accuracy**
- **Precision**
- **Recall**
- **ROC AUC**

---

## ✅ How to Run

1. Make sure dependencies are installed:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
```
2. Run the code file `spotify_analysis.py` or use in Jupyter Notebook.

---

## 🙌 Author
Created with ❤️ by **Élodie💕**

---

## 📬 Contact
Have questions or want to collaborate? Reach out anytime! 🎶
