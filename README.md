  # Sentiment-Analysis-on-IMDB-movie-review
# IMDB Movie Reviews Sentiment Analysis - My Cool Project! 

Hey everyone! This is my project on sentiment analysis of IMDB movie reviews. I used Python and some cool libraries like NLTK, pandas, and scikit-learn to build this.  I even learned about session management to make the analysis process smoother and more efficient. Let me walk you through it!

## What's This All About? 

Sentiment analysis is like figuring out if a movie review is positive or negative, just by looking at the words used.  This project uses a dataset of 50,000 IMDB movie reviews, each labeled as positive or negative. The goal is to build a model that can automatically predict the sentiment of a new review. 

## Session Management: The Secret Sauce 

Session management is a fancy term for keeping track of important stuff during the analysis. It's like having a virtual backpack where you store your tools and results so you don't have to keep searching for them. Here's how it works:

1. **Setting Up:** When you start the Jupyter Notebook, it creates a session just for your analysis. Think of it as a workspace dedicated to your project.
2. **Cleaning Up:**  First, we clean up the movie reviews.  This means removing HTML tags, converting everything to lowercase, and getting rid of unnecessary words (like "the", "a", "is"). We store this cleaned data in the session so we can access it later.
3. **Making Sense of Words:** We use TF-IDF to convert words into numbers that the computer can understand. It's like creating a secret code for the words in the reviews. We store this codebook (the TF-IDF vectorizer) in our session too.
4. **Training the Brain:**  Now, we train a machine learning model called Multinomial Naive Bayes (MNB).  We show it lots of examples of positive and negative reviews and teach it to recognize the patterns. The trained model is safely stored in our session backpack.
5. **Saving Progress:**  Using a tool called `pickle`, we save the important things like our trained model and vectorizer to files. This is like taking a snapshot of our progress. We can load these files later to resume our work without starting from scratch!
6. **Making Predictions:** When we have a new movie review, we use the saved model and vectorizer to predict its sentiment. It's like asking our trained brain for its opinion.

## Why is Session Management Cool? 

* **No More Repeats!** We don't have to re-do the cleaning, feature extraction, or model training every time. The session remembers our work. This saves time and makes the analysis much faster.
* **Everything in One Place!**  The session keeps all the important data and tools organized and readily available. No more searching for files or variables.
* **Smart Predictions:**  The session helps maintain the context of the analysis, so the model can make more accurate predictions.

## How to Use This Project 

1. Open the Jupyter Notebook.
2. Run the code cells in order (from top to bottom). This ensures the session is set up correctly.
3. If you want to stop and resume later, make sure to save your notebook!  When you reload the notebook, you can reload your session using the `pickle` code.

## Conclusion 

This project was a fun way to learn about sentiment analysis and the power of session management. I hope you find it interesting and helpful! 😊
