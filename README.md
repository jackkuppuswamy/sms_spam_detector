# SMS Spam Text Classification using Gradio

This repository demonstrates a SMS spam text classification model. The model uses machine learning techniques to classify text messages as either spam or not spam (ham). Additionally, it incorporates a user interface built with Gradio for easy interaction with the model.

## Features
### 1. SMS Classification:
A pipeline is built using:
- TF-IDF Vectorization: Converts text into numerical representations.
- Linear Support Vector Classifier (LinearSVC): A robust classification algorithm.
### 2. Dataset:
- The dataset is loaded from a CSV file named SMSSpamCollection.csv containing two columns:
    - label: Specifies whether a message is "spam" or "ham".
    - text_message: The content of the text message.

### 3.Model Training:
- The data is split into training and testing sets (33% test size).
- A pipeline combines TF-IDF transformation with the LinearSVC classifier to train the model.

### 4.Prediction Function:
- Predicts whether a given text message is spam or not.
- The prediction is displayed using Gradio's interactive interface.

### Prerequisites
The following Python libraries are required:
- gradio
- pandas
- scikit-learn

### How to Use
- Load Dataset: Ensure that the SMSSpamCollection.csv file is in the Resources/ directory of your project.
- Run the Notebook: Execute the cells of the notebook sequentially to train the model.
- Interactive UI: The notebook uses Gradio to create an interface. You can input your text message and check if it is classified as spam or not.

### Files
- Notebook: gradio_sms_text_classification.ipynb
- Dataset: Resources/SMSSpamCollection.csv