# 🚢 Titanic Survival Prediction

## 🌟 Project Overview
This project uses machine learning to predict passenger survival on the Titanic, focusing on how demographic and socio-economic factors influenced survival outcomes. The goal is to enhance historical understanding and inform future safety protocols.

## 📊 Data Description
The dataset consists of passenger information such as age, sex, ticket class, and survival status. It is structured for a comprehensive analysis of factors that influenced survival rates.

## 🔍 Data Preprocessing and Analysis
- 🛠 Handling Missing Values: Missing data in 'Age', 'Cabin', and 'Embarked' fields were imputed to maintain data integrity.
- ✨ Feature Engineering: New features like 'FamilySize' were created from 'SibSp' and 'Parch' to assess the impact of traveling with family.
- 🔄 Encoding Categorical Variables: Transformed 'Sex' and 'Embarked' into numeric formats to fit machine learning models.


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

### Title: Ethical Analysis of Titanic Dataset and Machine Learning Models

#### Overview of Biases in the Dataset:
- **Gender Bias:** The Titanic survival data shows that females had a higher survival rate compared to males. This reflects the "women and children first" societal norm, which may introduce a gender bias into predictions.
- **Class Bias:** Passengers in higher classes (Pclass 1) had significantly higher survival rates due to better access to lifeboats. Lower-class passengers faced a survival disadvantage, reflecting socioeconomic biases.
- **Age Bias:** Children were prioritized during the rescue, leading to higher survival rates among younger passengers, creating an age-based skew in predictions.

#### Biases in Model Predictions:
- Models trained on such datasets might reinforce biases. For example, predictions might unfairly prioritize females and higher-class passengers as more "likely" to survive.
- **Impact on fairness:** While models might achieve high accuracy, they can unintentionally discriminate against groups (e.g., predicting fewer males and third-class passengers to survive).

#### Trade-offs Between Accuracy and Fairness:
- **Accuracy:** Models like Decision Trees and Random Forest achieved high accuracy (99–100%), but this might be due to overfitting rather than generalization. Bias in the data influences these results.
- **Fairness:** Optimizing for fairness requires balancing predictions across gender, class, and age without overly relying on one group to improve accuracy.

#### Real-World Implications of Bias:
- If deployed in real-world scenarios (e.g., disaster planning), biased models may prioritize certain groups for rescue or resources unfairly.
- The use of biased predictions may perpetuate societal inequalities rather than addressing them.

#### Recommendations for Fair Models:
- Use Fairness-aware techniques (e.g., fairness constraints, sampling techniques).
- Evaluate performance using metrics beyond accuracy, such as fairness disparity scores.
- Ensure transparency and explainability in predictions to identify biases in real-world deployments.

