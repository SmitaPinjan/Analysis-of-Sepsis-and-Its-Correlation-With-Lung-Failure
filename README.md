# Analysis of Sepsis and Its Correlation With Lung Failure

### Table of Contents

- [Problem Statement](#problem-statement)
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
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

- Advanced visualization charts like Funnel charts, Stacked Sunburst charts, Heatmap charts, Dendrogram charts, Infrographic charts etc.
- Customized dashboard.
  - Tableau Link: [Analysis of Sepsis and Its Correlation With Lung Failure | Tableau Public](https://public.tableau.com/views/AnalysisofSepsisandItsCorrelationWithLungFailure/AnalysisofSepsisandItsCorrelationWithLungFailure?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link)

 
### Insights

As per my analysis, among all patients with Sepsis, Onset and SIRS, around 10%  to 20% of patients who experience either Lung, Kidney, Heart or Liver Failure are at high risk of mortality exceeding 90%
- The Analysis results are summarized in the presentation file. Please check the Presentation file for the detailed analysis including the dashboard, insights and findings for more information.

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
