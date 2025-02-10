# DECODE: Data Preparation for Hospital Length of Stay Prediction
# Equitable Hospital Length of Stay Prediction for Patients with Learning Disabilities and Multiple Long-term Conditions Using Machine Learning

This is the Python repository for the paper ["Equitable Hospital Length of Stay Prediction for Patients with Learning Disabilities and Multiple Long-term Conditions Using Machine Learning"](https://www.frontiersin.org/journals/digital-health/articles/10.3389/fdgth.2025.1538793/abstract).\
The code obtains and extracts variables from several electronic health records databases for Welsh patients and creates structured tabular data of selected features for a machine learning prediction of the hospital's length of stay.
Please cite our paper, if the code is used for publishing research.
![Fig2_page-0001](https://github.com/user-attachments/assets/18ebe535-c54c-46b7-8300-bc6b5f27d063)

Fig1. Consort Flow Diagram


Purpose:
Individuals with learning disabilities (LD) often face higher rates of premature mortality and prolonged hospital stays compared to the general population. Predicting the length of stay (LOS) for patients with LD and multiple long-term conditions (MLTCs) is critical for improving patient care and optimising medical resource allocation. However, there is limited research on the application of machine learning (ML) models to this population. Furthermore, approaches designed for the general population often lack generalisability and fairness, particularly when applied across sensitive groups within their cohort.

Method:
This study analyses hospitalisations of 9,618 patients with LD in Wales using electronic health records (EHR) from the SAIL Databank. The target patient extraction setup is detailed in Fig 1. A Random Forest (RF) ML model was developed to predict hospital LOS, incorporating demographics, medication history, lifestyle factors, and 39 long-term conditions. To address fairness concerns, two bias mitigation techniques were applied: a post-processing threshold optimizer and an in-processing reductions method using an exponentiated gradient. These methods aimed to minimise performance discrepancies across ethnic groups while ensuring robust model performance.

Results:
The Random Forest (RF) model outperformed other state-of-the-art models, achieving an Area Under the Curve (AUC) of 0.759 for males and 0.756 for females, a false negative rate (FNR) of 0.224 for males and 0.229 for females, and a balanced accuracy of 0.690 for males and 0.689 for females. Bias mitigation algorithms reduced disparities in prediction performance across ethnic groups, with the threshold optimizer yielding the most notable improvements. Performance metrics, including false positive rate and balanced accuracy, showed significant enhancements in fairness for the male cohort.

Conclusion:
This study demonstrates the feasibility of applying ML models to predict LOS for patients with LD and MLTCs, while addressing fairness through bias mitigation techniques. The findings highlight the potential for equitable healthcare predictions using EHR data, paving the way for improved clinical decision-making and resource management.}

Keywords: learning disabilities, Length of Stay.
