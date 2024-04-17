
# Box Office Revenue Prediction Using Linear Regression in Machine Learning

## Introduction
This project focuses on predicting the box office revenue of movies using machine learning techniques. By leveraging movie genres and other related features, we aim to develop a model that can forecast the potential revenue of a movie. In this README, I'll provide an overview of the project, including the dataset, data preprocessing steps, exploratory data analysis (EDA), model development, and evaluation.

## Dataset
The dataset used in this project contains information about movies, including features such as genre, budget, MPAA rating, opening theaters, release days, and domestic revenue. The dataset comprises 2694 entries with 10 columns initially.

## Libraries Used
- Pandas: For data manipulation and analysis.
- Numpy: For numerical computations.
- Matplotlib and Seaborn: For data visualization.
- Scikit-learn: For model development and evaluation.
- XGBoost: For implementing the XGBoost regressor algorithm.

## Data Preprocessing
- Removal of irrelevant columns: Columns such as 'world_revenue' and 'opening_revenue' were removed as they were not relevant to the prediction task.
- Handling missing values: Null values in columns such as 'MPAA' and 'genres' were imputed with the mode of the respective columns, and rows with remaining null values were dropped.
- Data type conversion: Certain columns like 'domestic_revenue', 'opening_theaters', and 'release_days' were converted to numeric format after removing commas and dollar signs.
- Log transformation: To address outliers, a log transformation was applied to certain features.

## Exploratory Data Analysis (EDA)
EDA was performed to understand the distribution of features and relationships between variables. Visualizations such as count plots, distribution plots, and box plots were utilized to explore the data. Key insights were derived regarding the impact of movie ratings and various features on domestic revenue.

## Feature Engineering
- Creation of features from genre: CountVectorizer was used to convert movie genres into binary features.
- Removal of rare genres: Genres with less than 5% occurrence were removed to simplify the model.

## Model Development
- Features and target variable separation: Features such as movie title and financial features were separated from the target variable (domestic revenue).
- Data normalization: StandardScaler was used to normalize the features for stable and efficient training.
- Model selection: XGBoost regressor was chosen for model training due to its effectiveness in achieving high prediction accuracy.

## Model Evaluation
- Mean Absolute Error (MAE) was used as the evaluation metric.
- Training and validation errors were calculated to assess model performance.

## Conclusion
The developed model demonstrates promising results in predicting box office revenue based on movie genres and other relevant features. Further refinements and optimizations can be explored to enhance the model's performance and applicability in the film industry.

Feel free to explore the provided code and dataset for detailed insights into the project. If you have any questions or suggestions, please don't hesitate to reach out. Happy coding!
