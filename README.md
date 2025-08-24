📊 Unlocking YouTube Channel Performance Secrets  

This project analyzes YouTube channel performance data to uncover key factors that influence video success and revenue.  
By combining data analysis, visualization, and machine learning, we build a model to predict Estimated Revenue (USD) for YouTube videos. 

📌 Project Overview  

- YouTube creators produce massive amounts of data (views, likes, watch time, CTR, etc.).  
- Understanding which factors drive higher revenue is crucial for channel growth.  
- Using this dataset, we explore relationships, identify top drivers, and build a Random Forest regression model.  
- The project also highlights top-performing videos and provides actionable insights for creators.  

 🗂 Dataset  

- The dataset contains detailed video-level analytics, including:  
  - Views, Subscribers, Impressions  
  - Watch Duration & Average View Percentage  
  - Likes, Shares, Comments (Engagement metrics)  
  - CTR (Click-Through Rate)  
  - Estimated Revenue (Target variable)  
  - Video Publish Time & Duration 
 🛠 Workflow  

 1. Data Preprocessing  
- Parse publish time into datetime.  
- Convert Video Duration into numeric values.  
- Handle missing values with median imputation.  

 2. Feature Engineering  
- *Revenue per View* = Revenue ÷ Views  
- *Engagement Rate* = (Likes + Shares + Comments) ÷ Views × 100  
- Extract publish_hour and publish_dayofweek.  

 3. Exploratory Data Analysis (EDA)  
- Revenue distribution histogram  
- Scatter plot: Views vs. Revenue (log-log scale)  
- Correlation heatmap  
- Pairplot of Views, Subscribers, and Revenue  
- Top 10 highest revenue-generating videos  

 4. Modeling  
- Split into train/test sets (80/20).  
- Train a Random Forest Regressor.  
- Evaluate with RMSE and R².  

 5. Feature Importance  
- Identify top features influencing revenue (e.g., Views, CTR, Watch Duration).  

 6. Predictions  
- Save model and imputer with joblib.  
- Provide predict_sample() function to estimate revenue for a new video input.  

Conclusion

This project demonstrates how data-driven insights can help YouTube creators:
Identify what drives revenue.
Pinpoint top-performing vs underperforming videos.
Predict estimated revenue for new content.

📊 Ultimately, it shows the power of Machine Learning and Analytics in improving YouTube channel growth and success.
