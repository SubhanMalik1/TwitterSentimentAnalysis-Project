# Twitter Sentiment Analysis

This project analyzes tweet sentiment, classifying text as **positive** or **negative** using machine learning (logistic Regression ).

## Dataset
The **Twitter Sentiment Dataset** is available on Kaggle:
- [Dataset Link](https://www.kaggleusercontent.com/datasets/datasets/159112/twitter-sentiment-dataset)

### Steps:
1. Download the dataset from the provided link.
2. Authenticate with your Kaggle API key (`kaggle.json`).
3. Place the dataset in the appropriate directory.

## Workflow
1. **Data Loading**:
   - Load the dataset into a Pandas DataFrame.
   - Remove unnecessary or duplicate rows.
2. **Preprocessing**:
   - Convert sentiment values (4 to 1).
   - Clean text data (remove punctuations, special characters).
   - Apply stemming to normalize text.
3. **Train-Test Split**:
   - Split the cleaned data into **80% training** and **20% testing** sets.
4. **Training**:
   - Train a **Logistic Regression** model on the training set.
5. **Evaluation**:
   - Evaluate the model using Accuracy, Precision, Recall, and F1-score.

## Model
- **Model Used**: Logistic Regression
- **Reason**: Simple, interpretable, and performs well for text classification tasks.

## Setup
### Requirements:
1. **Python Version**: 3.7+
2. **Libraries**:
   - pandas
   - numpy
   - scikit-learn
   - nltk
   - kaggle

### Install Dependencies:
```bash
pip install pandas numpy scikit-learn nltk kaggle
```

## Usage
Follow these steps to run the project:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/SubhanMalik1/twitter-sentiment-analysis.git
   cd twitter-sentiment-analysis
   ```

2. **Setup Kaggle Access**:
   - Download your `kaggle.json` from Kaggle API credentials.
   - Place it in the root directory.
   - Run:
   ```bash
   kaggle datasets download -d kaggleusercontent/datasets/159112/twitter-sentiment-dataset
   unzip twitter-sentiment-dataset.zip
   ```

3. **Run the Notebook**:
   - Launch Jupyter Notebook:
   ```bash
   jupyter notebook tweet_sentiment_analysis.ipynb
   ```
   - Execute cells to train and evaluate the model.

## Results
The model achieves the following performance metrics:

| Metric       | Value    |
|--------------|----------|
| **Accuracy** | 0.7780125|

## Contributing
We welcome contributions! To contribute:
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes and push:
   ```bash
   git commit -m "Add new feature"
   git push origin feature-name
   ```
4. Submit a Pull Request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

