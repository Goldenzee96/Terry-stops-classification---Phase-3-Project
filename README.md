# Terry-stops-classification---Phase-3-Project
This project analyzes Terry Stop data to predict whether an arrest occurs based on various factors. Using machine learning models, we aim to uncover key drivers of arrests and assess potential biases.
# Terry Stops Arrest Prediction

##  Project Overview
This project builds a machine learning model to predict whether an arrest will be made after a Terry Stop. Using real-world data, we analyze key factors that influence these arrests, such as the presence of weapons, time of stop, and subject demographics. Our goal is to provide data-driven insights to inform policing strategies and identify potential biases.

## Introduction
Terry Stops are a critical component of law enforcement, allowing officers to briefly detain individuals based on reasonable suspicion. However, concerns about fairness and potential bias in these stops have led to increased scrutiny. By analyzing data from past Terry Stops, we aim to uncover patterns, assess predictive factors, and provide recommendations for improved policing strategies.

##  Dataset
- **Source:** Publicly available Terry Stop data [https://www.oyez.org/cases/1967/67]
- **Key Features:**
  - Officer Age
  - Presence of Weapons
  - Time of Stop
  - Subject Demographics (e.g., Gender, Race)
  - Stop Resolution
- **Target Variable:** Whether an arrest was made (Binary: 0 = No Arrest, 1 = Arrest)

##  Key Questions
1. What factors influence an arrest after a Terry Stop?
2. Can we identify potential biases in Terry Stops?
3. How well can we predict arrests based on available data?
4. Can the model achieve both high accuracy and fairness?

## Exploratory Data Analysis (EDA)
- Stops involving weapons have a significantly higher arrest rate.
- Nighttime stops show a slight increase in arrests compared to daytime stops.
- Demographic disparities in stop outcomes suggest potential biases.

##  Models Used
###  Baseline Model: Logistic Regression
- Strengths: Simple, interpretable
- Weaknesses: Lower recall, struggles with complex relationships

###  Advanced Model: Random Forest
- Strengths: Higher predictive power, captures complex patterns
- Weaknesses: Less interpretable, risk of overfitting

##  Model Performance
| Model                | Precision | Recall | F1-Score |
|----------------------|----------|--------|----------|
| Logistic Regression | 0.91     | 0.85   | 0.88     |
| Random Forest       | 0.99     | 0.98   | 0.99     |

##  Evaluation Metrics
- **Precision:** Measures how many predicted arrests were correct.
- **Recall:** Evaluates how well the model identifies actual arrests.
- **F1-Score:** A balance between precision and recall to account for class imbalances.

##  Key Insights
- **Presence of Weapons** was the most influential factor in arrests.
- **Time of Stop** had a significant impact, suggesting potential policy revisions for nighttime policing.
- **Subject Demographics** played a role, emphasizing the need for bias monitoring.

##  Challenges & Limitations
- **Potential Data Bias:** Arrest data may reflect systemic biases rather than purely objective factors.
- **Feature Selection:** Some key influences on arrest decisions may not be present in the dataset.
- **Imbalanced Data:** Arrests occur in a small proportion of stops, requiring careful metric selection.

##  Recommendations
- **Policy Adjustments:** Revise nighttime policing strategies.
- **Training:** Emphasize de-escalation techniques for stops involving weapons.
- **Bias Monitoring:** Continuously audit the model to ensure fairness.

## Future Work
- Test additional models such as Gradient Boosting or Neural Networks.
- Incorporate external datasets for deeper context.
- Develop fairness-aware machine learning techniques to mitigate bias.

```

## Getting Started
### **Requirements**
- Python 3.x
- Libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`

### **Installation**
```bash
pip install -r requirements.txt
```

### **Run the Model**
```bash
python model.py
```

##  Contributors
 **Zena Margaret Gathoni Weru**  
[GitHub Profile](https://github.com/Goldenzee96/Terry-stops-classification---Phase-3-Project.git)

##  License
This project is licensed under the MIT License.

