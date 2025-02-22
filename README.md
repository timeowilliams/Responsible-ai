# CORD-19 Dataset Analysis

Analysis and modeling of the CORD-19 dataset for Responsible AI assignments.

## Project Structure
- `test.ipynb`: Bias analysis of COVID-19 research publications
- `model.ipynb`: Predictive model for paper accessibility
- `json_schema.txt`: Schema for dataset JSON files
- `metadata.readme`: Dataset metadata info
- `requirements.txt`: Python dependencies

## Getting Started
1. Clone this repository: `git clone https://github.com/timeowilliams/Responsible-ai`
2. Install dependencies: `pip install -r requirements.txt`
3. Set up Kaggle API:
   - Get your API token from [Kaggle Account](https://www.kaggle.com/account) (`kaggle.json`).
   - In `model.ipynb`, replace `your_kaggle_username` and `your_kaggle_key` in Section 1 with your credentials.
   - Or configure via terminal: `kaggle config set -n username -v YOUR_USERNAME` and `kaggle config set -n key -v YOUR_KEY`.
4. Run notebooks in Jupyter:
   - `test.ipynb`: Bias analysis
   - `model.ipynb`: Downloads `metadata.csv` (1.65 GB) from [Kaggle](https://www.kaggle.com/datasets/allen-institute-for-ai/CORD-19-research-challenge?select=metadata.csv) and builds model

## Assignments
- **Assignment 2 (test.ipynb)**: Analyzes bias in journal distribution, accessibility, topics, language, and geography.
- **Assignment 3 (model.ipynb)**: Builds a Logistic Regression model to predict PDF availability, with performance analysis and proxy detection.

## Dependencies
See `requirements.txt`. Key libraries: `pandas`, `scikit-learn`, `matplotlib`, `seaborn`, `langdetect`, `statsmodels`, `kaggle`.