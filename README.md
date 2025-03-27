# Perceptron Feature Scaling Tutorial

This project evaluates the impact of different feature scaling techniques on the performance of a Perceptron model for classifying genuine and forged banknotes.

Project Overview
Objective: Compare how Min-Max Scaling, Standardization, Robust Scaling, and No Scaling affect the Perceptron's accuracy.

Dataset:  The dataset used is the Banknote Authentication Dataset from UCI Machine Learning Repository. Contains 4 numerical features (wavelet-transformed variance, skewness, kurtosis, entropy) with binary labels (0 = forged, 1 = genuine).

Key Libraries: scikit-learn, pandas, numpy, matplotlib, seaborn.

Model: sklearn.linear_model.Perceptron.

Installation & Setup
Clone the repository:

bash
Copy
git clone https://github.com/your-username/banknote-perceptron.git
cd banknote-perceptron
Install dependencies (recommended: use a virtual environment):

bash
Copy
pip install -r requirements.txt
(Sample requirements.txt: numpy, pandas, scikit-learn, matplotlib, seaborn)

Run the Jupyter Notebook or Python script:

bash
Copy
jupyter notebook perceptron_scaling_comparison.ipynb
or

bash
Copy
python perceptron_scaling.py


Methodology
Data Preprocessing:

Load and split data (train/test).

Apply scaling methods:

Min-Max Scaling (features scaled to [0, 1])

Standardization (mean=0, variance=1)

Robust Scaling (resistant to outliers)

No Scaling (baseline).

Training & Evaluation:

Train a Perceptron model on each scaled dataset.

Compare accuracy, convergence speed, and decision boundaries.


Visualization:
Plot feature distributions before/after scaling.
Generate confusion matrices and accuracy bar charts.


File Structure
Copy
banknote-perceptron/
├── data/                   # Dataset (CSV format)
│   └── banknote_authentication.csv
├── notebooks/              # Jupyter Notebook for analysis
│   └── perceptron_scaling_comparison.ipynb
├── scripts/                # Python scripts (optional)
│   └── perceptron_scaling.py
├── results/                # Outputs (plots, metrics)
│   ├── accuracy_scores.png
│   └── feature_distributions.png
├── requirements.txt        # Dependencies
└── README.md

Results
Standardization typically performs best due to Gaussian-like feature distributions.

Min-Max Scaling improves accuracy when features have bounded ranges.

Robust Scaling is useful if outliers are present.

No Scaling often underperforms due to feature dominance.

(Include a screenshot of accuracy comparisons or plots if applicable.)

References
Rosenblatt, F. (1958). The Perceptron: A Probabilistic Model for Information Storage and Organization in the Brain. Psychological Review.

Lohweg, V. (2013). Banknote Authentication Dataset. UCI ML Repository.

Pedregosa et al. (2011). Scikit-learn: Machine Learning in Python. JMLR.

License
MIT License (or specify your preferred license).
