# PYTHON---MEDICAL-INSURANCE-COST-ESTIMATION
This is a Python project that estimates medical insurance costs using a formula-based approach and explores how age, BMI, sex, and smoking status affect the final estimate.
# Medical Insurance Cost Estimator

This project explores how a simple pricing formula can be used to estimate yearly medical insurance costs based on a few personal factors such as age, sex, BMI, number of children, and smoking status.

It started as a Python syntax practice project and was standardised into a clean, GitHub-ready format with a notebook, Python script, dataset folder, and supporting project files.

## Project Objective

The goal of this project is to:
- practice Python syntax and variable manipulation
- apply arithmetic expressions and string formatting
- understand how changes in personal attributes can affect estimated insurance costs
- organise a beginner Python project in a professional repository structure

## Dataset

The repository includes the `insurance.csv` dataset, which contains:
- `age`
- `sex`
- `bmi`
- `children`
- `smoker`
- `region`
- `charges`

Although the main exercise uses a fixed insurance cost formula, the dataset is included for further exploration and future analysis.

## Formula Used

The insurance estimate is calculated as:

```python
insurance_cost = (
    250 * age
    - 128 * sex
    + 370 * bmi
    + 425 * num_of_children
    + 24000 * smoker
    - 12500
)
```

Where:
- `sex`: `0` for female, `1` for male
- `smoker`: `0` for non-smoker, `1` for smoker

## Project Files

```text
medical-insurance-cost-estimator/
├── data/
│   └── insurance.csv
├── medical_insurance_cost_estimator.ipynb
├── medical_insurance_cost_estimator.py
├── requirements.txt
├── .gitignore
└── README.md
```

## What the Project Covers

The project walks through:
1. setting up patient profile variables
2. calculating a base insurance estimate
3. testing how age changes affect the estimate
4. testing how BMI changes affect the estimate
5. comparing cost differences by sex
6. summarising the results in a clean, readable format

## Key Skills Demonstrated

- Python variables
- arithmetic operations
- function creation
- scenario analysis
- string formatting
- code organisation
- GitHub project presentation

## How to Run

### Option 1: Run the notebook
Open `medical_insurance_cost_estimator.ipynb` in Jupyter Notebook, VS Code, or Google Colab.

### Option 2: Run the Python script
From the project folder, run:

```bash
python medical_insurance_cost_estimator.py
```

## Sample Output

```text
Base insurance cost: $5469.0
Change after increasing age by 4 years: $1000.0
Change after increasing BMI by 3.1: $1147.0
Change for being male instead of female: $-128.0
```

## Why This Project Matters

This project shows the ability to take a beginner-level Python exercise and present it in a cleaner, more professional way for a portfolio. It demonstrates not only Python fundamentals, but also the ability to structure work clearly for GitHub and future employers.

## Next Improvements

Possible future enhancements:
- analyse the full dataset with pandas
- compare estimated costs with actual insurance charges
- visualise trends using matplotlib or seaborn
- build a small prediction or comparison tool

## Author

Prepared and standardised for portfolio and GitHub presentation.
