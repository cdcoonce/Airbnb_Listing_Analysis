# AirBnB Listing Analysis

## The Situation

AirBnB, a platform that enables individuals to rent out their homes to travelers, is facing increasing regulatory pressures. As a newly hired Performance Analyst, the focus is to analyze Paris listings with an emphasis on pricing trends and the impact of regulations introduced in 2015.

## The Assignment

Leadership has requested a visual summary that outlines factors affecting pricing and assesses whether the 2015 regulations have influenced the Paris market. The analysis centers on examining the listing data to uncover key insights and provide actionable recommendations.

## Objectives

1. **Data Exploration and Quality Assurance**  
   - Examine the dataset to understand its structure, key variables, and any potential data quality issues.
   - Identify missing values, especially in critical fields such as the host registration date, and determine the best approach for imputation.
   - Validate numerical columns, ensuring that anomalies such as zero values in pricing are appropriately handled.

2. **Data Preparation**  
   - Filter the dataset to focus solely on Paris listings, reducing the column set to the most relevant fields such as host details, neighbourhood, accommodations, and price.
   - Reformat the data to facilitate time-series analysis, ensuring that dates are accurately represented and that non-numeric values do not interfere with aggregations.
   - Group the data by neighbourhood to calculate average pricing trends, and explore additional groupings to understand the influence of accommodations on price.

3. **Data Visualization and Insights**  
   - Develop visualizations that capture trends over time, such as the evolution of new hosts and average price per night.
   - Utilize dual-axis plots to compare multiple data series, ensuring that elements like legend placement are optimized for clarity.
   - Analyze the resulting graphs to interpret whether the 2015 regulations have led to fewer new hosts and higher prices, thereby identifying underlying market trends.

## Analysis Process and Findings

**Data Exploration:**  
The initial step involved loading the AirBnB listing data and reviewing its structure. Key fields such as listing ID, host information, and pricing were examined. It was discovered that certain fields, notably the host registration date, had missing values. These gaps were addressed by imputing the missing dates with an average value, ensuring that the dataset was complete for analysis.

**Filtering and Quality Assurance:**  
The dataset was refined to include only listings from Paris. This involved selecting essential columns such as the host registration date, neighbourhood, city, accommodations, and price. Additionally, any entries with a price of zero were removed, as these were deemed invalid for the analysis.

**Data Aggregation:**  
For a focused examination of pricing trends, the data was grouped by neighbourhood. The average price for each neighbourhood was calculated and sorted to provide insight into the variation of prices across Paris. An attempt to further group by accommodations highlighted the importance of accurate column naming and maintaining data integrity during the aggregation process.

**Visualization and Trends:**  
Time-series visualizations were created to compare the number of new hosts and the average price per night. A dual-axis plot was particularly effective in displaying these trends simultaneously. The visual analysis suggested that the 2015 regulatory changes were associated with a reduction in new host entries and an increase in average prices, providing a compelling narrative about the market’s response to regulation.

## Conclusion

The analysis of Paris AirBnB listings revealed critical insights into how regulatory changes may have reshaped market dynamics. By ensuring the data was clean and properly formatted, meaningful visualizations were produced that demonstrated:

- A decrease in the number of new hosts post-2015.
- An upward trend in the average price per night across various neighbourhoods.

These findings offer a data-driven foundation for further strategic decisions and highlight areas for potential policy adjustments. The insights gained from this project serve as a valuable asset in understanding and navigating the complex interplay between regulation and market behavior in the Paris AirBnB ecosystem.

## 6. Acknowledgments

This project was completed as part of a guided learning experience with **Maven Analytics**. Special thanks to Maven Analytics for providing structured guidance and high-quality datasets to enhance analytical skills.

---

## 🚀 Getting Started

This project uses [**uv**](https://github.com/astral-sh/uv) to manage Python environments and dependencies. It is designed to be run in a Jupyter Notebook environment.

### 🧰 Prerequisites

Install `uv` if you haven’t already:

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Verify it’s working:

```bash
uv --version
```

---

### 📥 Clone the Repository

Use the following command to clone this repository:

```bash
git clone https://github.com/cdcoonce/Airbnb_Listing_Analysis.git
cd Airbnb_Listing_Analysis
```

---

### 📦 Install Dependencies

Create a virtual environment and install dependencies:

#### On macOS / Linux

```bash
uv venv
source .venv/bin/activate
uv sync
```

#### On Windows (PowerShell)

```powershell
uv venv
.venv\Scripts\Activate
uv sync
```

> If using a `pyproject.toml`, you can install it in editable mode:

```bash
uv pip install -e .
```

---

### 📓 Run the Jupyter Notebook

Make sure ipykernel is installed:

```bash
uv pip install ipykernel
```

---

## 📁 Project Structure

```
your-repo-name/
├── notebooks/
│   └── EDA.ipynb
├── data/
│   └── ...
├── assets/
│   └── ...
├── pyproject.toml
├── README.md
└── ...
```

---

## 📬 Feedback and Contributions

Feel free to open issues or submit PRs!

