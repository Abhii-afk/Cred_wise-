
# CredWise — Loan Approval Prediction

CredWise is a lightweight machine learning project that preprocesses loan application data and trains classification models to predict loan approval. The notebook demonstrates data cleaning, feature engineering, model training, and evaluation.

**Dataset**: `loan_approval_data.csv`

**Highlights**
- Data imputation for missing values (numerical and categorical)
- One-hot encoding and label encoding for categorical features
- Feature engineering (polynomial features)
- Standard scaling and model comparison: Logistic Regression, KNN, Naive Bayes

**Project Structure**
- `credit_wise (1).ipynb` — Jupyter notebook with full EDA, preprocessing, modeling, and evaluation
- `loan_approval_data.csv` — Source dataset

Getting Started
---------------

Requirements
1. Python 3.8+
2. Packages: `pandas`, `numpy`, `scikit-learn`, `seaborn`, `matplotlib`

Quick setup
1. Create a virtual environment (optional but recommended):

```bash
python -m venv .venv
```

2. Activate the environment and install dependencies:

On Windows (PowerShell):

```powershell
.\.venv\Scripts\Activate.ps1
pip install pandas numpy scikit-learn seaborn matplotlib
```

Usage
-----
1. Open `credit_wise (1).ipynb` in Jupyter Notebook or VS Code.
2. Run the cells sequentially to reproduce preprocessing, model training, and evaluation.

Model & Evaluation Notes
------------------------
- The notebook trains several baseline models and prints precision, recall, F1 score, accuracy, and confusion matrices.
- Naive Bayes was highlighted as the best model by precision in the notebook experiments; feel free to run cross-validation or hyperparameter tuning for more robust selection.

Push to GitHub
--------------
If you want to push this project to a new GitHub repository, run the following commands in the project root:

```bash
git init
git add .
git commit -m "Initial commit: CredWise loan approval predictor"
gh repo create CredWise --public --source=. --remote=origin
git push -u origin main
```

Notes:
- The `gh` command uses the GitHub CLI. If you don't have it, create a repo on GitHub and follow the instructions there, or replace the `gh repo create` step with the `git remote add origin <URL>` command.

Contributing
------------
- Suggestions, issues, and PRs are welcome. For quick improvements, add new notebooks, experiments, or a `requirements.txt` file.

License
-------
This project is provided as-is; add a license file if you plan to publish the repository publicly.

Contact
-------
For questions, attach an issue in the GitHub repo once created.
