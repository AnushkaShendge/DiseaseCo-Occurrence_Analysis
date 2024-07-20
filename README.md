# Disease Co-Occurrence Analysis

This project aims to identify common co-occurrences of diseases or symptoms using association rule mining. The goal is to improve diagnostic processes and treatment plans by analyzing patterns in medical data.

## Project Description

Using the MIMIC-III Clinical Database and healthcare data from Kaggle, we perform data preprocessing and apply the Apriori algorithm to find frequent itemsets and generate association rules. The results are visualized using various graphs to provide a clear understanding of the relationships between different diseases.

## Dataset

- MIMIC-III Clinical Database
- Healthcare Data from Kaggle

The dataset contains the following columns:

- Name
- Age
- Gender
- Blood Type
- Medical Condition
- Date of Admission
- Doctor
- Hospital
- Insurance Provider
- Billing Amount
- Room Number
- Admission Type
- Discharge Date
- Medication
- Test Results

## Overview

This project involves analyzing disease co-occurrence using the MIMIC-III Clinical Database and healthcare data from Kaggle. The analysis employs association rule mining with the Apriori algorithm to uncover patterns in disease relationships.

## Results

The association rules are saved in the `results/rules.csv` file. Example rules include:

| Left Hand Side | Right Hand Side | Support | Confidence | Lift |
|----------------|-----------------|---------|------------|------|
| Arthritis      | Diabetes        | 0.1677  | 0.1677     | 1.0  |
| Asthma         | Hypertension    | 0.1655  | 0.1655     | 1.0  |
| Cancer         | Obesity         | 0.1663  | 0.1663     | 1.0  |

## Visualization
![Screenshot 2024-07-20 215802](https://github.com/user-attachments/assets/72979523-c9ff-460c-bf1d-6768c5adfed1)


The following visualizations help in understanding the significance of the association rules:

- **Bar Plot of Association Rule Metrics**: This bar plot visualizes the support, confidence, and lift values for each association rule. It helps in understanding which rules are more significant based on these metrics.
![Screenshot 2024-07-20 215823](https://github.com/user-attachments/assets/9b9e3290-fe0b-42e5-97f3-ee5af02adecf)


- **Heatmap of Support Values**: This heatmap shows the support values for the co-occurrence of diseases. The intensity of color represents the frequency of co-occurrence, which helps in identifying patterns in disease relationships.

- **Pair Plot of Confidence and Lift**: This pair plot visualizes the relationships between support, confidence, and lift values for the association rules. It provides insights into how these metrics correlate with each other.

![Screenshot 2024-07-20 215858](https://github.com/user-attachments/assets/bd384923-d06a-4061-8714-2b5492e30e9c)


## Getting Started

To run this project, clone the repository and install the necessary dependencies:

```bash
git clone https://github.com/your-username/disease-co-occurrence-analysis.git
cd disease-co-occurrence-analysis
pip install -r requirements.txt
