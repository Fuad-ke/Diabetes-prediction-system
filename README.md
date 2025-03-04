# Diabetes-prediction-system


This project is an interactive application built using Streamlit that integrates two key components:

Diabetes Prediction: A machine learning model that predicts whether a user is diabetic based on input data.
Diabetes Chatbot: A chatbot based on BERT (Bidirectional Encoder Representations from Transformers) that can answer diabetes-related questions by extracting relevant information from a provided context.

Features
Diabetes Prediction: Uses an LSTM-based deep learning model to predict diabetes based on user input.
Diabetes Chatbot: Implements a BERT-based chatbot to answer user questions on diabetes, such as symptoms, treatment options, risk factors, and more.
Metrics: Provides model accuracy and F1 score on the test set.
Technologies Used:

Streamlit: To build the interactive UI.
TensorFlow/Keras: For building the LSTM model to predict diabetes.
PyTorch: For implementing the BERT-based chatbot.
Scikit-learn: For data processing, train-test split, and model evaluation.
Pandas and Numpy: For data manipulation and numerical computation.
Transformers (Hugging Face): For utilizing BERT model for question-answering tasks.
How to Run the Project:

Clone the repository:

bash git clone https://github.com/your-username/diabetes-prediction-chatbot.git cd diabetes-prediction-chatbot

Install the required dependencies:

Ensure you have Python 3.x installed. Install the necessary packages by running:

bash pip install -r requirements.txt

The requirements.txt should include the following dependencies:

streamlit
pandas
numpy
scikit-learn
tensorflow
torch
transformers
Prepare the dataset:

Download the Diabetes dataset and ensure it is stored as diabetes.csv in the root directory of the project.

Run the Streamlit app:

Start the Streamlit application by running the following command:

bash streamlit run app.py

This will launch the web app, where you can input data for diabetes prediction and interact with the diabetes chatbot.

Diabetes Prediction
User Inputs:

The model takes in the following inputs for prediction:

Pregnancies: Number of pregnancies.
Glucose: Plasma glucose concentration.
Blood Pressure: Diastolic blood pressure (mm Hg).
Skin Thickness: Triceps skinfold thickness (mm).
Insulin: 2-Hour serum insulin (mu U/ml).
BMI: Body mass index (weight in kg/(height in m)^2).
Diabetes Pedigree Function: Diabetes pedigree function, which assesses the likelihood of diabetes based on family history.
Age: The person's age.
The model predicts whether the person is diabetic or not based on the input values.

Model:

An LSTM-based deep learning model is used for diabetes prediction. The model architecture includes three LSTM layers with Dropout layers for regularization.

Metrics:

The following metrics are provided:

Accuracy: Measures the model's accuracy on the test data.
F1 Score: Evaluates the balance between precision and recall.
Diabetes Chatbot:

The chatbot uses a pre-trained BERT model fine-tuned on the SQuAD dataset to answer questions related to diabetes. The context includes general information about diabetes symptoms, treatment, risk factors, and lifestyle management.

Usage:

Type in a question in the chatbot section of the sidebar, and the bot will provide an answer based on the context.

Future Improvements:

Advanced Diabetes Prediction: Consider incorporating additional data or advanced models to improve prediction accuracy.
Fine-tuning the Chatbot: Fine-tune the BERT model on a specific medical Q&A dataset to improve the chatbot's accuracy and relevance.
Real-time API Integration: Integrate with a real-time diabetes API for more dynamic answers to health-related queries.
License:

This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments:

UCI Machine Learning Repository for the diabetes dataset.
Hugging Face for the BERT model.
The Streamlit and TensorFlow communities for providing amazing tools to build this project.
