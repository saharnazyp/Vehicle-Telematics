## 🚗 Vehicle Telematics Analysis with Machine Learning

### 📌 Overview

This project focuses on analyzing vehicle telematics data to uncover driving behaviors, detect anomalies, and train predictive models aimed at enhancing efficiency, safety, and diagnostics across fleets.

With the rise of IoT and connected cars, vast volumes of telematics data are now available. This repository demonstrates how machine learning and deep learning methods can harness this data for meaningful insights.

---

### 🗂️ Project Structure

```
TelemaicVehicle/
├── 📊 Data Loading
├── 🧼 Data Preprocessing
├── 📈 Exploratory Data Analysis (EDA)
├── 🧠 Feature Engineering
├── 🧱 Modeling Pipeline
├── ⚡ LazyPredict Model Comparison
├── 🤖 Model Training (ML/DL)
├── 📈 Model Evaluation
├── 🎛️ Gradio Interface
├── 🔍 Sample Predictions
└── 📄 README.md
```

---

### ⚙️ Technologies Used

* **Programming:** Python 🐍
* **Libraries:** Pandas, NumPy, Seaborn, Matplotlib
* **Modeling:** Scikit-learn, TensorFlow, Keras, LazyPredict
* **Interface:** Gradio
* **IDE:** Jupyter Notebook
* **Data Storage:** Google Drive (for large `.csv` datasets)

---

### 📥 Data Description

The dataset includes telematics features such as:

* GPS Speed
* Engine Temperature
* Battery Voltage
* Mass Air Flow (MAF), kpl, IAT, and other fuel metrics
* Diagnostic Trouble Codes (DTC)
* Trip-based time-series data (via `tripID`)

Data preprocessing includes cleaning, deduplication, and format standardization.

---

### 📊 Exploratory Data Analysis (EDA)

Performed using:

* Descriptive statistics
* Correlation heatmaps
* Distribution plots (speed, engine load, etc.)
* Outlier and duplicate detection

Custom features like `acceleration`, `angle_change`, and their squared values were also engineered to support non-linear modeling.

---

### 🧼 Data Preprocessing

* Categorical to numeric transformation
* Missing value imputation
* Outlier handling
* Feature scaling with `StandardScaler`
* Sequence reshaping for LSTM: `[samples, time_steps, features]`

---

### ⚡ LazyPredict Model Comparison

We use LazyPredict to quickly compare the performance of several baseline models with minimal code, helping identify strong candidates for further tuning.

---

### 🤖 Machine Learning Modeling

#### ✅ Classical ML Models:

* Random Forest Classifier
* Logistic Regression

#### ✅ Deep Learning:

* LSTM (ideal for time series modeling)
* Conv1D (captures short-term fluctuations)

---

### 📈 Evaluation Metrics

* Accuracy
* Precision / Recall / F1-Score
* Confusion Matrix
* Validation Curves

To manage class imbalance (e.g. `normal` vs `faulty`), we apply `class_weight='balanced'`.

---

### 🧪 Sample Predictions

New sequences can be passed through the entire pipeline (scaling, reshaping, predicting) using trained models.

---

### 🎛️ Gradio Web Interface

A simple web UI built using **Gradio** allows for interactive model testing by uploading CSV sequences and viewing predictions without writing code.

---

### 📚 Key Takeaways

* Sensor data requires domain-specific feature engineering.
* Sequence models like LSTM outperform static models for telematics.
* Automating evaluation with LazyPredict saves time in model selection.
* A clean pipeline with Gradio interface enhances usability and deployment readiness.

---

### 🚀 Future Enhancements

* Real-time dashboard integration via Streamlit or Tableau
* RESTful API with FastAPI or Flask
* Add behavioral clustering for new driver behavior profiles
* Export trained models for use in embedded devices or edge computing

---

### 🤝 Contributing

Have ideas or improvements? Fork the repo, create a branch, and submit a pull request. Contributions are welcome!

---

### 📬 Contact

For questions or collaboration:

* 📧 Email: [saharnazyaghoobpoor@gmail.com](mailto:saharnazyaghoobpoor@gmail.com)
* 🌐 [LinkedIn](https://www.linkedin.com/in/saharnaz-yaghoobpour-90068ab2/)
* 💻 [GitHub](https://github.com/saharnazyp)
* 📊 [Kaggle](https://www.kaggle.com/saharnazyaghoobpoor)

🎯 MY GOAL:Aiming to lead the evolution of Automotive AI Systems through innovation and data-driven solutions.
