# Urban-Housing-Analytics-Predicting-Cash-Rent-Trends
Building a predictive model to estimate cash rent prices based on features like Contract Housing rent, Aggregate household income in the past 12 months etc.

The features used are Contract Housing rent, Aggregate household income in the past 12 months, Housing unit value, Educational attainment for the population 25 and older, Public assistance income in the past 12 months.


STEPS:
1. Collect a dataset
2. Preprocess the data, handle missing values, perform EDA
3. Split the data into training and testing data
4. Build a regression model
5. Evaluate the model’s performance
6. Create visualisations to interpret the model’s predictions and feature importance.

STEP 1:
Data used:
1. Contract Housing rent - Location and neighbourhood features
2. Aggregate household income in the past 12 months - Income and economic indicators
3. Housing unit value - Housing Characteristics
4. Educational attainment for the population 25 and older - Demographic factors
5. Public assistance income in the past 12 months - Government assistance and social support
      
      Data was collected from Pittsburg American Community Servey 2015 - Miscellaneous data
      https://catalog.data.gov/dataset/pittsburgh-american-community-survey-2015-miscellaneous-data
      
The predictive model is based on a comprehensive dataset consisting of residential areas, economic indicators, housing characteristics, demographic factors, and social support measures. The dataset encompasses five key dimensions: Contract Housing Rent, providing insights into location and neighbourhood features; Aggregate Household Income in the Past 12 Months, offering crucial income and economic indicators; Housing Unit Value, housing characteristics; Educational Attainment for the Population 25 and Older, providing demographic insights; and Public Assistance Income in the Past 12 Months, shedding light on government assistance and social support. This multifaceted dataset was selected to capture the interplay of factors influencing housing prices. The inclusion of such diverse dimensions ensures a robust foundation for constructing a predictive model that encapsulates the intricate dynamics shaping housing markets.

STEP 2:
In the preprocessing phase of the data, a comprehensive approach was taken to ensure the dataset's readiness for subsequent analysis. Missing values were carefully addressed through a combination of imputation techniques, where appropriate, and data elimination when deemed necessary. The process involved a thorough exploration of the dataset to gain insights into its structure and identify patterns or trends. Additionally, feature engineering was performed to enhance the dataset's representational power, capturing relevant information that could contribute meaningfully to the subsequent analytical tasks. One-hot encoding was employed to transform categorical variables into a binary format, facilitating the incorporation of nominal data into machine learning models effectively. This step not only ensured a more robust and interpretable representation of the data but also set the stage for the application of advanced analytical techniques. Overall, the preprocessing and feature engineering steps aimed to create a clean, complete, and feature-rich dataset, laying a solid foundation for the subsequent stages of the analysis and modelling process.

STEP 3:
The merged dataset was divided into training and testing sets to ensure an unbiased evaluation of the regression model’s performance. This process involved allocating a portion of the data for model training, allowing it to learn patterns within the features. Simultaneously, a separate set was reserved for testing, enabling the assessment of the model's ability to generalize to new, unseen data. The common practice of an 80-20 split was adopted, with 80% of the data dedicated to training and 20% held out for testing. This strategic partitioning facilitated rigorous model evaluation and provided a reliable indication of its predictive capabilities on real-world data.

STEP 4:
This step constructed a regression model using the merged dataset, comprising features extracted from public assistance, educational, housing, and income data. The choice of a linear regression model was made to predict the target variable, "Estimate; With cash rent," based on various features. The dataset was split into training and testing sets to facilitate model training and performance evaluation.

STEP 5:
The performance of the regression model was assessed using standard evaluation metrics. Mean Squared Error (MSE) was employed to quantify the average squared difference between predicted and actual values. The model achieved an exceptionally low MSE, indicating a high level of accuracy. Additionally, R-squared was computed to measure the proportion of variance explained by the model, yielding a perfect score of 1.0, suggesting an excellent fit.

STEP 6:
Visualizations were crafted to provide insights into the model's predictions and feature importance. A scatter plot depicted the predicted values against the actual values, revealing a near-perfect alignment along the diagonal line. This indicated the model's effectiveness in capturing underlying patterns. Feature importance was visualized through a coefficients plot, showcasing the impact of each feature on the predictions. The model identified certain key features, such as "Total rent" and "Estimate; Aggregate household income," as significant contributors to the predictions.
