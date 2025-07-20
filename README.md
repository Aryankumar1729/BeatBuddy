# 🎧 BeatBuddy - AI-Powered Music Recommendation System

BeatBuddy is a **content-based song recommendation system** that suggests similar tracks based on both genre and numerical audio features. Whether you're vibing to a mellow tune or a high-energy banger, BeatBuddy finds you the next perfect track — intelligently.

---

## 🚀 Features

- 🎶 **Smart Song Matching**: Enter a song name to receive intelligent music recommendations.
- 📊 **Text + Numeric Similarity**: Combines genre (text) and audio features (numbers) using cosine similarity.
- ❓ **Graceful Handling of Unknown Songs**: If a song isn’t found, the app suggests random tracks to keep the music flowing.
- 🔗 **Spotify API Integration**: Get direct Spotify links for recommended tracks.

---

## 🧠 How It Works

1. **Vectorization**: The genre of each song is transformed using `TfidfVectorizer`.
2. **Feature Extraction**: Numeric features such as tempo, danceability, and energy are extracted using `pandas`.
3. **Similarity Calculation**: Cosine similarity is applied to both text and numerical vectors.
4. **Recommendation Output**: The top matches are returned with song titles and Spotify track URLs.

---

## 🛠️ Tech Stack

- Python 3
- NumPy
- Pandas
- Scikit-learn
- Spotify API (for metadata and track hrefs)

---

## 📸 Screenshots

| Input Song | Output Recommendation |
|------------|------------------------|
| `"Me Love"` | 5 song recommendations with Spotify links |
| `"Shape of You"` | Song not found fallback with 5 random suggestions |

---
