# 🚢 Titanic Survival Prediction

## 🌟 Project Overview
This project uses machine learning to predict passenger survival on the Titanic, focusing on how demographic and socio-economic factors influenced survival outcomes. The goal is to enhance historical understanding and inform future safety protocols.

## 📊 Data Description
The dataset consists of passenger information such as age, sex, ticket class, and survival status. It is structured for a comprehensive analysis of factors that influenced survival rates.

## 🔍 Data Preprocessing and Analysis
- 🛠 Handling Missing Values: Missing data in 'Age', 'Cabin', and 'Embarked' fields were imputed to maintain data integrity.
- ✨ Feature Engineering: New features like 'FamilySize' were created from 'SibSp' and 'Parch' to assess the impact of traveling with family.
- 🔄 Encoding Categorical Variables: Transformed 'Sex' and 'Embarked' into numeric formats to fit machine learning models.

### 📊 Histogram of Oriented Gradients (HOG) Feature Extraction
- **HOG Implementation**: We utilized the Histogram of Oriented Gradients (HOG) technique to extract detailed texture and shape information from images associated with the data. This method is pivotal for capturing edge directions and intensities, which are vital for feature discrimination in image-based data.
- **Purpose**: The HOG features are especially beneficial for enhancing the model's ability to discern subtle variations in the visual data that might correlate with survival patterns, such as distinguishing clothing or accommodation types that are not explicitly labeled in the dataset.


### ➡️ Exploratory Data Analysis (EDA)
- 🔎 Univariate Analysis: Focused on the distributions of individual features to understand their basic properties.
- 🔗 Bivariate Analysis: Explored relationships between two variables and their impact on survival.
- 🌐 Multivariate Analysis: Investigated interactions between multiple variables to uncover complex patterns affecting survival.

## 🧠 Models Used and Their Rationale
To predict survival, we employed several models, each chosen for its unique strengths in handling classification tasks:

- ➖ Logistic Regression: Used for its efficiency and effectiveness in binary classification problems. It provides a probabilistic framework that allows for easy interpretation of feature importance.

- 🌳 Decision Tree Classifier: Offers a visual representation of decision-making processes, making it useful for understanding the feature splits that most significantly impact survival. It's also beneficial for handling non-linear data relationships.

- 🌲 Random Forest Classifier: An ensemble method that improves on the decision tree's performance by reducing overfitting through averaging multiple trees. It's known for its high accuracy and robustness across various types of data.

- 🔍 Support Vector Machine (SVC): Chosen for its ability to find the optimal boundary between possible outputs, which is crucial in clear-cut classification tasks like survival prediction. It works well with clear margin of separation and is effective in high-dimensional spaces.

The **Random Forest Classifier** 🌲 was ultimately selected as the primary model due to its superior performance in managing overfitting while maintaining a high level of accuracy, making it exceptionally suitable for this predictive modeling task.

## 🛠 Technologies Used
- 🐍 Python: For programming and data manipulation.
- 📈 Pandas & NumPy: For data handling and numerical calculations.
- 🤖 Scikit-Learn: For implementing machine learning algorithms.
- 📊 Matplotlib & Seaborn: For data visualization to uncover underlying patterns and results.

## 📈 Key Insights
- 📉 The analysis revealed significant survival differences based on gender, class, and age.
- 🚀 The findings contribute valuable insights toward improving maritime safety and emergency preparedness.

## 📝 Conclusions
This project illustrates the power of machine learning in historical data analysis, providing deep insights into the dynamics at play during the Titanic disaster.

