# OIBSIP_task4

# Email Spam Detector

This is a simple Python script that demonstrates how to train a machine learning model to classify emails into spam and non-spam categories. It uses the Multinomial Naive Bayes classifier and TF-IDF vectorization to process the email text.

## Getting Started

### Prerequisites

- Python 3.x
- Pandas
- Scikit-Learn

You can install the required libraries using pip:

```
pip install pandas scikit-learn
```

### Usage

1. Clone this repository or download the `spam_detector.py` script.

2. Prepare your dataset with two columns, 'v1' (labels - spam or non-spam) and 'v2' (email text), and save it as a CSV file. Make sure to replace `'your_dataset.csv'` in the script with the path to your dataset.

3. Run the script:

```
python spam_detector.py
```

4. The script will split your dataset into training and testing sets, preprocess the text using TF-IDF vectorization, train the Multinomial Naive Bayes classifier, and evaluate the model's performance.

### Customization

You can customize the script by adjusting the following parameters:

- `max_features`: Limit the number of features in the TF-IDF vectorizer to control memory usage and model complexity.

- Machine learning model: Replace the Multinomial Naive Bayes classifier with other algorithms available in Scikit-Learn for text classification.

- Hyperparameters: Experiment with different hyperparameters for your chosen machine learning algorithm to optimize performance.

### Dataset

Ensure that your dataset is well-labeled with 'spam' and 'ham' (non-spam) labels in the 'v1' column and corresponding email text in the 'v2' column.

### Evaluation

The script provides the following evaluation metrics:

- Accuracy: Measures the overall correctness of predictions.
- Confusion Matrix: Shows the count of true positive, true negative, false positive, and false negative predictions.
- Classification Report: Provides precision, recall, F1-score, and support for each class (spam and non-spam).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- This code is for educational purposes and can serve as a starting point for building more advanced spam detectors.
- Special thanks to the Scikit-Learn and Pandas communities for their excellent libraries.

