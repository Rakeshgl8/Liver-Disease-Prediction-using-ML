# Liver-Disease-Prediction-using-ML
Web application | Flask | Machine Learning 

# Liver Disease Prediction using Machine Learning

This is a project titled "Liver Disease Prediction Using Machine Learning," where I implemented three distinct machine learning algorithms: Random Forest, Support Vector Machine (SVM), and Logistic Regression.

The dataset was obtained from Kaggle and contains various features crucial for liver disease prediction, including 
- Age of the patient
- Gender of the patient
- Total Bilirubin
- Direct Bilirubin
- Alkphos Alkaline Phosphatase
- Sgpt Alamine Aminotransferase
- Sgot Aspartate Aminotransferase
- Total Proteins
- ALB Albumin
- A/G Ratio Albumin and Globulin Ratio
- Result

To ensure robust model performance, I employed several data preprocessing techniques. Initially, I separated the dataset into numeric and categorical data types. Duplicate records were removed, and missing numerical data was imputed using the mean value. Categorical data, such as 'Gender', was encoded using LabelEncoder, where '1' represented male and '0' represented female.

To handle outliers in numerical features, I utilized the Interquartile Range (IQR) method and subsequently removed outlier values. Normalization and scaling of numeric features were performed using StandardScaler to ensure uniformity in data ranges across different features.

For model evaluation and validation, I implemented Stratified K-Fold cross-validation to split the dataset into training and testing sets. 

The performance of each model was assessed using key metrics such as Accuracy, Precision, Recall, F1-score, and ROC-AUC. Additionally, I visualized the model's performance using a confusion matrix to analyze classification results comprehensively.

After evaluating the models, it was determined that the Random Forest algorithm outperformed SVM and Logistic Regression, achieving higher accuracy and demonstrating superior predictive capabilities for identifying liver disease risk in individuals.

To make the model accessible and user-friendly, I developed a web application using HTML, CSS, JavaScript, and the Python Flask web framework. MySQL was employed for efficient data management within the application. The Random Forest model was integrated into the application to allow users to input relevant patient data and obtain predictions regarding the likelihood of liver disease.

In conclusion, this project illustrates the application of machine learning techniques in healthcare, specifically for predicting liver disease based on patient demographics and clinical markers. It showcases effective data preprocessing, model selection, evaluation methodologies, and deployment in a web-based application, aimed at assisting healthcare professionals in early diagnosis and intervention.







# Tech Stack

### 1. Machine Learnning Algorithms:
- Random Forest
- Support Vector Machine (SVC)
- Logistic Regression

### 2. Web Development:

**Frontend:** 
- HTML&CSS
- JavaScript
 
**Backend:** 
- Flask
- Mysql 

### 3. IDE:
- Jupyter Lab
- VS code
## Run Locally
**1.** Open command prompt and navigate to the `project`folder. 

Create virtual environment  

```bash
    python -m venv my_env
```

Activate virtual environment

```bash
  my_env\Scripts\activate
```

Install dependencies using pip

```bash
  pip install requirements.txt
```
**2. Database design and Setup**:

Install and Launch MySQL and create a new database. 

You can use a tool like phpMyAdmin or the MySQL command line to create the database.

users Table:

   - `user_id` (Primary Key): Unique identifier for each user.
   - `name`: User's name.
   - `email`: User's email (used for login).
   - `password_hash`: Hashed password for security.

    CREATE TABLE users (
        user_id INT AUTO_INCREMENT PRIMARY KEY,
        name VARCHAR(255),
        email VARCHAR(255),
        password_hash VARCHAR(255),
        created_at TIMESTAMP DEFAULT            
        CURRENT_TIMESTAMP
    );
**3. Run the Application**:

 Run the following command in terminal/command prompt to start the Flask development server
    
```bash
  flask run
```
 This will start the Flask development server, and you'll see output similar to `Running on http://127.0.0.1:5000/` 

**4. Access the Application**:

Open a web browser and go to `http://127.0.0.1:5000/` to access the welcome page of the application.

   we can navigate to other routes defined in a code by appending the route paths to the base URL. For example, to access the signup page, go to `http://127.0.0.1:5000/rendersignup`

## Screenshots


![Performance Measure](https://github.com/Rakeshgl8/raki/assets/100138738/468fcebb-58df-478e-9532-9943047f9805)


![AUC_ROC](https://github.com/Rakeshgl8/raki/assets/100138738/ca4d3819-020c-4894-b90f-8d5f62556d5a)


## Feedback

If you have any feedback, please reach out to me at [![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rakesh-gl-78699a245?)

Please do ⭐ the repository, if you like this.😊

Thank you ❤
