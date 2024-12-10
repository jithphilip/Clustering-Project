# Report on Clustering of Liver Cirrhosis Data

Introduction: This Report focuses on the analysis of the dataset which contains features regarding Liver Cirrhosis. Cirrhosis results from prolonged liver damage, leading to extensive scarring, often due to conditions like hepatitis or chronic alcohol consumption. The goal is to develop a clustering model which will help us to identify the clusters of patients based on their Stage of disease.

Data Overview: Entries & Features: The dataset comprises of 25000 instances of 18 features. Key Features: Status, Drug, Hepatomegaly, Spiders, Edema, Bilirubin, Albumin, Alk_Phos, SGOT, Triglycerides, Platelets, Prothrombin, etc.

Data Cleaning & Preprocessing: Age variable has been converted into years from days. Outliers have been removed using the IQR Method.

Exploratory Data Analysis (EDA): Distribution of Age has been visualized using Histograms. Box Plot prior and post outlier removal have been visualized. Scatter plots for Triglycerides vs. Cholesterol & Alk_Phos vs. Cholesterol along with trendline. Pie chart & Double Bar Chart for other Categorical variables have also been plotted.

Model Development: Models Used: K-Means, DBSCAN, Gaussian Mixture Model.

Model Evaluation: Evaluation Metrics: Silhouette Score, Inertia (Used in Elbow Method)

Model Interpretation: Across the 3 models that have been used, Gaussian Mixture Model was the best performing in terms of Silhouette score followed by K-Means & DBSCAN. DBSCAN was the least performing with a Silhouette Score of 0.2839 even after merging the clusters. Although, K-Means had a silhouette score less than that of Gaussian Mixture Model, but the clusters formed were denser & clearly separable.

Conclusions: Key Findings: Gaussian Mixture Model was the best performing in terms of Silhouette score. Even though the Gaussian Mixture was the performing in terms of Silhouette Score, it had clusters overlapping due to its soft clustering.
