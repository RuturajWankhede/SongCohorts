# Song Popularity and Cohort Analysis

This project explores the factors influencing song popularity using a dataset from Spotify. It employs techniques like data preprocessing, feature scaling, PCA for dimensionality reduction, and K-means clustering to identify trends and cohorts within the data.

## Table of Contents
1. [Project Structure](#project-structure)
   - [1. Data Loading and Cleaning](#1-data-loading-and-cleaning)
   - [2. Exploratory Data Analysis (EDA)](#2-exploratory-data-analysis-eda)
   - [3. Feature Scaling](#3-feature-scaling)
   - [4. Principal Component Analysis (PCA)](#4-principal-component-analysis-pca)
   - [5. Clustering](#5-clustering)
2. [Key Findings and Insights](#key-findings-and-insights)
3. [Model Performance](#model-performance)
4. [Suggestions for Improvement](#suggestions-for-improvement)
5. [Conclusion](#conclusion)
6. [Future Work](#future-work)

## Project Structure

### 1. Data Loading and Cleaning
The project begins by loading a dataset of song attributes from Spotify, which includes features such as `acousticness`, `danceability`, and `popularity`.

**Screenshot**:
- Table preview of the loaded data (showing columns like `name`, `album`, `popularity`).

![dataPreview](https://github.com/user-attachments/assets/6891a2ee-22bd-4f2f-aaab-7da40a9f6b14)

### 2. Exploratory Data Analysis (EDA)
EDA reveals interesting patterns in song attributes and popularity, such as the dominance of loudness and danceability in determining popularity.

**Screenshots**:
- Boxplot visualizing outliers in features like `duration_ms` and `tempo`.

![durationBoxplot](https://github.com/user-attachments/assets/31bc84a9-7aba-4a62-a3f8-00a914fbb92f)

![tempoBoxplot](https://github.com/user-attachments/assets/d9f3fd58-5e2e-47c1-9bfa-c1b5e606fc65)


### 3. Feature Scaling
All numerical features were scaled using MinMaxScaler to prepare for PCA and clustering.


### 4. Principal Component Analysis (PCA)
PCA was applied to reduce dimensionality and identify key factors influencing song popularity.

**Screenshots**:
- Scatter plot of the two principal components.

![PCA](https://github.com/user-attachments/assets/7ab016f9-bde9-4711-9a71-a70f6e8cfd3b)


### 5. Clustering
K-means clustering was used to group songs into cohorts based on the principal components.

**Screenshots**:
- Elbow plot for determining the optimal number of clusters.

![elbowPlot](https://github.com/user-attachments/assets/18404417-6e75-4f3b-950f-103a6b16ca4b)

- Scatter plot showing the clusters of songs.

![Kmeans](https://github.com/user-attachments/assets/597722db-e04b-4438-a756-24eb2a0f1c45)

## Key Findings and Insights
- **Loudness and Danceability**: These features significantly impact song popularity, especially in recent years.
- **Cohorts**: The K-means algorithm identified clusters of songs based on similar features.

## Model Performance
The PCA and clustering models performed well in reducing dimensionality and grouping songs into meaningful cohorts.

## Suggestions for Improvement
1. **Add more features**: Incorporate additional metadata like genre and artist information.
2. **Tune clustering**: Experiment with different clustering algorithms or number of clusters.

## Conclusion
The project demonstrates the use of PCA and K-means clustering to analyze song popularity and create song cohorts.

## Future Work
1. **Time-series analysis**: Investigate how song popularity changes over time.
2. **Recommendation system**: Build a system to recommend songs based on cohort membership.
