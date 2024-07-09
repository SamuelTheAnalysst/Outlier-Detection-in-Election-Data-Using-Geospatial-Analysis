# Outlier Detection in Election Data Using Geospatial Analysis

## Case Study: Ensuring Election Integrity

### Introduction

In the recently concluded election, the Independent National Electoral Commission (INEC) faced multiple legal challenges concerning the integrity and accuracy of the election results. As a data analyst intern at [HNG](https://hng.tech/internship), I was tasked with uncovering potential voting irregularities to ensure transparency in the election results.

### Objectives

- **Dataset Preparation:**
  - Locate and download the dataset for Niger state.
  - Ensure the dataset includes longitude and latitude values for each polling unit.
  - Clean the dataset for accuracy and completeness.
- **Neighbors Identification:**
  - Identify neighboring polling units based on geographical proximity.
- **Outlier Score Calculation:**
  - Compare the votes each party received with those of neighboring units.
  - Calculate an outlier score for each party.
- **Sorting and Reporting:**
  - Sort the dataset by outlier scores.
  - Highlight the top outliers and their neighboring polling units.

### Methodology

1. **Dataset Preparation:**
   - Downloaded and cleaned the dataset to include accurate location data.
2. **Neighbors Identification:**
   - Used geopy to calculate distances and identify neighbors within a 15 km radius.
3. **Outlier Score Calculation:**
   - Calculated outlier scores for each party by comparing the votes with neighboring units.

### Summary of Findings

Significant deviations in votes were identified in several polling units, indicating potential irregularities. Below are examples of top outliers:

- **Polling Unit: KACE I (APC)**
  - **Votes:** 44
  - **Neighbor Mean Votes:** 440
  - **Absolute Difference:** 396

- **Polling Unit: UNGUWAR SARKI (LP)**
  - **Votes:** 5
  - **Neighbor Mean Votes:** 125
  - **Absolute Difference:** 120

- **Polling Unit: SABON GARI (PDP)**
  - **Votes:** 100
  - **Neighbor Mean Votes:** 200
  - **Absolute Difference:** 100

- **Polling Unit: GALADIMA (NNPP)**
  - **Votes:** 120
  - **Neighbor Mean Votes:** 30
  - **Absolute Difference:** 90

### Conclusion

This analysis provided insights into potential voting irregularities, warranting further investigation to ensure election integrity.

### Recommendations

- Investigate the identified outliers.
- Implement measures to ensure data integrity in future elections.
- Use advanced statistical techniques for more comprehensive outlier detection.


### Data Sources
◾ IINEC Election Data (https://inecnigeria.org/election-data)

### Acknowledgments
◾ HNG Internship (https://hng.tech/internship)
◾ All contributors and reviewers.
