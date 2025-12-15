# 🏃‍♂️ FitPulse – Health Data Analysis & Anomaly Detection

FitPulse is a **Streamlit-based data analysis and anomaly detection application** designed to analyze fitness and running-related health data.  
The application performs **data cleaning, correlation analysis, regression, clustering, and anomaly detection** using machine learning techniques, and presents results through interactive visualizations.

---

## 🚀 Features

### ✅ Data Loading & Cleaning
- Handles missing values  
- Converts numerical columns to appropriate types  

### 📊 Correlation Matrix
- Visual heatmap of correlations between health metrics  

### 🔍 Correlation Visualization
- Absolute correlation plots  
- Identification of highly correlated variable pairs  

### 📈 Linear Regression
- Distance vs Time Elapsed prediction  
- Interactive Plotly visualization  

### 🔗 Scatter Matrix
- Pairwise relationships between all numerical features  

### 🧩 Clustering
- K-Means clustering on selected health metrics  
- Scaled data visualization  

### 🚨 Anomaly Detection
- Mahalanobis distance–based anomaly detection  
- Interactive user input for real-time anomaly checking  

---

## 🛠️ Tech Stack

- **Programming Language:** Python 3.11+  
- **Framework:** Streamlit  
- **Libraries:**  
  - pandas  
  - numpy  
  - matplotlib  
  - seaborn  
  - plotly  
  - scikit-learn  
  - scipy  

---

## 📂 Project Structure

```
FitPulse-Health-Anomaly-Detection/
│
├── requirements.txt
├── README.md
├── src/
│   └── streamlit/
│       ├── app.py
│       ├── data_loading_and_cleaning.py
│       ├── correlation_matrix.py
│       ├── visualize_correlation.py
│       ├── plotting_all_relationships.py
│       ├── plotly_linear_regression.py
│       ├── clustering.py
│       ├── anomaly_detection.py
│       └── data/
│           └── data.csv
└── .devcontainer/
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/Adithyaharshithreddy24/FitPulse-Health-Anomaly-Detection.git
cd FitPulse-Health-Anomaly-Detection
````

### 2️⃣ Create & Activate Virtual Environment

```bash
python -m venv venv
source venv/bin/activate   # macOS / Linux
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ How to Run the Application

⚠️ **Important:** Run Streamlit from the `src/streamlit` directory.

```bash
cd src/streamlit
streamlit run app.py
```

Open your browser and go to:

```
http://localhost:8501
```

---

## 📊 Dataset

* The dataset (`data.csv`) must be placed inside:

```
src/streamlit/data/data.csv
```

* The application automatically cleans and processes the dataset at startup.

---

## 🧠 Anomaly Detection Logic

* Uses **Mahalanobis Distance**
* Flags a data point as an anomaly if:

```
distance ≥ 3
```

### User Inputs

* Heart Rate
* Time Elapsed
* Running Cadence
* Calories Burned
* Distance

---

## 🌐 Deployment (Streamlit Cloud)

* Push the project to GitHub
* Visit [https://streamlit.io/cloud](https://streamlit.io/cloud)
* Select this repository
* Set the **main file path** as:

```
src/streamlit/app.py
```


