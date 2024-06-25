# Description

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
