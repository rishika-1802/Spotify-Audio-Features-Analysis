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

## 🎵 Features Explained (from Spotify API)

All columns in this dataset and full descriptions:

| Feature              | Description |
|----------------------|-------------|
| `artist_name`        | Name of the artist. |
| `track_id`           | Spotify's unique track ID. |
| `track_name`         | Name of the song/track. |
| `acousticness`       | Confidence from 0.0 to 1.0 whether the track is acoustic. 1.0 = very likely acoustic. |
| `danceability`       | How suitable a track is for dancing (0.0 = not danceable, 1.0 = very danceable). |
| `duration_ms`        | Duration of the track in milliseconds. |
| `energy`             | Intensity and activity level of a track. Higher values mean more energetic. |
| `instrumentalness`   | Likelihood a track has no vocals (closer to 1.0 = more instrumental). |
| `key`                | Estimated key (0 = C, 1 = C♯/D♭, ..., 11 = B). -1 if unknown. |
| `liveness`           | Detects audience presence. Values >0.8 imply live performance. |
| `loudness`           | Overall loudness (in dB). Ranges typically between -60 and 0. |
| `mode`               | Modality: 1 = major, 0 = minor. |
| `speechiness`        | Detects spoken words. Closer to 1.0 = more speech-like. |
| `tempo`              | Beats per minute (BPM). |
| `time_signature`     | Number of beats per bar (e.g., 4 means 4/4 time). |
| `valence`            | Musical positivity. 0.0 = sad, 1.0 = happy. |
| `popularity`         | Spotify popularity score (0–100). Higher = more popular. |

ℹ️ **Note:** Popularity is based on total plays and recency.


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
pip install pip install -r requirements.txt

```
2. Run the code file `spotify_code.py` or use in Jupyter Notebook.

---



---

## 📬 Contact
Have questions or want to collaborate? Reach out anytime!~rishika1826@gmail.com 🎶
