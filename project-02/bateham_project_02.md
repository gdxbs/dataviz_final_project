# Data Visualization 

> Gregory Bateham

## Mini-Project 2: An Analysis of Billboard Summer Hits

This project explores the audio characteristics of songs from the "All Billboard Summer Hits" dataset. My goal was to practice data wrangling and visualization to uncover the patterns that define a summer hit and to tell a story about how the sound of popular music has evolved over the decades. 

### Motivation

The concept of a "song of the summer" is a major part of pop culture, but what gives a song that distinct summer feel? This project was motivated by a desire to look beyond subjective opinion and use quantitative audio feature data to answer that question. By analyzing decades of Billboard hits, I was able to identify the specific sonic ingredients that make a song feel upbeat, danceable, and memorable.

### Data Description

The dataset used is `all_billboard_summer_hits.csv`, which contains track information and a suite of audio features for songs that have appeared on Billboard charts. The key variables utilized in this analysis include:

* **Track Metadata**: `track_name`, `artist_name`, `year`
* **Audio Features**: `danceability`, `energy`, `valence` (a measure of musical positiveness), `loudness`, `acousticness`, `instrumentalness`, and `speechiness`.

For the analysis, a `decade` column was created from the `year` variable to group songs for historical comparison.

### Summary of Findings

* **The Timeless Formula for a Hit:** The interactive scatter plot revealed a strong and persistent positive correlation between a song's **energy** and its **danceability**. This suggests that for decades, the most reliable recipe for a summer hit has been to make it both high-energy and easy to dance to.

* **The Shifting Sound of Summer:** The conceptual spatial map was created to visualize the "homes" of different musical eras. By linking decades to influential music cities (e.g., 1970s Disco to New York), the map tells a story of how the cultural center of pop music has evolved, from the British Invasion sound of 60s London to the globalized pop of the 2010s.

* **The Recipe for a "Happy" Song:** The multiple linear regression model was built to predict a song's `valence` (its perceived happiness or positivity). The model's coefficients clearly showed that **energy** and **danceability** are the strongest positive predictors of valence. Conversely, `acousticness` was a significant negative predictor, confirming that stripped-down, acoustic tracks are generally perceived as more mellow or melancholic, not as upbeat summer anthems.