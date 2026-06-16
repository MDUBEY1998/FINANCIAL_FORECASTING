

# 🚀 Efficient Banking Analytics & Predictive Modeling with PySpark

This project demonstrates large-scale **data processing, exploratory data analysis, machine learning, and real-time analytics** using Apache Spark (PySpark). It covers batch processing, parallel computation, and streaming-style analytics on the **Bank Marketing Dataset (`bank.csv`)**.

---

## 📌 Project Overview

The workflow is divided into four major tasks:

* **Task 1:** Data Parallelism & Machine Learning Pipeline
* **Task 2:** Exploratory Data Analysis (EDA)
* **Task 3:** Predictive Modeling & Hyperparameter Tuning
* **Task 4:** Real-Time Stream Analytics Simulation

---

# ⚙️ Task 1: Data Parallelism & ML Pipeline

### 🔹 Key Steps

* Built Spark session with optimized memory & shuffle partitions
* Loaded and processed `bank.csv` using Spark DataFrame API
* Applied **data partitioning using `repartition()` on balance**
* Performed distributed aggregations:

  * Average balance per job category
  * Top age groups by financial activity

### 🔹 Machine Learning Model

* Model used: **Random Forest Classifier**
* Feature Engineering:

  * StringIndexing for categorical variables
  * VectorAssembler for feature vector creation
* Pipeline-based training approach

### 🔹 Output

* Model evaluated using **AUC (Area Under ROC Curve)**
* Model saved for reuse

---

# 📊 Task 2: Exploratory Data Analysis (EDA)

### 🔹 Data Exploration

* Schema inspection, summary statistics, and filtering
* GroupBy analysis on job, marital status, education

### 🔹 Feature Engineering

* Created:

  * Age groups using UDF
  * Subscription rate per education level
  * Loan default rate per job

### 🔹 Insights Generated

* Highest subscription rates by education
* Financial behavior differences across job types
* Correlation between age and balance

### 🔹 Visualization

* Job distribution bar chart using Matplotlib
* Contact method success rate analysis

---

# 🤖 Task 3: Predictive Modeling & Optimization

### 🔹 ML Pipeline

* Data preprocessing:

  * Missing value handling
  * Outlier filtering
  * Categorical encoding

### 🔹 Model Training

* Algorithms used:

  * Logistic Regression
  * Gradient Boosting / Tree-based models
* Feature engineering using VectorAssembler

### 🔹 Hyperparameter Tuning

* Used:

  * CrossValidator
  * ParamGridBuilder
* Evaluated using:

  * Accuracy
  * BinaryClassificationEvaluator

### 🔹 Model Insights

* Extracted feature importance / coefficients
* Identified most influential predictors of term deposit subscription

---

# ⚡ Task 4: Real-Time Stream Analytics (Simulated)

### 🔹 Streaming Simulation

* Converted batch dataset into streaming-like chunks
* Aggregated real-time metrics:

  * Average balance by job
  * Average transaction duration

### 🔹 Window Analytics

* Implemented rolling window computations:

  * Transaction count
  * Average balance trends

### 🔹 Watermarking

* Handled late and out-of-order data using watermarking
* Ensured accurate time-based aggregation

---

# 📈 Key Technologies Used

* Python
* PySpark
* Spark SQL
* Spark MLlib
* Matplotlib / Pandas
* Google Colab + Google Drive

---

# 🧠 Key Learnings

* Distributed data processing using Spark RDD/DataFrame APIs
* Parallel computation using partitioning strategies
* End-to-end ML pipeline development in Spark
* Real-time analytics using structured streaming concepts
* Model tuning and evaluation at scale

---

# 📌 Conclusion

This project demonstrates how large-scale financial datasets can be efficiently processed and analyzed using distributed computing. It combines **data engineering, machine learning, and streaming analytics** into a unified Spark-based pipeline.


