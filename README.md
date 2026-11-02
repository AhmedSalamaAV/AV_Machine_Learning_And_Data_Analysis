# AV Classroom Analysis with Python and Machine Learning

An exploratory project connecting AV systems design with data analysis and machine learning using records for **204 classrooms** at the University of Illinois Chicago.

## Project Overview

Publicly available classroom records were converted into a structured dataset to explore how AV system types vary with room capacity, floor area, and furniture.

The workflow includes:
- Data cleaning and missing-value analysis.
- Feature engineering and data visualisation.
- Comparisons of AV systems across room characteristics.
- K-means clustering using standardised capacity and area.
- Cluster interpretation and stability checks.

## Key Findings

- **15 classrooms** had no recorded AV system type, all within one building.
- AV system categories varied among rooms with similar capacity and area.
- An exploratory **four-cluster solution** distinguished two groups of large rooms with different spatial and furniture characteristics, despite sharing the same recorded AV system category.
- The four-cluster solution achieved a **silhouette score of 0.790** and identical assignments across five tested random seeds (**ARI = 1.0**). These are clustering evaluation results, not predictive accuracy.

## Tools

Python, pandas, NumPy, Matplotlib, and scikit-learn.

## How to Explore

Open the `.ipynb` notebook in this repository to view the saved code, charts, and findings.

To run it in Google Colab:
1. Open the notebook in Colab.
2. Upload the included CSV dataset.
3. Update the `pd.read_csv(...)` path to match the uploaded file.
4. Run the notebook cells in order.

## Data Source

[University of Illinois Chicago — Classroom Database](https://classrooms.uic.edu/Public/Search)

Source records belong to their respective owner. This is an independent educational project and is not affiliated with UIC.

## Limitations

The analysis describes recorded equipment categories and room characteristics. It does not determine whether a room requires an upgrade or recommend specific AV equipment. Final design decisions require site surveys, room layouts, equipment details, and user requirements.

## Author

Ahmed Salama — AV Systems Designer
