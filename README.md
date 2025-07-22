# Smart-Salary-Predictor
🧠 CAPSTONE PROJECT: Smart Salary Predictor
✅ Presented By
Student Name: Thutukuri Jagadeesh
College Name: Presidency University
Department: MCA (Computer Science)
AICTE ID: STU674ac1ed70f0b173295255

1️⃣ Problem Statement
The Smart Salary Predictor aims to estimate the annual and monthly income of an employee based on key demographic and employment factors.
Using a dataset derived from IBM’s salary records, the goal is to create a machine learning model that helps users:

Predict future earning potential.

Analyze the impact of variables like education, experience, and occupation on income.

Empower HR and individuals with insights for career planning.

Support batch processing of multiple employee records for organizations.

Present clear visual insights with experience trends and recommendations.

2️⃣ System Development Approach
🔧 Technologies & Tools Used:
Language: Python

Libraries: Pandas, NumPy, Matplotlib, Scikit-learn, Streamlit

Platform: Google Colab, Streamlit Cloud

Deployment: Ngrok/Streamlit Sharing

🗃️ Libraries Required:
pandas, numpy

sklearn: RandomForestRegressor, Pipeline, StandardScaler, LabelEncoder, etc.

streamlit, io for front-end UI and file downloads

3️⃣ Algorithm & Deployment
🔄 Step-by-Step Process:
Data Preprocessing

Clean nulls and outliers

Remove irrelevant fields like education (due to redundancy with educational-num)

Replace '?' with 'Others' for workclass and occupation

Normalize values and label encode categorical fields

Feature Engineering

Added experience manually

Filtered valid ranges:

Age: 17–75

Education-num: 5–16

Hours/week: 1–99

Model Training

Used RandomForestRegressor with hyperparameters:

n_estimators=50, max_depth=6

Trained on 80/20 split of processed data

App Interface with Streamlit

Sidebar for inputs (Age, Education Level, Gender, etc.)

Real-time predictions

Experience vs Salary graph

CSV Export & Batch Upload

4️⃣ Result
📌 Model Output Examples (from screenshots):

Annual Salary: ₹409,660.70

Monthly Salary: ₹34,138.39

Batch Prediction: Predicted salaries shown for 10 uploaded records (screenshot verified)

📊 Graph: "Experience vs Predicted Salary" line chart indicates salary growth trend with years of experience.

📥 Batch Upload CSV: Uploaded file with columns age, educational-num, experience, hours-per-week was processed and augmented with prediction columns.


5️⃣ Conclusion
The Smart Salary Predictor efficiently forecasts individual and bulk employee salaries using streamlined input fields.

The model performs well using Random Forest Regressor with accurate salary ranges and trends.

Key challenges included:

Encoding categorical variables properly.

Ensuring Streamlit UI was intuitive and styled.

The solution empowers users with actionable career insights and company-wide forecasting.

6️⃣ Future Scope
Include real-time API integration with HRMS tools.

Add role-based salary benchmarking and market trends.

Enable model fine-tuning by uploading training data.

Integrate login and report generation for HR departments.

