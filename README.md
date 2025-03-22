📊 Hypothesis Testing on Student Performance Based on Socio-Economic Survey
📌 Overview

This project investigates the relationship between socio-economic factors and student performance using statistical hypothesis testing. The dataset consists of student records with attributes like family background, parental education, financial status, and academic scores. By applying ANOVA and Chi-Square tests, we determine the impact of these socio-economic factors on student performance.
📂 Dataset

The dataset (Final-data.csv) contains various attributes related to student performance and socio-economic conditions. Key columns include:

    G1, G2, G3: Periodic exam scores.

    Final_Score: A derived metric based on weighted exam scores.

    Parental Education: Education level of parents.

    SES_Score: A derived feature representing socio-economic status.

    Romantic Relationship: Binary indicator (yes or no).

🔍 Steps in the Notebook
1️⃣ Data Preprocessing

    Importing required libraries: pandas, numpy, scipy.stats.

    Loading Final-data.csv and checking for missing values.

    Feature Engineering:

        Final_Score: Computed as 0.3*G1 + 0.3*G2 + 0.4*G3.

        SES_Score: Socio-economic metric derived from family attributes.

2️⃣ Hypothesis Testing
📌 ANOVA Test

    Used to determine if there is a significant difference in student performance across different socio-economic groups.

    Null Hypothesis (H₀): No difference in mean performance between groups.

    Alternative Hypothesis (H₁): At least one group differs significantly.

📌 Chi-Square Test

    Evaluates whether categorical socio-economic factors (e.g., parental education, financial support) have an impact on student performance.

    Null Hypothesis (H₀): No association between socio-economic factors and performance.

    Alternative Hypothesis (H₁): There is an association.

3️⃣ Results & Insights

    If p-value < 0.05, we reject H₀, meaning socio-economic factors do affect student performance.

    If p-value ≥ 0.05, we fail to reject H₀, meaning socio-economic factors do not have a significant impact.
