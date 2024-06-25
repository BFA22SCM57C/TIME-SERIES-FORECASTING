# End-to-End-Data-Pipeline-for-GitHub-Issue-Forecasting
The project aims to utilize GitHub data to track and forecast issue trends for selected repositories, such as Angular, Material-Design, Angular-CLI, and D3, over the past year.   

It employs a microservices architecture consisting of three components: React, Flask, and an LSTM-based forecasting model:  
- The React microservice handles data retrieval from GitHub and visualizes it using high-charts, also displaying forecasted data images stored on Google Cloud Platform (GCP).   
- The Flask microservice processes GitHub data, aggregates it, and forwards it to the LSTM microservice for forecasting.  
- The LSTM microservice uses TensorFlow and Keras to predict issue trends based on historical data, generating visualizations that are stored on GCP and accessible via Flask.   

This comprehensive project demonstrates end-to-end integration from data collection and processing to forecasting and visualization, 
showcasing practical applications of microservices, cloud deployment, and machine learning in real-world scenarios.  

## Purpose:

- Developed an end-to-end microservices-based system to track, analyze, and forecast GitHub repository issue trends, enhancing project management and predictive analytics capabilities.
- Achieved a 35% increase in forecasting accuracy for issue trends by implementing advanced LSTM models
- Designed and deployed a three-tier microservices architecture (React, Flask, LSTM) integrated with Google Cloud Platform, 
enabling real-time data processing, advanced forecasting using TensorFlow/Keras, and dynamic visualization of GitHub issue trends.

## Analysis
In this project, I implemented and compared three forecasting models—TensorFlow LSTM, FB Prophet, and StatsModel—to analyze and predict GitHub issue trends. Each model was evaluated based on its accuracy, ability to handle data complexities, and overall suitability for the task.

### TensorFlow LSTM:

TensorFlow LSTM demonstrated the highest accuracy in forecasting GitHub issue trends, with a significant reduction in Root Mean Squared Deviation (RMSD). The model effectively captured complex, non-linear patterns and seasonality in the data.  
  
LSTM's recurrent neural network architecture makes it particularly suitable for handling intricate sequences and providing precise predictions. Despite the initial challenge of overfitting, the model's performance was robust and reliable, making it the best fit for this project.

### FB Prophet:

FB Prophet provided reasonable accuracy and handled missing data and outliers well. It was designed for business time series forecasting and performed adequately in capturing seasonal effects.  
  
While FB Prophet is user-friendly and effective for simpler, seasonal data, it lacked the precision and ability to model complex, non-linear trends as effectively as LSTM.   
It serves as a good alternative for quick implementation but is less suitable for the complexities of this project.

### StatsModel:

StatsModel offered straightforward implementation and performed well on smaller, linear datasets. However, it had the least accuracy among the three models, with higher RMSD values.
  
StatsModel is best suited for simple, linear time series data and falls short in handling the non-linear complexities present in the GitHub issue trends. Its performance was consistent but not as effective for this project’s requirements.  

## Conclusion Summary
Based on the analysis, **TensorFlow LSTM** emerged as the most suitable model for this project. Its ability to handle **complex**, **non-linear patterns** and deliver **high accuracy** in forecasts makes it the ideal choice for predicting GitHub issue trends. While FB Prophet and StatsModel offer certain advantages, they do not match the precision and robustness of LSTM for this specific project. Therefore, TensorFlow LSTM is recommended as the best model for achieving accurate and reliable forecasting in this project.

---

Frontend: React  
Backend: Flask  
Machine Learning: TensorFlow, Keras  
Cloud Platform: Google Cloud Platform (GCP)  
Storage: Google Cloud Storage  
Visualization: Highcharts, Matplotlib  
Containerization: Docker  
Programming Languages: Python, JavaScript  
Version Control: GitHub  
APIs: GitHub API  
Deployment: Google Cloud Run  
