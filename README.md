# Educational-Data-Mining-Student-Dropout-Prediction
This is a project on 'Educational Data Mining',  used IBM SPSS Modeler to predict student dropout risks by analyzing academic and behavioral patterns.

# Student Dropout Prediction & Performance Analysis
**Tool Used:** IBM SPSS Modeler  
**Accuracy:** ~89.4% (C5.0 Algorithm)

##  Project Overview
This project applies Educational Data Mining (EDM) to identify students at risk of academic failure. By analyzing 1,044 student records, we built a predictive system that flags "at-risk" individuals before the final exam.

##  Repository Structure
* **/Data**: Contains `student-mat.csv` and `student-por.csv`.
* **/Screenshots**: Visual proof of the SPSS Stream and Model Results.
* `Student_Analysis.str`: The original SPSS Modeler Stream file.

##  The Workflow
We followed the CRISP-DM methodology:
1. **Data Ingestion**: Merged Math and Portuguese datasets using an **Append Node**.
2. **Feature Engineering**: Created `PassFail` and `Total_Grade` using the **Derive Node**.
3. **Modeling**: Compared **C5.0**, **CHAID**, and **K-Means** clustering.
4. **Validation**: Used a **Partition Node** (70/30) to ensure high predictive power.

##  Key Results
* **Top Predictor**: G1 (First Period Grade) has an 80% correlation with final outcomes.
* **Risk Factors**: 2+ past failures and high absenteeism (>15 days) are critical red flags.
* **Success Rate**: The C5.0 model correctly identifies 89% of student outcomes.
