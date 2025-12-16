🩺**Chronic Kidney Disease (CKD) Prediction – Machine Learning Project**

🧠 **Introduction**

⦁ Chronic Kidney Disease (CKD) is a progressive condition where the kidneys gradually lose their ability to filter waste from the blood. Early detection is extremely important because CKD can be treated and managed to prevent complete kidney failure.

⦁ Traditional diagnosis requires clinical expertise and several lab tests. With machine learning, we can build a model that learns patterns from patient health parameters and predicts whether an individual is at risk for CKD.

⦁ This project uses clinical dataset features such as age, blood pressure, haemoglobin, serum creatinine, sugar levels, red blood cell count, and other medical indicators to classify whether a patient has CKD or Not CKD.

⦁ The final output is a Streamlit web application where users can input patient details and instantly get a prediction.

📘 **Problem Statement**

Chronic Kidney Disease (CKD) is often detected at later stages because symptoms are mild in the beginning.
Early prediction using machine learning can help prevent complications.

The problem statement is:

“Build a machine learning model that predicts whether a patient has Chronic Kidney Disease (CKD) or not based on diagnostic features.”

📂 **Dataset Description**

The dataset contains 26 features related to clinical observations such as:

🔢 Numerical Features:

1.	age
2.	blood_pressure
3.	specific_gravity
4.	albumin
5.	sugar
6.	blood_glucose_random
7.	blood_urea
8.	serum_creatinine
9.	sodium
10.	potassium
11.	haemoglobin
12.	packed_cell_volume
13.	white_blood_cell_count
14.	red_blood_cell_count

🔠 Categorical Features:

1.	red_blood_cells (normal/abnormal)
2.	pus_cell (normal/abnormal)
3.	pus_cell_clumps
4.	bacteria
5.	hypertension
6.	diabetes_mellitus
7.	coronary_artery_disease
8.	appetite
9.	peda_edema
10.	aanemia

🎯 Target Variable:

classification (ckd / notckd)

🛠 Technologies Used

1.	Python
2.	Pandas / NumPy
3.	Scikit-Learn
4.	Matplotlib / Seaborn
5.	XGBoost
6.	Streamlit
7.	Pickle

🔧 **Project Workflow**:

1️⃣ Data Loading & Cleaning

⦁	Handled missing values
⦁	Converted object columns to numeric
⦁	Encoded categorical values
⦁	Removed invalid/outlier values

2️⃣ Exploratory Data Analysis (EDA)

⦁	Distribution of numerical features
⦁	Value counts of categorical features
⦁	Correlation heatmap
⦁	Boxplots & KDE plots

3️⃣ Data Preprocessing

1.	Label encoding
2.	Feature scaling
3.	Train–Test Split (80/20)

4️⃣ Model Building

Models trained:

⦁	Model	Accuracy

⦁	Random Forest Classifier	98.75%

⦁	AdaBoost Classifier	98.75%

⦁	XGBoost	96.25%

⦁	KNN	95%

⦁	Decision Tree / SVM / GBC	Lower accuracy

⦁	🏆 Best Model: Random Forest (98.75%)

🔍 Hyperparameter Tuning


⦁	GridSearchCV was used to tune:

⦁	n_estimators

⦁	max_depth

⦁	min_samples_split

⦁	criterion

⦁	Final optimized model was saved as:

⦁	good_model.pkl

🌐 Streamlit Application

A user-friendly interface was built using Streamlit where doctors can enter patient details and get CKD predictions.

Run Streamlit App:
streamlit run app.py

App Features:


✔ Input fields for all 24 features

✔ Automatic categorical encoding

✔ Displays prediction as CKD or Not CKD

✔ Uses the trained pickle model

📁 Project Folder Structure

📦 chronic-kidney-disease-prediction

│

├── 📄 chronic-kidney-disease.ipynb       # Model training & EDA

├── 📄 app.py                              # Streamlit app code

├── 📄 good_model.pkl                       # Saved trained model

├── 📄 requirements.txt                     # All dependencies

├── 📄 README.md                            # Project documentation

└── 📁 data/
      └── kidney_disease.csv               # Dataset

📥 Installation & Setup

1.	 Clone the repository:

git clone https://github.com/yourusername/ckd-prediction.git
cd ckd-prediction

2.	Install dependencies:

pip install -r requirements.txt

3.	Run the Streamlit app:

   streamlit run app.py

📊 Results


⦁Best accuracy achieved: 98.75%

⦁	Model generalizes well on test data

⦁	Streamlit app provides real-time prediction

🚀 Conclusion

This project demonstrates that Machine Learning can reliably predict Chronic Kidney Disease (CKD) using clinical parameters.
The deployed Streamlit app is fast, easy to use, and doctor-friendly.

Future improvements:

⦁	Deploy on AWS / Render

⦁	Add SHAP explainability

⦁	Expand dataset for robustness

🤝 Contributing

Pull requests are welcome.
For major changes, please open an issue first to discuss.
