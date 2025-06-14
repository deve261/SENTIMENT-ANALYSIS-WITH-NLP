# SENTIMENT-ANALYSIS-WITH-NLP

COMPANY: CODTECH IT SOLUTIONS

NAME: YELLANKI DEVENDRA

INTERN ID: CT04DG224

DOMAIN: MACHINE LEARNING

DURATION: 4 WEEKS

MENTOR: NEELA SANTOSH

PROJECT DESCRIPTION : Customer Review Sentiment Analyzer with Interactive Gradio Interface
This project implements a machine learning-powered sentiment analysis tool with a user-friendly graphical interface using Gradio, designed to classify customer reviews into predefined sentiment categories such as positive, neutral, or negative. The model is built using Python, leveraging prominent machine learning libraries like scikit-learn and pandas, and is intended to make sentiment analysis accessible even to non-technical users.

The application accepts raw textual input in the form of customer reviews and provides real-time sentiment predictions. It is particularly useful for businesses and analysts aiming to gain quick and automated insights from user feedback without the need to manually read through large volumes of reviews.

1. Data Loading and Preprocessing
At the heart of the application is a dataset of customer reviews, stored in a CSV file named customer_reviews.csv. The dataset consists of two main columns:

review: The textual feedback provided by the customer.

sentiment: The label indicating the sentiment associated with the review (e.g., positive, negative, or neutral).

Using pandas, the script loads the dataset into a DataFrame and separates the features (X) from the labels (y). Text data being inherently unstructured requires preprocessing before it can be used in machine learning models. For this, the project utilizes TF-IDF vectorization through TfidfVectorizer from scikit-learn. TF-IDF (Term Frequency-Inverse Document Frequency) helps convert textual data into meaningful numerical vectors by assessing the importance of words in the document relative to the corpus, while removing common stopwords.

2. Model Training and Evaluation
Once the reviews are vectorized, the dataset is split into training and testing subsets using an 80/20 ratio. The model chosen for this task is Logistic Regression, a simple yet effective linear classifier that performs well in text classification problems like sentiment analysis. The training is performed using model.fit() on the transformed text vectors.

To ensure the model's quality, accuracy metrics and a classification report can be computed using accuracy_score and classification_report from sklearn.metrics. These measures help evaluate how well the model generalizes to unseen data and highlight performance across each sentiment class.

3. Real-Time Sentiment Prediction
The prediction functionality is encapsulated in a function predict_sentiment(text) which takes a raw text input, vectorizes it using the same TF-IDF model that was fit on the training data, and returns the predicted sentiment label. This function ensures that users can input any arbitrary review and receive an instant assessment of its emotional tone.

4. Gradio Interface
To make the model easily accessible, the application integrates Gradio, an open-source library that allows developers to create customizable and interactive interfaces for machine learning models. The Gradio interface wraps the predict_sentiment function with a clean layout, consisting of:

Input textbox: Allows the user to type or paste a customer review.

Output textbox: Displays the predicted sentiment as a result.

Title and Description: Provides context for the app and guides the user.

This interface runs in a web browser, offering a simple and portable deployment mechanism that can even be shared with stakeholders via a link.

5. Applications and Use Cases
This sentiment analysis tool can be employed across a wide range of industries and scenarios:

E-commerce: Analyze customer reviews for products and services to gauge satisfaction.

Hospitality: Understand guest feedback from hotel or restaurant reviews.

Social Media Monitoring: Assess public sentiment toward brands or events.

Customer Support: Identify negative feedback for prompt issue resolution.

6. Benefits and Extensibility
The project is lightweight, easily extendable, and serves as a solid foundation for building more advanced Natural Language Processing (NLP) applications. Developers can enhance it further by:

Adding support for multilingual reviews.

Integrating more advanced models like BERT or LSTM.

Expanding the dataset for greater accuracy.

Visualizing sentiment trends over time.

#OUTPUT :
