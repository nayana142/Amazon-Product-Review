# Amazon Product Review Sentiment Analysis
![proj_7](https://github.com/user-attachments/assets/d637dddb-d96b-4ae0-8da0-485dec134adb)
![Screenshot 2025-01-17 123513](https://github.com/user-attachments/assets/f74686a5-e921-4d13-afc9-0530336ecab3)


## Overview

The Amazon Product Review Sentiment Analysis project is designed to analyze customer reviews of Amazon products and classify them as either Positive or Negative. This tool leverages Machine Learning and Natural Language Processing (NLP) techniques and provides a user-friendly Flask web application for real-time sentiment analysis.

## Features

        1.Sentiment Analysis: Predicts whether a given review is positive or negative.
        
        2.Interactive Web Application: Built using Flask for seamless user interaction.
        
        3.Real-Time Predictions: Processes and analyzes user input instantly.
        
        4.Clear Button: Clears inputs for new predictions.

## Process

1. Data Preprocessing

        Text Cleaning: Removed HTML tags, punctuation, numbers, and newline characters.
        
        Stopword Removal: Filtered out commonly used words that do not add value to the sentiment analysis.
        
        Stemming: Reduced words to their root forms using SnowballStemmer.

2. Model Development

        Algorithm: Logistic Regression was used as the classification model.
        
        Training Data: The model was trained on a dataset of labeled Amazon product reviews.
        
        Vectorization: Used CountVectorizer or TF-IDF Vectorizer to convert text into numerical data.

3. Web Application

        Flask Framework: Created a web interface for users to input reviews.
        
        Frontend Design: Used HTML and CSS to create a responsive and visually appealing design.
        
        Prediction Display: Shows whether the review is Positive or Negative.
        
        Clear Button: Allows users to reset the form and input a new review.

4. Deployment

        The application can be deployed on any local server or cloud platform for public access.

## How to Run the Project

### Prerequisites

    Flask
    
    NLTK
    
    Scikit-learn
    
    Joblib
    
    Installation

### Clone the repository:

    git clone https://github.com/nayana142/Amazon-Product-Review-Analysis.git
    cd Amazon-Product-Review-Analysis

### Install the required dependencies:

    pip install -r requirements.txt

### Download NLTK data:

    import nltk
    nltk.download('stopwords')

### Run the Application

    Start the Flask server:
    
    python app.py

### Open your browser and visit:

    http://127.0.0.1:5000

## File Structure

        Amazon-Product-Review-Analysis/
        ├── app.py               # Flask application
        ├── model.pkl            # Trained Logistic Regression model
        ├── vectorizer.pkl       # Saved CountVectorizer or TF-IDF Vectorizer
        ├── templates/           # HTML templates
        │   └── index.html       # Main web page
        ├── static/              # Static files (CSS, images)
        │   ├── style.css        # Styling for the web app
        │   └── reviews-stars.jpg# Background image
        ├── requirements.txt     # Dependencies
        └── README.md            # Project documentation

## Technologies Used

1.Programming Language: Python

2.Machine Learning: Scikit-learn

NLP: NLTK

4.Web Framework: Flask

5.Frontend: HTML, CSS
