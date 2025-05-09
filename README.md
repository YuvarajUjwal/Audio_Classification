COMPARATIVE ANALYSIS OF ML MODELS FOR AUDIO CLASSIFICATION

This repository presents a comparative study of various machine learning models applied to the **ESC-50 dataset**, a benchmark for environmental sound classification. The goal is to evaluate the performance of different models on the same dataset to identify a better performing model.

---

- Dataset Source: https://github.com/karolpiczak/ESC-50
- Number of Audio Files: 2000
- Classes: 50

---

Project Structure

- `Visualization/`: Folder for saved plots.
- `Comparative_Analysis_ESC50.ipynb`: The core analysis notebook.
- `README.md`: You're reading it!
- `requirements.txt`: List of libraries used.

---

Features Extracted

- **MFCCs (Mel Frequency Cepstral Coefficients)**: 13 coefficients were used as features.
- The boxplot analysis reveals wide variability in `mfcc_1`, while others are more stable.

---

Models Evaluated

- Baseline Model was selected as Dummy Classifier.
- Compared Models are Logistic Regression, KNN, SVM, Random Forest and ANN.

---

Hyperparameter Tuning

- All models (except baseline) were tuned using **Optuna**, due its efficient optimization and intelligent sampling.
- As long as there's an `objective` function, the **Optuna** can be applied to any model. 


---

Comparitive Model Performance Evaluation

| Model                             | Accuracy | Precision | Recall | F1 Score |
|-----------------------------------|----------|-----------|--------|----------|
| **Baseline (Dummy Classifier)**   | 0.02     | 0.02      | 0.02   | 0.02     |
| Logistic Regression               | 0.33     | 0.39      | 0.39   | 0.33     |
| K-Nearest Neighbors (KNN)         | 0.44     | 0.50      | 0.50   | 0.44     |
| Random Forest                     | 0.45     | 0.52      | 0.52   | 0.44     |
| Support Vector Machine (SVM)      | 0.46     | 0.50      | 0.50   | 0.45     |
| Artificial Neural Network (ANN)   | 0.46     | 0.49      | 0.49   | 0.45     |

---

Note:

- The above metrics were obtained on a single run of the models.
- Re-running the notebook may yield different metric values.

---

Setup Instructions

```bash
git clone  https://github.com/YuvarajUjwal/Audio_Classification.git
cd Audio_Classification
pip install -r requirements.txt
