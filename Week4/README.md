## Unsupervised Learning

Performed k-means clustering of Spotify's dataset which contains 13 features related to each song: acousticness, danceability, duration_ms, energy, instrumentalness, key, liveness, loudness, mode, speechiness, tempo, time_signature, and valence.

**Step 1:** Computed first 2 Principle Components (PC's).

A pipeline was fitted which first standardizes the values w.r.t. Z-score of each metric, and then performs PCA. The factor loadings for each metric for the first 2 PC's are as follows:

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/wk4-2-1.png?raw=true"/>

**Step 2:** Visualized various songs wrt the PC's.

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/wk4-2-4.png?raw=true"/>

**Step 3:** Created pandas dataframes of the top-3 metrics w.r.t. each PC.

For PC 1:

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/wk4-2-2.png?raw=true"/>

For PC 2:

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/wk4-2-3.png?raw=true"/>

**Step 4:** Run K-means for 10 PC's, and 5 clusters.

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/wk4-2-5.png?raw=true"/>

## Generalization Performance

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/wk4-1.png?raw=true"/>

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/wk4-2.png?raw=true"/>

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/wk4-3.png?raw=true"/>

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/wk4-4.png?raw=true"/>

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/wk4-5.png?raw=true"/>

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/wk4-6.png?raw=true"/>

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/wk4-7.png?raw=true"/>
