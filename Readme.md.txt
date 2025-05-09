Comparative Analysis of ML Models for Audio Classification using ESC-50 Dataset

This repository presents a comparative study of various machine learning models applied to the **ESC-50 dataset**, a benchmark for environmental sound classification. The goal is to evaluate the performance of different models on the same dataset to identify a better performing model.

---

Project Structure

- `Comparative_Analysis_ESC50.ipynb`: The core analysis notebook.
- `requirements.txt`: List of libraries used.
- `Visualization/`: Folder for saved plots (optional).
- `README.md`: You're reading it!

---

Models Evaluated

- Baseline Model was selected as "Dummy Classifier"


**Note:** Metrics may vary slightly due to Optuna-based hyperparameter tuning.

---

Features Extracted

- **MFCCs (Mel Frequency Cepstral Coefficients)**: 13 coefficients were used as features.
- The boxplot analysis reveals wide variability in `mfcc_1`, while others are more stable.

---

Hyperparameter Tuning

- All models (except baseline) were tuned using **Optuna**, allowing dynamic search space optimization.
- Re-running the notebook may yield different metric values.

---

Setup Instructions (Windows)

```bash
git clone https://github.com/yourusername/esc50-ml-comparison.git
cd esc50-ml-comparison
pip install -r requirements.txt
