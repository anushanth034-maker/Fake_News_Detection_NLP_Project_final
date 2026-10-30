# 📰 Fake News Detection Using NLP

## 📌 Project Overview

Fake News Detection Using NLP is a Machine Learning project that classifies news articles into two categories: **Fake News** and **Real News**.

The project uses Natural Language Processing (NLP) techniques and Machine Learning algorithms to analyse news content and identify patterns based on labelled training data.

The system converts text into numerical features using TF-IDF and applies classification algorithms to predict the category of a given news article.

**Note:** The model identifies patterns in its training dataset. Its predictions are not independent verification of whether news is factually true or false.

## 🎯 Objectives

- Develop a text classification system using NLP.
- Collect and preprocess labelled news datasets.
- Convert text into numerical features using TF-IDF.
- Train and compare Machine Learning algorithms.
- Evaluate model performance using standard metrics.
- Build an interactive web application using Streamlit.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| Pandas | Data processing |
| NumPy | Numerical operations |
| Scikit-learn | Machine Learning |
| NLTK | Natural Language Processing |
| TF-IDF | Text feature extraction |
| Matplotlib | Data visualisation |
| Streamlit | Web application |
| Jupyter Notebook | Model experimentation |

## 🧠 Machine Learning Algorithms

The project compares the following algorithms:

1. Logistic Regression
2. Multinomial Naive Bayes
3. Linear Support Vector Machine (SVM)

The best-performing model is selected using validation data.

## ⚙️ Project Workflow

1. **Dataset Collection:** Collect labelled real and fake news articles.
2. **Data Preprocessing:** Handle missing values, duplicates and unwanted text.
3. **Text Cleaning:** Convert text into a consistent format.
4. **Feature Extraction:** Apply TF-IDF vectorization.
5. **Model Training:** Train multiple classification algorithms.
6. **Model Selection:** Compare models using validation performance.
7. **Evaluation:** Calculate accuracy, precision, recall and F1-score.
8. **Web Application:** Display predictions through Streamlit.

## 📂 Project Structure

```text
Fake_News_Detection_NLP/
│
├── app.py
├── requirements.txt
├── README.md
│
├── data/
│   ├── news_dataset.csv
│   ├── Fake.csv
│   ├── True.csv
│   └── news_dataset_real.csv
│
├── src/
│   ├── preprocessing.py
│   ├── prepare_dataset.py
│   └── train.py
│
├── models/
│   └── fake_news_pipeline.joblib
│
├── reports/
│   ├── evaluation.json
│   ├── confusion_matrix.csv
│   └── confusion_matrix.png
│
└── tests/
    └── test_project.py
```

*Note: The dataset files and generated model/report files should be added only when available. Do not upload large datasets or generated model files without checking repository size and dataset redistribution terms.*

## 💻 Installation and Setup

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Navigate to the project directory

```bash
cd Fake_News_Detection_NLP
```

### 3. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Prepare the dataset

Place the required dataset CSV files inside the `data` directory.

For the ISOT dataset, use `Fake.csv` and `True.csv`.

Run:

```bash
python src/prepare_dataset.py
```

### 5. Train the Machine Learning models

```bash
python src/train.py --data data/news_dataset_real.csv
```

### 6. Run the Streamlit application

```bash
python -m streamlit run app.py
```

## 📊 Model Evaluation

The project evaluates classification performance using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

Actual evaluation results will be documented after training with the selected real-world dataset.

## 🧪 Testing

The project includes automated tests for:

- Text cleaning
- Lowercase conversion
- URL removal
- Punctuation removal
- Empty input handling
- Missing column validation
- Label normalisation
- Duplicate removal
- Model training and prediction

Run the tests using:

```bash
python -m unittest discover -s tests -v
```

**Initial testing:** 9 out of 9 tests passed.

These tests verify basic functionality; they do not establish real-world model accuracy.

## 🌐 Application Features

- User-friendly Streamlit interface.
- News text input.
- Automated text classification.
- Fake-like and real-like prediction display.
- Clear explanation of prediction limitations.

## ⚠️ Limitations

- Predictions depend on the quality of the training dataset.
- The model may misclassify unfamiliar news content.
- Dataset bias can affect model performance.
- Classification does not establish factual accuracy.
- Human fact-checking is still necessary.

## 🚀 Future Enhancements

- Improve model performance using larger and more diverse datasets.
- Explore advanced NLP techniques.
- Add confidence and explanation features where appropriately calibrated.
- Improve the user interface.
- Integrate trusted external fact-checking sources.

## 👩‍💻 Author

**Anushanth S**

B.Tech – Artificial Intelligence and Data Science

## 📌 Project Status

**Development in Progress**

This project is being developed as a practical implementation of Natural Language Processing and Machine Learning concepts.

---

*Built using Python, NLP and Machine Learning.*
