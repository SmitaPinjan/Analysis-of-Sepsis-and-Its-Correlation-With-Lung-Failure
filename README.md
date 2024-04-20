# Analysis of Sepsis and Its Correlation With Lung Failure

### Table of Contents

- [Problem Statement](#problem-statement)
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Visualization](#visualization)
- [Insights](#insights)
- [Recommendations](#recommendations)
- [References](#references)

---

### Problem Statement
Sepsis is a serious medical condition caused by the body’s improper response to an infection which leads to damage to its vital organs and may lead to death. Due to their critical conditions, patients admitted to ICU are more prone to be diagnosed with Sepsis Infection. Therefore, early detection of Sepsis signs will help to curb the infection and save patients by initiating proper and in-time treatment. 

Through this project, I am attempting to create a dashboard that can alert the healthcare team about possible signs of Sepsis that can lead to Lung failure of patients. So the healthcare providers can take immediate action and initiate the treatment.

---

### Project Overview

This data analysis project aims to provide insight into the Sepsis Patient Dataset to determine the correlation with Lung or Respiratory failure. By analyzing various aspects of the data, I am seeking to gain a deeper understanding of the correlation between different biomarkers, and how it will affect the sepsis patient based on this analysis will provide recommendations to detect early signs of Sepsis infection.

### Data Sources 

Sepsis Patient Dataset: The primary dataset used for this analysis is the "Dataset1.xlsx" file, containing 40336 unique patients and their lab result information.
Size of the sample: 1.5M. The data has 43 features which can broadly be classified into
- Demographics
- Vital Signs
- Laboratory values
  Different biomarkers are different tests and conditions that can help to identify Sepsis, its symptoms, stages, and diagnosis. Eg. O2Sat, HCO3, PaCO3, SBP, DBP, HR, Temp, Resp etc.
- Total no. of patients: 40336
- The dataset is provided by Numpy Ninja and used for the data analysis.

### Tools 
Tools used for Data Analysis and Report generation :
- Excel
- Tableau 

### Exploratory Data Analysis

EDA involved exploring the Sepsis Patient dataset to answer key questions, such as:

- What is the correlation between Sepsis infection and different biomarkers or lab tests?
- How and what are different biomarkers that will contribute to lung or respiratory failure of Sepsis Patients?

### Data Analysis

Include some interesting codes/features that I have worked with
- LOD functions, Calculated fields. For example
  ~~~ Calculated field using LOD function
     Count of Sepsis, Non-Sepsis, Onset Patients :
        IF {FIXED [Patient ID] : MIN([Sepsis Label])} = 1 THEN "Sepsis Patient"
        ELSEIF {FIXED [Patient ID] : MIN([Sepsis Label])} = 0 AND
                {FIXED [Patient ID] : MAX([Sepsis Label])} = 1 THEN "Onset Patient"
        ELSE "Non-Sepsis Patient"
        END
  ~~~

### Visualization

- Advanced visualization charts like Funnel charts, Stacked Sunburst charts, Heatmap charts, Dendrogram charts, Infrographic charts etc.
- Customized dashboard.
  - Tableau Link: [Analysis of Sepsis and Its Correlation With Lung Failure | Tableau Public](https://public.tableau.com/views/AnalysisofSepsisandItsCorrelationWithLungFailure/AnalysisofSepsisandItsCorrelationWithLungFailure?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link)
    
![image](https://github.com/SmitaPinjan/Analysis-of-Sepsis-and-Its-Correlation-With-Lung-Failure/assets/152721562/ed403ed1-eca6-4784-9168-bc13a3ade6bc)

![image](https://github.com/SmitaPinjan/Analysis-of-Sepsis-and-Its-Correlation-With-Lung-Failure/assets/152721562/d224fa77-c82b-403e-8c17-8d37b86c40d7)

![image](https://github.com/SmitaPinjan/Analysis-of-Sepsis-and-Its-Correlation-With-Lung-Failure/assets/152721562/449a5004-b3ba-448f-93c7-f6cf1ad1d62f)

![image](https://github.com/SmitaPinjan/Analysis-of-Sepsis-and-Its-Correlation-With-Lung-Failure/assets/152721562/4c33065f-b1fe-4743-a1af-b2fb643e606f)

![image](https://github.com/SmitaPinjan/Analysis-of-Sepsis-and-Its-Correlation-With-Lung-Failure/assets/152721562/85cb1e6a-2ae5-473d-9286-fece7b784108)

![image](https://github.com/SmitaPinjan/Analysis-of-Sepsis-and-Its-Correlation-With-Lung-Failure/assets/152721562/6da9846c-7476-4e0d-b3da-192b537fac7f)

![image](https://github.com/SmitaPinjan/Analysis-of-Sepsis-and-Its-Correlation-With-Lung-Failure/assets/152721562/98bc2e43-3e95-45f6-93e2-46f144bbab8f)

![image](https://github.com/SmitaPinjan/Analysis-of-Sepsis-and-Its-Correlation-With-Lung-Failure/assets/152721562/f336a596-85c6-47ed-9f46-a3521d2d3402)

 
### Insights

As per my analysis, among all patients with Sepsis, Onset and SIRS, around 10%  to 20% of patients who experience either Lung, Kidney, Heart or Liver Failure are at high risk of mortality exceeding 90%.
Some of the key insights:

- As analysed, 1% patients were sepsis, 6% were onset sepsis (who didnt have spesis when admitted but later-on diagoned with sepsis). So bascially for evry 100 patients, 7 patients are diagonsed with Sepsis infection.
- Sepsis patients those transferred from hospital to ICU were 95% compared to those who transferred from ICU to hospital were 0.1%. This indicates the recovery rate of Sepsis patient is minimal. Therefore, early detection of Sepsis is essential for better treatment.
- As per analysis, 31% patients showed signs of Acute Respiratory Distress Syndrom (ARDS) and Hypoxemia.Among those, 60-70% of female and 70-80% of male patients between age group 20-40 are having highest risk of respiratory failure.
- 60% of patients admitted in ICU shown SIRS (Systemic Inflammatory Response Syndrom) condition which indicates the early signs of Sepsis infection.
- As analyzed, 4% of patients with Severe Respiratory System failure risks, 7% with Severe Renal System Failure, 2% with Severe Liver Failure, 1% with Severe Coagulation failure risk have a moderate to severe risk of Multi-Organ failure risk.

- More detailed analysis results are summarized in the presentation file below. Please check the Presentation file for the detailed analysis including the dashboard, insights and findings for more information. 
[Sepsis Analysis Presentation (3).pptx](https://github.com/SmitaPinjan/Analysis-of-Sepsis-and-Its-Correlation-With-Lung-Failure/files/15046771/Sepsis.Analysis.Presentation.3.pptx)

### Recommendations

Based on the analysis, I recommend the following actions:
- Healthcare professionals can implement similar dashboards to alert the caregiver whenever a Patient's condition starts changing abnormally.
- Implement a strategy to detect early signs of Sepsis and provide proper diagnosis.

### References
As provided in the presentation file.

|Heading1|Heading2|
|--------|--------|
|Content |Content2|
|Data Analysis| Tableau|
