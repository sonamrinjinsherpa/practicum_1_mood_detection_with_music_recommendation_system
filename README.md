# Mood-Aware Music Recommendation System

## Project Overview

The rapid growth of digital music streaming platforms has made it increasingly difficult for users to discover music that matches their preferences, listening context, and emotional state. Modern platforms host millions of songs across diverse genres and artists, making efficient music discovery an important challenge. This project explores the development of a mood-aware music recommendation system using Spotify audio features.

The system uses numerical audio attributes such as danceability, energy, tempo, loudness, acousticness, and valence to represent songs. These features describe both the structural and emotional characteristics of music. By analyzing these attributes, the system identifies songs with similar acoustic properties and generates recommendations accordingly.

The recommendation model follows a content-based filtering approach and computes similarity between songs using cosine similarity and nearest neighbor techniques. The goal of this project is to demonstrate how data science techniques can be applied to music recommendation and mood-based music discovery.

---

## Dataset

The datasets used in this project are publicly available Spotify datasets containing thousands of songs along with numerical audio features generated using Spotify's audio analysis algorithms.

Each track in the dataset includes features describing the musical structure and emotional characteristics of songs. Key features used in this project include:

- Danceability
- Energy
- Loudness
- Tempo
- Acousticness
- Instrumentalness
- Liveness
- Speechiness
- Valence

These features provide a quantitative representation of music that allows similarity between songs to be measured computationally.

Dataset Source:

Spotify Songs Dataset (Kaggle)  
https://www.kaggle.com/datasets/joebeachcapital/30000-spotify-songs

---

## Methodology

The recommendation system follows a content-based filtering approach using Spotify audio features. Instead of relying on user listening behavior, the system analyzes the intrinsic characteristics of songs to determine similarity.

The workflow of the project consists of the following steps:

1. Data collection and preprocessing  
2. Exploratory data analysis (EDA)  
3. Mood representation using audio features  
4. Feature normalization and scaling  
5. Similarity computation using cosine similarity  
6. Recommendation generation using nearest neighbors  
7. Evaluation of recommendation results  

Each song is represented as a numerical feature vector composed of selected Spotify audio features. Cosine similarity is used to compute the similarity between songs, and the nearest neighbors algorithm retrieves the most similar tracks for recommendation.


## Repository Structure

data/
raw/            → original datasets
processed/      → cleaned datasets

notebooks/
data_prep_and_eda.ipynb
mood_inference.ipynb
recommendation_system.ipynb
evaluation.ipynb

reports/
figures/        → visualizations used in the report
practicum_report.pdf

---


## Tools and Libraries

The project was implemented using the following tools and libraries:

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Plotly
- Jupyter Notebook
- Git and GitHub

---

## Results

The implemented recommendation system successfully identifies songs with similar acoustic structures and mood-related characteristics. Songs characterized by high energy and fast tempo tend to generate recommendations within energetic musical genres such as pop or electronic music. Conversely, songs with higher acousticness and lower energy often produce recommendations associated with calmer musical styles.

These results demonstrate that Spotify audio features provide meaningful signals for representing musical similarity and mood-related characteristics within recommendation systems.

---

## Future Work

Several improvements could enhance the recommendation system in future work. One possible extension is the incorporation of collaborative filtering techniques to complement the content-based approach. Hybrid models that combine multiple recommendation strategies often provide more accurate and personalized recommendations.

Another potential improvement is the use of larger datasets or additional sources of musical information such as song lyrics or user listening behavior. Deep learning methods could also be explored to capture more complex relationships between musical features and listener preferences.

---

## Author

Sonam Rinjin Sherpa  
Master of Science in Data Science  
Regis University

## System Architecture 
