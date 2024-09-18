## Song Recommendation System Using K-Means Clustering and Spotify API

### Overview

This project builds a song recommendation system by clustering a collection of songs based on their audio features. The dataset was created by fetching song data using the Spotify API and clustering was performed using K-Means. The system enables more accurate song recommendations by limiting recommendations to songs within the same cluster, which share similar audio characteristics.

**Key Features**
- API Integration: Used Spotify API to retrieve audio features like danceability, energy, loudness, and more for a large number of songs.
- Unsupervised Learning: Applied K-Means Clustering to group songs into clusters based on their audio attributes.
- Feature Evaluation: Conducted ANOVA to determine which audio features significantly vary across clusters.
- Optimal Clustering: Determined the best number of clusters using the Elbow Method and Silhouette Score for better recommendation accuracy.

![image](https://github.com/user-attachments/assets/14dfa65e-3db9-4154-8033-b2f0acad71bb)
![image](https://github.com/user-attachments/assets/b3b3bae5-4eff-4bec-b707-be31ab19327e)

### Technologies Used

- Programming Language: Python
- Libraries: pandas, NumPy, seaborn, matplotlib, scikit-learn, statsmodels
- API: Spotify API
- Machine Learning: KMeans Clustering, ANOVA

**Dataset**

- Source: Data was collected using the Spotify API. The dataset includes a wide range of audio features for each song.
- Key Features:
    Danceability
    Energy
    Loudness
    Tempo
    Acousticness
    Instrumentalness
    Speechiness
    Popularity
    Length

![image](https://github.com/user-attachments/assets/dc8a9b02-960e-44b9-83f4-4cfd2cf034b9)


**Spotify API Setup:**

You will need to create a Spotify Developer account to obtain your API key and client secret.
Create a config.py file and add your credentials:

    python
        client_id = 'your-client-id'
        client_secret = 'your-client-secret'

### Results

- Optimal Clustering: The optimal number of clusters was determined using the Elbow Method and Silhouette Scores.
- Cluster Analysis: Audio features like length and time signature showed significant differences between clusters, as confirmed by ANOVA tests.

### Future Work

- Improve the recommendation algorithm by adding more audio features and refining the clustering process.
- Integrate a web interface using Flask to allow users to input a song and receive recommendations in real-time.
