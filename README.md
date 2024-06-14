# Email and SMS Spam Detection

This repository contains an Email and SMS Spam Detection project using the Multinomial Naive Bayes algorithm. The project leverages natural language processing (NLP) techniques and machine learning to classify messages as either spam or not spam.

## Project Overview

The primary objective of this project is to build a machine learning model capable of distinguishing between spam and non-spam messages. The project includes data cleaning, exploratory data analysis (EDA), data preprocessing, model building, and deployment using Streamlit for a user-friendly interface.

## Features

- Data Cleaning: Removing unnecessary columns and handling missing values.
- Exploratory Data Analysis (EDA): Understanding the distribution and characteristics of the data.
- Data Preprocessing: Tokenization, stemming, and removal of stop words and punctuation.
- Model Building: Using Multinomial Naive Bayes for classification.
- Deployment: A web application using Streamlit to classify messages.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/spam-detection.git
    cd spam-detection
    ```

2. Create a virtual environment:
    ```bash
    python -m venv env
    ```

3. Activate the virtual environment:
    - On Windows:
        ```bash
        .\env\Scripts\activate
        ```
    - On macOS/Linux:
        ```bash
        source env/bin/activate
        ```

4. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

5. Download NLTK data:
    ```python
    import nltk
    nltk.download('punkt')
    nltk.download('stopwords')
    ```

## Usage

1. Ensure you are in the project directory and your virtual environment is activated.
2. Run the Streamlit application:
    ```bash
    streamlit run app.py
    ```
3. Open your browser and navigate to `http://localhost:8501` to interact with the web application.

## Project Structure
The project directory contains the following files:

Each file serves a specific purpose in the project:
- `app.py`: Contains the Streamlit application code that provides a web interface for the spam classifier.
- `main.ipynb`: Jupyter notebook for data processing, exploratory data analysis, and model building.
- `spam.csv`: Dataset used for training the spam detection model.
- `requirements.txt`: List of dependencies required to run the project.
- `vectorizer.pkl`: Serialized TfidfVectorizer used for transforming text data.
- `model.pkl`: Serialized Multinomial Naive Bayes model.
- `README.md`: Project documentation (this file).

## Data Preprocessing

The preprocessing steps include:

- Converting text to lowercase.
- Tokenization: Splitting text into individual words.
- Removing stop words and punctuation.
- Stemming: Reducing words to their root form using PorterStemmer.

## Model Building

- **Algorithm**: Multinomial Naive Bayes
- **Vectorization**: TfidfVectorizer with a maximum of 3000 features
- **Accuracy**: The model achieved an accuracy score of ` 97%` on the test set.

## Deployment

The model is deployed using Streamlit. Users can input a message, and the application will predict whether the message is spam or not.

## Results

The project demonstrates a practical application of NLP and machine learning in detecting spam messages. The Streamlit app provides an intuitive interface for users to interact with the model.





