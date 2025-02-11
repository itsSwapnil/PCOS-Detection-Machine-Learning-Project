# PCOS Detection Machine Learning Project

## Project Overview
This project aims to build a machine learning model to predict the likelihood of Polycystic Ovary Syndrome (PCOS) using various health indicators. The dataset is in CSV format, and the solution involves data preprocessing, feature scaling, and training several machine learning models.

---

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Optimizations](#optimizations)
- [Contributing](#contributing)
- [License](#license)

---

## Dataset
The dataset is provided in CSV format. It contains multiple features related to health indicators that may influence PCOS diagnosis.

**Target Variable:**
- `PCOS Diagnosis` (binary classification: 1 indicates PCOS, 0 indicates no PCOS)

**Sample Features:**
- Age
- BMI
- Insulin levels
- Hormonal indicators
- Menstrual cycle information
- PCOS status

---

## Features
- Data loading and exploratory analysis
- Data preprocessing (handling categorical and missing data)
- Feature scaling using `StandardScaler`
- Model training and hyperparameter tuning using `GridSearchCV`
- Performance evaluation metrics (accuracy, precision, recall, F1-score)

---

## Technologies Used
- **Programming Language:** Python
- **Libraries:**
  - Pandas
  - Scikit-Learn
  - NumPy
  - Matplotlib (for visualizations)

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/pcos-detection.git
   cd pcos-detection
   ```

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Place your dataset CSV file in the project directory.

---

## Usage
1. Open the notebook `FINAL_PCOS.ipynb`.
2. Run the cells sequentially to preprocess the data, train the model, and evaluate its performance.
3. Modify hyperparameters or model types if needed.

---

## Results
Initial results indicate that the model achieved the following performance metrics:
- Accuracy: 91%  
- F1-Score: 91%  

Further optimization is suggested to improve model performance.

---

## Optimizations
1. **Data Preprocessing:**
   - Consider target encoding for high-cardinality categorical variables.
2. **Hyperparameter Tuning:**
   - Use `RandomizedSearchCV` for faster tuning when dealing with larger parameter spaces.
3. **Pipeline Creation:**
   - Integrate the preprocessing and model training steps into a Scikit-Learn pipeline for cleaner and more maintainable code.
4. **Cross-Validation:**
   - Increase the number of cross-validation folds to improve performance generalization.

---

## Contributing
Contributions are welcome. Please create a pull request or open an issue for discussion.

---

## License
This project is licensed under the [MIT License](LICENSE).
