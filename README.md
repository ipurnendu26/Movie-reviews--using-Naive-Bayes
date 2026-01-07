# 🎬 Movie Reviews Sentiment Analysis using Naive Bayes

A machine learning project that performs sentiment analysis on IMDB movie reviews using the Naive Bayes classifier. This project follows the complete Data Science lifecycle from data loading to model evaluation.

![Python](https://img.shields.io/badge/Python-3.11-blue.svg)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3+-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Data Science Lifecycle](#data-science-lifecycle)
- [Results](#results)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

This project analyzes IMDB movie reviews to classify them as **positive** or **negative** sentiment using Natural Language Processing (NLP) techniques and the Multinomial Naive Bayes algorithm. The dataset contains 50,000 movie reviews with balanced positive and negative sentiments.

## ✨ Features

- **Data Cleaning**: Removes HTML tags, URLs, special characters, and normalizes text
- **Exploratory Data Analysis**: Comprehensive visualization of data distributions
- **Multiple Vectorization Methods**: Implements both Count Vectorizer and TF-IDF
- **Model Comparison**: Compares performance of different feature extraction methods
- **Interactive Predictions**: Predict sentiment on new custom reviews
- **Feature Importance Analysis**: Identifies top words indicating positive/negative sentiment

## 📁 Project Structure

```
Movie-reviews--using-Naive-Bayes/
│
├── Movie reviews.ipynb    # Main Jupyter notebook with complete analysis
├── IMDB Dataset.csv       # Dataset with 50,000 movie reviews
├── requirements.txt       # Python dependencies
├── README.md              # Project documentation
└── .venv/                 # Virtual environment (not tracked)
```

## 🚀 Installation

### Prerequisites

- Python 3.11 or higher
- pip (Python package manager)

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/Movie-reviews--using-Naive-Bayes.git
   cd Movie-reviews--using-Naive-Bayes
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv .venv
   ```

3. **Activate the virtual environment**
   
   - Windows:
     ```bash
     .venv\Scripts\activate
     ```
   - macOS/Linux:
     ```bash
     source .venv/bin/activate
     ```

4. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## 💻 Usage

1. **Open the Jupyter Notebook**
   ```bash
   jupyter notebook "Movie reviews.ipynb"
   ```
   Or open in VS Code with the Jupyter extension.

2. **Run all cells** sequentially from top to bottom

3. **Predict on custom reviews** using the `predict_sentiment()` function:
   ```python
   review = "This movie was fantastic! Great acting and storyline."
   sentiment, confidence = predict_sentiment(review, nb_cv, count_vectorizer)
   print(f"Sentiment: {sentiment}, Confidence: {confidence:.1f}%")
   ```

## 📊 Data Science Lifecycle

The notebook follows these stages:

| Stage | Description |
|-------|-------------|
| **1. Data Loading** | Import IMDB dataset with 50,000 reviews |
| **2. Data Cleaning** | Handle missing values, duplicates, text preprocessing |
| **3. EDA** | Visualize sentiment distribution, review lengths, common words |
| **4. Feature Engineering** | Apply Count Vectorization and TF-IDF |
| **5. Model Building** | Train Multinomial Naive Bayes classifiers |
| **6. Model Evaluation** | Accuracy, Classification Report, Confusion Matrix, ROC Curve |

## 📈 Results

### Model Performance

| Model | Accuracy | AUC-ROC |
|-------|----------|---------|
| Naive Bayes (Count Vectorizer) | ~86% | ~93% |
| Naive Bayes (TF-IDF) | ~86% | ~93% |

### Key Findings

- ✅ Both models achieve high accuracy (>85%)
- ✅ Dataset is perfectly balanced (50% positive, 50% negative)
- ✅ Words like "excellent", "great", "best" strongly indicate positive sentiment
- ✅ Words like "worst", "terrible", "waste" strongly indicate negative sentiment

### Sample Predictions

| Review | Prediction | Confidence |
|--------|------------|------------|
| "This movie was absolutely amazing!" | POSITIVE 😊 | 95% |
| "Terrible film. Waste of time." | NEGATIVE 😞 | 92% |

## 🛠️ Technologies Used

- **Python 3.11** - Programming language
- **pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical visualization
- **scikit-learn** - Machine learning library
- **Jupyter Notebook** - Interactive development environment

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Purnendu Kale**

---

⭐ Star this repository if you found it helpful!
