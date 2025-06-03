# 🍷 Wine Quality Predictor

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![ML](https://img.shields.io/badge/Machine%20Learning-XGBoost%20|%20SVC%20|%20LogisticRegression-orange)](https://scikit-learn.org/)

A machine learning project that predicts wine quality (0-10 scale) based on physicochemical properties. Achieves 82% accuracy using XGBoost classifier.

![Confusion Matrix](https://via.placeholder.com/600x400?text=Confusion+Matrix+Example) <!-- Replace with actual plot -->

## Features
- **Comprehensive EDA** with histograms, correlation heatmaps, and feature analysis
- **Multiple ML models** comparison (XGBoost, SVM, Logistic Regression)
- **Advanced preprocessing** with missing value imputation and feature scaling
- **Model evaluation** using ROC-AUC scores and classification reports
- **Clean codebase** with PEP8 compliance and modular structure

## 📚 Importing Libraries and Dataset

To handle and analyze the wine quality dataset, the following Python libraries are essential:

- **🐼 Pandas**: For data manipulation and analysis.
- **🔢 NumPy**: For working with arrays and matrices.
- **📊 Seaborn/Matplotlib**: For creating beautiful data visualizations.
- **🤖 scikit-learn (sklearn)**: For machine learning tasks—preprocessing, modeling, and evaluation.
- **🚀 XGBoost**: For advanced boosting-based machine learning.

## Installation
1. Clone repository:
   git clone https://github.com/yourusername/wine-quality-predictor.git
   cd wine-quality-predictor

2. Install dependencies:
   pip install -r requirements.txt


## Usage
## Sample training code
from xgboost import XGBClassifier
from sklearn.preprocessing import MinMaxScaler

## Load and preprocess data
df = pd.read_csv('winequalityN.csv')
... [preprocessing steps]

## Train model
model = XGBClassifier()
model.fit(xtrain, ytrain)

## Dataset
Contains 11 fundamental wine features:
- Fixed acidity
- Volatile acidity
- Citric acid
- Residual sugar
- Chlorides
- Free sulfur dioxide
- Density
- pH
- Sulphates
- Alcohol
- Quality (target)

## Model Performance
| Model                | Training AUC | Validation AUC |
|----------------------|--------------|----------------|
| Logistic Regression  | 0.70         | 0.69           |
| XGBoost              | 0.98         | 0.80           |
| SVM (RBF Kernel)     | 0.72         | 0.71           |

**Best Model (XGBoost) Classification Report:**
          precision    recall  f1-score   support
       0       0.76      0.74      0.75       474
       1       0.86      0.86      0.86       826
accuracy                           0.82      1300


## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

## License
Distributed under the MIT License. See `LICENSE` for more information.

## Credits
- **Adityabaan Tripathy** - Initial work
- Wine Quality Dataset - [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/wine+quality)

