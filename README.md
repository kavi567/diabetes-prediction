Diabetes Prediction App Open in Streamlit
Streamlit Web App to predict the onset of diabetes based on diagnostic measures. For a walkthrough of the entire process of building the machine learning web application, have a look at the accompanying Medium article published in Towards AI.

Data
The data for the following example is originally from the National Institute of Diabetes and Digestive and Kidney Diseases and is available on Kaggle. The data contains information on females at least 21 years old of Pima Indian heritage. Since the data has been added to the data/ directory, cloning this repository would suffice.

Pre-requisites
The project was developed using Python 3.6.7 with the following packages.

Pandas
Numpy
Scikit-learn
Pandas-profiling(renamed as ydata_profiling)
Joblib
Streamlit
Installation with pip:

pip install -r requirements.txt
Getting Started
Open the terminal in your machine and run the following command to access the web application in your localhost.

streamlit run app.py
Run on Docker
Alternatively, you can build the Docker container and access the application at localhost:8051 on your browser.

docker build --tag app:1.0 .
docker run --publish 8051:8051 -it app:1.0
Files
diabetes_prediction_pipeline.ipynb : Jupyter Notebook with all the workings including pre-processing, modelling and inference.
app.py : Streamlit App script
requirements.txt : pre-requiste libraries for the project
models/ : trained model files and scaler objects
data/ : source data
Summary
This repository acts as a guide to [this blog post] where I talk about how I use Streamlit to build Machine Learning Applications quickly. Here we use a real-world example of predicting if a patient has diabetes and build a machine learning model. A Streamlit App was then built using a step-by-step approach in this project.

Acknowledgements
Kaggle, for providing the data for the machine learning pipeline.
Streamlit, for the open-source library for rapid prototyping.
