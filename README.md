# StockEcho - Sentiment Analysis Web App

This project is a sentiment analysis web application built with Flask, NLP, and machine learning. Users can enter a text message, and the model will predict its sentiment as Positive 😊, Neutral 😐, or Negative 😢.

## Features
- **User Input:** Enter a message and get sentiment prediction.
- **Text Preprocessing:** Tokenization, stopword removal, and stemming.
- **Machine Learning Model:** Uses scikit-learn for sentiment classification.
- **Flask Web Interface:** Provides a user-friendly interface for predictions.
- **Pickled Model & Vectorizer:** Loads a trained model and vectorizer for predictions.

## Installation & Setup

### Prerequisites
Make sure you have Python installed. Install the required dependencies:

```sh
pip install -r requirements.txt
```

### Run the Application

```sh
python app.py
```

The application will be accessible at `http://127.0.0.1:5050/`.

## File Structure

- `app.py` - Flask application to handle routes and predictions.
- `test.py` - Contains the `TextToNum` class for text preprocessing.
- `vectorizer.pickle` - Pre-trained vectorizer for transforming text.
- `model.pickle` - Trained sentiment analysis model.
- `templates/`
  - `index.html` - Home page with project overview.
  - `predict.html` - Input page for sentiment analysis.
  - `result.html` - Displays sentiment prediction results.
- `requirements.txt` - List of dependencies.

## How It Works
1. User enters a text message in the `predict.html` form.
2. The text is preprocessed (cleaning, tokenization, stemming).
3. The preprocessed text is transformed using `vectorizer.pickle`.
4. The model (`model.pickle`) predicts sentiment based on the processed text.
5. The result is displayed on `result.html`.

## Technologies Used
- **Backend:** Flask, scikit-learn, NLTK
- **Frontend:** HTML, CSS, JavaScript
- **Model:** Machine Learning with vectorized text processing

## Future Improvements
- Expand dataset for better accuracy.
- Implement deep learning for improved predictions.
- Add multilingual support.

## License
This project is open-source under the MIT License.
