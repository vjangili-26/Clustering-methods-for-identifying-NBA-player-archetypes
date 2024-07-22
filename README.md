# NBA Archetypes Using Clustering Algorithms

## ABSTRACT
The NBA coaches and scouts need to identify player archetypes to build successful teams. With a vast amount of player performance data at their disposal, advanced analytical techniques can be used to find patterns that aid this process. In this paper, we will explore clustering methods to group NBA players based on their statistical performance and identify player archetypes while investigating the traits that define them. The resulting archetypes can inform player evaluation, roster construction, and game strategy. Teams might prioritize signing players who fit a specific archetype to fill gaps in their roster. We are using a dataset consisting of player statistics from the 2018-2019 NBA season. K-means clustering, Gaussian clustering, and DBSCAN will group players based on similarity in various statistical categories. This study aims to provide a more comprehensive understanding of NBA player performance using data analytics, enabling teams to make informed decisions about player evaluation, team building, and game strategies. The results of this research have implications not only for NBA teams but also for other organizations seeking to analyze large datasets and find patterns to guide decision-making.

**Keywords:** archetypes, K-means, Gaussian clustering, DBSCAN, data analytics

## INTRODUCTION
The basketball leagues require teams to find the right players and assembling a strong team roster are essential for success in professional basketball. Coaches and scouts must find the best players and develop player archetypes using the vast amounts of player performance data that are currently available and cutting-edge analytical techniques. This paper aims to identify player archetypes while examining the characteristics that define them by using clustering methods to group NBA players based on their statistical performance. The resulting archetypes can guide player evaluation, roster planning, and game strategy. Teams can prioritize signing players who fit a specific archetype to fill gaps in their roster by spotting common patterns in player performance data. K-means clustering, Gaussian clustering, and DBSCAN clustering will be used to group players based on similarity in different statistical categories using a dataset of player statistics from the 2018-2019 NBA season.

## LITERATURE REVIEW
Clustering is a popular technique in data mining and machine learning that involves grouping data points into clusters based on their similarity. There are many different clustering algorithms and methods available, each with its own strengths and weaknesses. In this literature review, we provide an overview of some of the most popular clustering methods and discuss their advantages and disadvantages applied to our dataset for NBA players clustering.

1. **Identifying and Characterizing Team Roles in the NBA using Player Tracking Data** by Lucey et al. (2014): This study used k-means clustering to identify player roles like "rim protector," "mid-range scorer," and "spot-up shooter."
2. **Clustering and Prediction of Basketball Players Based on their Scoring Behaviours** by Jin et al. (2019): This study used a Gaussian mixture model to identify player types like "shoot-first guards" and "rebounders and inside scorers."
3. **Clustering NBA Players Based on their Per-Game Statistics** by Kiritchenko and Mohammad (2018): This study used k-means clustering to categorize different player types like "scoring point guards" and "versatile forwards."
4. **Unsupervised Learning Techniques for Characterizing Playing Styles in the NBA** by Akhtar et al. (2016): This study used the DBSCAN clustering algorithm to distinguish between playing styles like "penetrators," "post players," and "perimeter shooters."

## DATA EXPLORATION AND ANALYSIS
Our analysis aims to explore the advanced statistics of NBA players in the 2019 season, focusing on identifying player archetypes based on their position. We obtained the dataset from the official NBA website, which contains 30 different attributes for 488 instances (i.e., individual players).

### Exploratory Data Analysis (EDA)
EDA helps us visualize the data and how it varies with other instances, visualize the correlation, and the distributions of the features with the given instances.

- **Figure 1:** Defence up position vs. Advanced AST percentage
- **Figure 2:** DREB vs. OREB percentages
- **Figure 3:** Heatmap representing the correlation among the features

## DATA MODELLING
The first step in any machine learning process is data cleaning, which involves pre-processing steps like exploring the dataset to visualize the distributions for various attributes and their correlation with each other and other features. This step gives us insights into the data. 

### Principal Component Analysis (PCA)
PCA is used for dimensionality reduction, retaining as much information as possible by finding a new set of orthogonal variables called principal components.

- **Figure 4a:** Variance vs. number of components
- **Figure 4b:** Difference in variance vs. number of components

### Clustering Algorithms
- **K-means Clustering:** Evaluated using the silhouette score to determine the optimal number of clusters.
- **Gaussian Mixture Models (GMMs):** Assumes data follows a Gaussian distribution.
- **Density-Based Spatial Clustering of Applications with Noise (DBSCAN):** Identifies clusters based on density.

- **Figure 5:** Flowchart representing the modelling of the algorithm development.

## RESULTS AND DISCUSSION
### Evaluation Metrics
- **Silhouette Score:** Measures how similar an object is to its own cluster compared to other clusters. 

- **Figure 6:** Variation of silhouette score and the number of clusters
- **Figure 7:** Differences in the slopes of silhouette score and the number of clusters

### Performance Analysis
- **Table 1:** Performance Analysis

| Analysis of the performance of models | Clustering model | Metric | Score |
|---------------------------------------|------------------|--------|-------|
| 1 | K-means | Silhouette | 0.13 |
| 2 | DBSCAN | Silhouette | 0.12 |
| 3 | Gaussian Models | Silhouette | 0.11 |

- **Figure 8a:** K-means Clusters
- **Figure 8b:** DBSCAN Clusters
- **Figure 8c:** Gaussian Model Clusters

## CONCLUSION AND FUTURE WORK
We have successfully implemented the clustering algorithms on the NBA dataset and assessed the models' performance. Although the DBSCAN model performed well, better metrics and optimized hyperparameters could improve performance. We are studying the underlying mathematics behind the models and exploring other models that may perform better.

## ACKNOWLEDGEMENT
We express our gratitude towards our professor for his hard work and the opportunity to select such an interesting topic. The explicit teaching helped us understand and manipulate the algorithms effectively.

## REFERENCES
1. J. Lucey, A. Bialkowski, P. Carr, S. Matthews, and I. Simon, "Identifying and characterizing team roles in the NBA using player tracking data," in IEEE Transactions on Visualization and Computer Graphics, vol. 20, no. 4, pp. 549-558, April 2014.
2. Y. Jin, S. Li, and X. Li, "Clustering and prediction of basketball players based on their scoring behaviors," in Journal of Sports Analytics, vol. 5, no. 3, pp. 139-152, Sep. 2019.
3. S. Kiritchenko and S. M. Mohammad, "Clustering NBA players based on their per-game statistics," in Proceedings of the First Workshop on NLP and Sports, 2018, pp. 30-39.
4. M. S. Akhtar, S. S. Ahmed, and A. El Saddik, "Unsupervised learning techniques for characterizing playing styles in the NBA," in Proceedings of the 2016 IEEE International Conference on Image Processing, 2016, pp. 3051-3055.
5. "NBA Advanced Stats: Player Analysis" by NBA.com: https://stats.nba.com/players/advanced/
6. A. Stern, "HoopDown," [Online]. Available: https://alexcstern.github.io/hoopDown.html. [Accessed: Apr. 26, 2023].
7. G. Hu, Y. Xue, and W. Shen, "Multidimensional heterogeneity learning for count value tensor data with applications to field goal attempt analysis of NBA players," arXiv preprint arXiv:2205.09918, May 2022.
8. F. Yin, G. Hu, and W. Shen, "Analysis of professional basketball field goal attempts via a Bayesian matrix clustering approach," arXiv preprint arXiv:2010.08495, Oct. 2020.
9. K. R. Shahapure and C. Nicholas, "Cluster Quality Analysis Using Silhouette Score," 2020 IEEE 7th International Conference on Data Science and Advanced Analytics (DSAA), Sydney, NSW, Australia, 2020, pp. 747-748, doi: 10.1109/DSAA49011.2020.00096.
10. Zhang, Shaoliang & Lorenzo Calvo, Alberto & Ruano, Miguel & Mateus, Nuno & Gonçalves, Bruno & Sampaio, Jaime. (2018).
