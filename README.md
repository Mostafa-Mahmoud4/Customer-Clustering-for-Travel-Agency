# Customer-Clustering-for-Travel-Agency

## Project Overview
This project aims to analyze and segment travel agency customers based on their booking behavior using clustering techniques. By leveraging machine learning, particularly K-Means clustering, we can identify patterns in customer preferences and booking behaviors.

## Dataset
The dataset is sourced from a publicly available repository and contains booking data from a travel agency. It includes various features such as:
- **User Information**: `user_id`, `user_location_city`
- **Booking Details**: `date_time`, `srch_ci`, `srch_co`, `is_booking`
- **Trip Characteristics**: `duration`, `days_in_advance`, `orig_destination_distance`, `is_mobile`, `is_package`, `srch_adults_cnt`, `srch_children_cnt`, `srch_rm_cnt`

## Data Preprocessing
1. **Loading Data**: The dataset is imported from a CSV file and previewed.
2. **Exploratory Data Analysis (EDA)**:
   - Summary statistics and correlation matrix are computed.
   - Missing values are identified and handled.
   - Histograms and heatmaps are used for visualization.
3. **Feature Engineering**:
   - `duration`: Number of days between check-in and check-out.
   - `days_in_advance`: Days between booking date and check-in date.

## Clustering Approach
1. **Feature Selection**: Relevant numerical features are chosen for clustering.
2. **Data Standardization**: Features are standardized using `preprocessing.scale()` to ensure uniformity in magnitude.
3. **Clustering with K-Means**:
   - K-Means is applied with different values of `k` (2, 3, 4, and 6 clusters) to explore customer segmentation.
   - The Elbow Method and Silhouette Coefficient are used to determine the optimal number of clusters.
   - The final model uses `k=3` based on the evaluation results.

## Results
- Principal Component Analysis (PCA) is used for visualization.
- Clusters are analyzed to profile different customer segments.
- A bar chart is generated to visualize the distribution of users among clusters.

## Conclusion
This project provides valuable insights into customer behavior in the travel industry. The clustering results can be used to tailor marketing strategies, personalize offers, and enhance customer experience.

## Requirements
- Python 3.x
- Pandas, NumPy, Matplotlib, Seaborn, SciPy, Scikit-learn, Statsmodels, Pydot

## Running the Project
1. Clone the repository or download the dataset.
2. Install the required dependencies.
3. Run the Jupyter Notebook to execute the clustering analysis.
4. Visualize and interpret the results.

