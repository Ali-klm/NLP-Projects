Overview
The notebook is divided into two main parts:

Part 1: CNN-based Models
IMDB Dataset (English Movie Reviews)

Uses the IMDB movie reviews dataset for binary sentiment classification.

Implements multiple CNN architectures with varying embedding dimensions, filter sizes, and max-pooling configurations.

Evaluates models using accuracy, precision, recall, F1-score, and confusion matrix.

Persian Text Sentiment Dataset

Loads and preprocesses a Persian sentiment dataset using datasets library.

Tokenizes Persian text and trains CNN models similar to the IMDB part.

Model evaluation with standard classification metrics.

Persian News Dataset

Loads a large-scale Persian news dataset.

Preprocesses texts and categories for multi-class classification.

Trains CNN models and reports precision, recall, accuracy, F1-score for each news category.

Part 2: CNN + LSTM Hybrid Models with Pre-trained Embeddings
IMDB Dataset

Builds a hybrid CNN-LSTM model.

Utilizes pre-trained GloVe embeddings for better word representations.

Model training and evaluation with detailed classification metrics.

Persian Text Sentiment Dataset

Similar CNN-LSTM architecture applied to Persian sentiment data.

Uses pre-trained embeddings and evaluates model performance.

Persian News Dataset

Extends the CNN-LSTM model to multi-class Persian news classification.

Reports metrics per category with confusion matrix visualization.