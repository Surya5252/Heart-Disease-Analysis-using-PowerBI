<h1>Heart Disease Analysis using Power BI <img width=125 align=right src="https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=Power%20BI&logoColor=white"></h1>

Cardiovascular diseases (CVDs) are the leading cause of death globally, claiming an estimated 17.9 million lives each year. The impact of behavioral risk factors can manifest in individuals, and identifying those at the highest risk is crucial for preventing premature deaths through appropriate treatment [(WHO)](https://www.who.int/health-topics/cardiovascular-diseases).

In this project, we explore how CVDs affect different patients based on factors like sex and age. We will analyze and visualize data from patient diagnoses to determine whether they have the disease.

These interactive visuals can assist medical professionals in prescribing treatments by comparing patient diagnosis data with our analyzed data, significantly reducing the time needed to identify patient issues.

By leveraging a large volume of data, decisions can be made with greater accuracy than relying on intuition alone. The use of analytics in healthcare enhances care by enabling preventive measures, allowing trends, patterns, and outliers within large datasets to be quickly identified.

## Problem Statement

The healthcare system increasingly relies on wearable, smart, and handheld devices, generating vast amounts of data. However, this massive influx of data makes it challenging for medical professionals to interpret and utilize it effectively for future prognosis. The process of analyzing numerical data is time-consuming and prone to misinterpretation, potentially leading to incorrect diagnoses. The current situation is compounded by a lack of meaningful clinical intelligence at the point of care and poor data visualization, both of which contribute to significant challenges within the healthcare industry.

## Solution

Power BI is an interactive data visualization tool that enables the creation of striking, engaging, and meaningful visualizations. It helps to simplify complex and intricate healthcare data, breaking it down into manageable components. This provides healthcare providers with deeper insights into how to deliver the highest quality care to patients while also achieving their strategic goals.

## Description

In this project, I used the Heart Disease dataset from UCI to identify the key factors contributing to heart disease.

The dashboard features two tabs—**Key Influencers** and **Top Segments**—along with two slicers for interactive data exploration.

<details><summary><b>Key Influencers</b></summary> 
<img align=right src='https://github.com/Zayd1602/Heart-Disease-Analysis-using-PowerBI/blob/main/Key-Influencers.png'/>

1. **Key Influencers Tab**: This tab highlights the key factors affecting the selected metric. In our case, the top factor leading to a positive heart disease diagnosis is Exercise-Induced Angina.
2. **Visualization**: A column chart or scatter plot displays the distribution of the selected factor, providing additional context.
3. **Influencer Bubbles**: Each influencer's bubble is encircled by a ring representing the approximate percentage of data that influencer contains. A more complete ring indicates a larger portion of data influenced by that factor.
4. **Interactivity**: You can select different factors to observe their effects on the heart disease diagnosis.

</details>

<details><summary><b>Top Segments</b></summary>   
<img align=right src='https://github.com/Zayd1602/Heart-Disease-Analysis-using-PowerBI/blob/main/Top-Segments.png'/>

1. **Top Segments Tab**: This tab displays the top segments identified by Power BI from the dataset for the selected metric.
2. **Segment Overview**: Initially, it provides an overview of all segments, ranked by the presence of heart disease (True/False) and population size. The higher the bubble, the greater the percentage of heart disease detected. 
3. **Bubble Size**: The size of each bubble represents the number of patients within that segment.
4. **Detailed View**: Selecting a bubble reveals detailed information about that segment.

</details>

- **Visualization Filters**: The visualizations are filtered by whether heart disease was detected (True/False).
- **Slicers**: Slicers are used to filter the dataset displayed in the report visualizations. I included two slicers: one for filtering by age range and another for filtering by gender or both.

---

## Conclusion

From the dataset, it was found that female patients are more likely to have heart disease, with the condition most prevalent in individuals aged 29 to 54.

**Key Factors Affecting Disease Diagnosis:**

1. **Exercise-Induced Angina**: This is negative in 69.61% of patients, making them 3 times more likely to have the disease.
2. **Chest Pain Type (1)**: Present in 89% of patients with this type of chest pain, making it 2.32 times more likely to be associated with the disease.
3. **Number of Major Blood Vessels (Type 0)**: Found in 74.29% of patients, this factor is 2.13 times more likely to be linked to the disease.
4. **Slope of the Peak Exercise ST Segment (Type 2)**: Present in 75.35% of patients, this factor is 2.09 times more likely to be associated with the disease.

<div align="center"> 
<img width=800 src="https://github.com/Zayd1602/FRT-Project-using-PowerBI/blob/main/Overall-visual.gif">
</div>

---

## About the Dataset

The dataset contains 13 attributes that we’ll use to predict the target variable: whether a patient has heart disease (1) or not (0).

<details><summary><b>Click to learn more about the features</b></summary>   

1. **age**: Age of the patient (in years).

2. **sex**: Gender (1 = male; 0 = female).

3. **cp**: Chest pain type:
   - **0**: Typical angina (all criteria met).
   - **1**: Atypical angina (two of three criteria met).
   - **2**: Non-anginal pain (less than one criterion met).
   - **3**: Asymptomatic (none of the criteria met).
   These classifications are based on the presence of chest pain in the substernal area, its occurrence due to emotional/physical stress, and its relief through nitroglycerine or rest.

4. **trestbps**: Resting blood pressure (in mmHg, recorded at hospital admission).

5. **chol**: Serum cholesterol level (in mg/dL).

6. **fbs**: Fasting blood sugar > 120 mg/dL (1 = true; 0 = false, indicating possible diabetes).

7. **restecg**: Resting electrocardiogram results:
   - **0**: Normal.
   - **1**: ST-T wave abnormality (indicating possible heart issues).
   - **2**: Left ventricular hypertrophy (based on Estes' criteria).

8. **thalach**: Maximum heart rate achieved.

9. **exang**: Exercise-induced angina (1 = yes; 0 = no).

10. **oldpeak**: ST depression induced by exercise relative to rest (measured in mm).

11. **slope**: Slope of the peak exercise ST segment:
    - **0**: Upsloping.
    - **1**: Flat.
    - **2**: Downsloping.
    These abnormalities are crucial indicators of potential ischemia.

12. **ca**: Number of major vessels (0-4) colored by fluoroscopy. A higher number of colored vessels correlates with a higher likelihood of heart disease.

13. **thal**: Thallium stress test results:
    - **0**: Normal.
    - **1**: Fixed defect (heart tissue can't absorb thallium under stress or at rest).
    - **2**: Reversible defect (heart tissue can't absorb thallium under stress but can at rest).

14. **target**: The target variable indicating the presence (1) or absence (0) of heart disease.

</details>

> **Note**: The column names were modified during data transformation in Power BI.
