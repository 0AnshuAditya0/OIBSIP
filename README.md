# OIBSIP Data Science

This repository contains 5 machine learning projects completed as part of the **OIBSIP Data Science **.

Each task is a self-contained Jupyter Notebook with complete data analysis, visualization, model training, and evaluation.

---

## Repository Structure

```
OIBSIP/
├── Task_1/                          
│   └── iris_classification.ipynb                      
│
├── Task_2/                         
│   └── unemployment_analysis.ipynb             
│
├── Task_3/                         
│   └── car_price_prediction.ipynb            
│
├── Task_4/                        
│   └── spam_detection.ipynb                     
│
├── Task_5/                          
│   └── sales_prediction.ipynb                 
│
└── README.md                    
```

---

## Quick Start

### Prerequisites

- Python 3.9 or higher
- pip (Python package manager)

### Setup Instructions

1. **Clone or download this repository**

2. **Navigate to any task folder**
   ```bash
   cd Task_1   # or Task_2, Task_3, etc.
   ```

3. **Create a virtual environment (recommended)**
   ```bash
   # Windows
   python -m venv venv
   venv\Scripts\activate

   # macOS / Linux
   python3 -m venv venv
   source venv/bin/activate
   ```

4. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

5. **Download the dataset** (if required — see task-specific `KAGGLE_SETUP.md` or `DATASET_SETUP.md`)

6. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

7. **Open the `.ipynb` file** and run all cells (`Cell → Run All`)

---

## Task Overview

### Task 1: Iris Flower Classification 

| Detail | Description |
|--------|-------------|
| **Objective** | Classify iris flowers into Setosa, Versicolor, or Virginica |
| **Type** | Multi-class Classification |
| **Dataset** | Built into scikit-learn (`load_iris`) — no download needed |
| **Models** | Logistic Regression, KNN, Decision Tree, Random Forest |
| **Key Output** | Best model identified with accuracy, confusion matrix, classification report |

**Features:**
- Full EDA with pairplot and box plots
- Feature selection discussion (which features are most discriminative)
- 4 classifiers trained and compared
- Complete evaluation metrics

---

### Task 2: Unemployment Analysis (India) 

| Detail | Description |
|--------|-------------|
| **Objective** | Analyze unemployment trends with focus on COVID-19 impact |
| **Type** | Exploratory Data Analysis + Time Series |
| **Dataset** | [Unemployment in India - Kaggle](https://www.kaggle.com/datasets/gokulrajkmv/unemployment-in-india) |
| **Key Output** | Pre-COVID vs Post-COVID comparison, regional trends |

**Features:**
- Region-wise and month-wise unemployment analysis
- Time-series line charts for major states
- Top 10 states with highest unemployment (bar chart)
- Correlation heatmap
- Pre/Post-COVID split and impact analysis

---

### Task 3: Car Price Prediction 

| Detail | Description |
|--------|-------------|
| **Objective** | Predict selling price of used cars based on features |
| **Type** | Regression |
| **Dataset** | [Vehicle dataset from cardekho - Kaggle](https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho) |
| **Models** | Linear Regression, Random Forest, Gradient Boosting |
| **Key Output** | Best model with MAE, RMSE, R² + feature importance |

**Features:**
- Data cleaning: nulls, duplicates, inconsistent categorical values
- Feature engineering: car_age from year, brand from car name
- EDA: price distribution, fuel type, transmission analysis
- One-hot encoding
- Feature importance chart for best model

---

### Task 4: Email Spam Detection 

| Detail | Description |
|--------|-------------|
| **Objective** | Classify emails as spam or ham (legitimate) |
| **Type** | Binary NLP Classification |
| **Dataset** | [SMS Spam Collection - Kaggle/UCI](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset) |
| **Models** | Multinomial Naive Bayes, Logistic Regression, SVM |
| **Key Output** | Best spam classifier with precision, recall, F1 |

**Features:**
- Complete NLP preprocessing pipeline (lowercase, punctuation removal, stopwords, stemming)
- TF-IDF vectorization with unigrams + bigrams
- Discussion on why recall is critical for spam detection
- WordCloud visualizations for spam vs ham words
- Live prediction on custom messages

---

### Task 5: Sales Prediction 

| Detail | Description |
|--------|-------------|
| **Objective** | Predict product sales from TV, Radio, and Newspaper advertising spend |
| **Type** | Regression |
| **Dataset** | Advertising.csv (auto-downloads from GitHub) |
| **Models** | Linear Regression, Random Forest, Polynomial Regression (degree 2) |
| **Key Output** | Best model + interpretation of which channel drives sales most |

**Features:**
- Individual scatter plots with trend lines and correlation coefficients
- Correlation matrix heatmap
- Polynomial regression with interaction terms
- Residual analysis (randomness check)
- Channel impact interpretation using 3 methods
- Business recommendations

---

## Tech Stack

| Technology | Purpose |
|------------|---------|
| **Python** | Core programming language |
| **pandas** | Data manipulation and analysis |
| **numpy** | Numerical computing |
| **scikit-learn** | Machine learning models and metrics |
| **matplotlib** | Data visualization |
| **seaborn** | Statistical visualizations |
| **NLTK** | Natural language processing (Task 4) |
| **WordCloud** | Text visualization (Task 4) |
| **Jupyter Notebook** | Interactive development environment |

---

## Common Dependencies

All tasks require:
```
numpy, pandas, scikit-learn, matplotlib, seaborn, jupyter
```

Task-specific additional dependencies:
- **Task 4**: `nltk`, `wordcloud`
- **Task 2, 3**: `kaggle` (optional, for API download)

Install all for a specific task:
```bash
cd Task_1    # or any task folder
pip install -r requirements.txt
```

---

## Notes

- **Task 1** uses a built-in dataset — no external download required.
- **Tasks 2, 3, 4** require downloading datasets from Kaggle (free account) or UCI Repository.
- **Task 5** auto-downloads the dataset from a public GitHub repository if not found locally.
- Each task folder contains its own `SETUP.md` with detailed instructions.
- All notebooks are fully commented and ready to run cell-by-cell.


---

## Info

**Program**: OIBSIP Data Science 
**Tasks Completed**: 5/5  

---
