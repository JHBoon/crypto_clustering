# crypto_clustering
**University of California, Irvine – Data Analytics Bootcamp**  
Week 19: Machine Learning

## Project Overview
This project explores unsupervised machine learning techniques to segment a  set of cryptocurrencies based on their historical price behavior. The goal is to discover meaningful groupings among assets using K-Means clustering, a method well-suited for pattern detection in large datasets.

The project emphasizes practical use of clustering methods to analyze trends in crypto markets, leveraging a full data science workflow from preprocessing to modeling and visualization.

## Key Concepts and Workflow

### 1. Data Preprocessing
- Load and inspect cryptocurrency market data.
- Normalize and scale the data using `StandardScaler` to ensure uniform feature contribution during modeling.

### 2. K-Means Clustering & Elbow Graph
- Iterate over values of **k** from 1 to 10.
- For each k, train a K-Means model and record the **inertia**—a measure of clustering compactness.
- Plot an **elbow graph** to identify the optimal number of clusters; in this case, **k = 4**.

### 3. Dimensionality Reduction using PCA
- Apply **Principal Component Analysis (PCA)** to reduce the multi-dimensional dataset to 2 components.
- This enables intuitive, visual interpretation of the clusters.

### 4. Visualization with hvPlot
- Plot the reduced data using **hvPlot**, an interactive plotting library.
- Visualize how cryptocurrencies group together based on their scaled behaviors, making the model’s insights accessible to non-technical stakeholders.

## Results

The final output is an interactive 2D scatter plot of clustered cryptocurrencies. By interpreting the PCA-reduced graph, we can clearly identify groupings, outliers, and potential relationships among coins. This not only validates the clustering results but also provides a visual aid for further business or investment insights.

## Tools & Technologies

- **Languages & Libraries:** Python, Pandas, scikit-learn, hvPlot, PCA
- **IDEs:** Visual Studio Code
- **Support Resources:** ChatGPT, XpertAssistant Chat+, Stack Overflow, Bootcamp Class Notes

## How to Run the Project

1. Clone the repository.
2. Install required dependencies:
   ```bash
   pip install pandas scikit-learn hvplot
