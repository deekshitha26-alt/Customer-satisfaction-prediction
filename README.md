# ✨ End-to-End Predictive Analytics Pipeline for Customer Satisfaction Using Python & Neural Networks

An interactive **Machine Learning and Predictive Analytics application** that predicts customer satisfaction scores using a trained **Neural Network model**. The application is built with **Python, TensorFlow/Keras, Pandas, Scikit-learn, and Streamlit** and provides both batch and real-time prediction capabilities.

---

## 📌 Project Overview

Customer satisfaction is an important business metric that helps organizations understand customer behavior and improve their products and services.

This project develops an end-to-end predictive analytics pipeline that:

* Processes customer information
* Performs categorical feature encoding
* Applies feature scaling
* Uses a trained Neural Network model to predict satisfaction
* Provides batch predictions from CSV files
* Provides real-time predictions through an interactive form
* Displays visual insights and prediction results
* Allows users to download batch prediction results

The complete solution is presented through an easy-to-use **Streamlit web application**.

---

## 🎯 Objectives

The main objectives of this project are:

1. Predict customer satisfaction based on customer-related attributes.
2. Build an end-to-end machine learning prediction pipeline.
3. Provide both batch and real-time prediction functionality.
4. Create an interactive dashboard for business users.
5. Generate visual insights from predicted satisfaction scores.
6. Demonstrate the practical use of Neural Networks in predictive analytics.

---

## 🚀 Key Features

### 📄 1. Batch Prediction

Users can upload a customer dataset in CSV format.

The application:

* Reads the uploaded CSV file
* Removes the `id` column when available
* Performs categorical encoding
* Aligns features with the trained model
* Applies the saved scaler
* Generates satisfaction predictions
* Displays prediction results
* Provides downloadable prediction results

### 🎯 2. Real-Time Prediction

Users can enter individual customer details through an interactive form.

The application accepts:

* Age
* Gender
* Income
* Education
* Region
* Loyalty Status
* Purchase Frequency
* Purchase Amount
* Product Category
* Promotion Usage

The trained Neural Network then generates a predicted customer satisfaction score.

### 📊 3. Interactive Visualizations

The application provides visual insights including:

* Satisfaction score distribution
* Top 10 customers based on predicted satisfaction
* Real-time satisfaction score visualization

### 📥 4. Download Predictions

Batch prediction results can be downloaded as a CSV file directly from the application.

---

## 🧠 Machine Learning Pipeline

The project follows an end-to-end predictive analytics workflow:

```text
Customer Dataset
       ↓
Data Preprocessing
       ↓
Categorical Feature Encoding
       ↓
Feature Alignment
       ↓
Feature Scaling
       ↓
Trained Neural Network
       ↓
Customer Satisfaction Prediction
       ↓
Visualization & Results
```

---

## 🛠️ Technologies Used

| Technology       | Purpose                                  |
| ---------------- | ---------------------------------------- |
| Python           | Core programming language                |
| TensorFlow       | Neural Network / Deep Learning framework |
| Keras            | Model loading and prediction             |
| Pandas           | Data processing and manipulation         |
| NumPy            | Numerical operations                     |
| Scikit-learn     | Feature scaling and preprocessing        |
| Streamlit        | Interactive web application              |
| Matplotlib       | Data visualization                       |
| Seaborn          | Statistical visualization                |
| Jupyter Notebook | Model development and experimentation    |

---

## 📁 Project Structure

```text
Customer-Satisfaction-Prediction/
│
├── app.py
├── code.ipynb
│
├── model.h5
├── model.keras
├── scaler.pkl
├── model_columns.pkl
│
├── customer_data.csv
├── Test_data.csv
│
├── requirements.txt
├── README.md
└── project documentation.pdf
```

### File Description

| File                        | Description                                          |
| --------------------------- | ---------------------------------------------------- |
| `app.py`                    | Streamlit application                                |
| `code.ipynb`                | Model development and analysis notebook              |
| `model.h5`                  | Trained Neural Network model used by the application |
| `model.keras`               | Keras model file                                     |
| `scaler.pkl`                | Saved feature scaler                                 |
| `model_columns.pkl`         | Saved feature-column configuration                   |
| `customer_data.csv`         | Customer dataset                                     |
| `Test_data.csv`             | Test dataset                                         |
| `requirements.txt`          | Required Python packages                             |
| `project documentation.pdf` | Detailed project documentation                       |

> **Note:** The current Streamlit application loads `model.h5`. Therefore, `model.keras` is not required for running the current `app.py`, but it can be retained as an alternative model artifact.

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/customer-satisfaction-prediction.git
```

Replace `YOUR-USERNAME` with your GitHub username.

### 2. Open the Project Folder

```bash
cd customer-satisfaction-prediction
```

### 3. Create a Virtual Environment

```bash
python -m venv env
```

### 4. Activate the Virtual Environment

#### Windows

```bash
env\Scripts\activate
```

#### macOS / Linux

```bash
source env/bin/activate
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

### 6. Run the Streamlit Application

```bash
streamlit run app.py
```

The application will open in your browser.

---

## 🖥️ How to Use the Application

### Batch Prediction

1. Launch the Streamlit application.
2. Select **Batch Prediction** from the sidebar.
3. Upload a customer CSV file.
4. The application preprocesses the uploaded data.
5. The Neural Network generates satisfaction predictions.
6. View the prediction results and visualizations.
7. Download the generated `predictions.csv` file.

### Real-Time Prediction

1. Select **Real-Time Prediction**.
2. Enter the customer's information.
3. Click **Predict Satisfaction**.
4. The application displays the predicted satisfaction score.
5. Review the score using the visual indicator.

---

## 📊 Input Features

The real-time prediction interface uses the following customer attributes:

```text
age
gender
income
education
region
loyalty_status
purchase_frequency
purchase_amount
product_category
promotion_usage
```

These features are encoded and transformed to match the feature structure expected by the trained model.

---

## 🧪 Model Prediction

The application loads the trained Neural Network model from:

```text
model.h5
```

The saved preprocessing components are loaded from:

```text
scaler.pkl
model_columns.pkl
```

This ensures that prediction data follows the same preprocessing structure used during model development.

---

## 📈 Business Applications

This predictive analytics solution can support organizations in:

* Identifying customer satisfaction patterns
* Understanding customer behavior
* Prioritizing high-value customers
* Supporting customer retention strategies
* Improving customer experience
* Making data-driven business decisions
* Analyzing satisfaction trends at scale

---

## 🔮 Future Enhancements

Possible improvements include:

* Model performance comparison with other algorithms
* Hyperparameter tuning
* Additional customer behavioral features
* Model evaluation metrics dashboard
* Prediction confidence visualization
* Database integration
* User authentication
* Cloud deployment
* Automated model retraining
* REST API integration
* Advanced business intelligence dashboards

---

## 📦 Requirements

The project uses the following major dependencies:

```text
streamlit==1.35.0
pandas==2.2.2
numpy==1.24.4
scikit-learn==1.4.2
tensorflow==2.15.0
matplotlib==3.8.4
seaborn==0.13.2
pickle-mixin==1.0.2
```

Install all dependencies using:

```bash
pip install -r requirements.txt
```

---

## ⚠️ Notes

* The application currently loads `model.h5`.
* Input CSV files should contain features compatible with the trained model.
* The preprocessing configuration stored in `model_columns.pkl` should be kept together with the model.
* The scaler stored in `scaler.pkl` is required for prediction.
* Large datasets may require additional memory during processing.

---

## 👩‍💻 Author

**Deekshitha Avala**

B.Tech – Computer Science and Engineering

### Technical Skills

* Python
* Machine Learning
* Neural Networks
* TensorFlow/Keras
* Predictive Analytics
* Data Analysis
* Streamlit
* Pandas
* Scikit-learn
* Data Visualization

---

## ⭐ Project Highlights

> **End-to-End Predictive Analytics + Neural Network + Interactive Streamlit Dashboard**

This project demonstrates the complete journey from **customer data preprocessing to machine learning prediction and interactive visualization** in a practical business-oriented application.

---

## 📄 Documentation

For detailed information about the project methodology, implementation, and results, refer to:

```text
project documentation.pdf
```

---

## 📜 License

This project is intended for educational, academic, and portfolio purposes.
