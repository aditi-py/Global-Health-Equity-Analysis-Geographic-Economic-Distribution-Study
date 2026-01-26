# Global Health Equity Analysis

A data analysis project examining the geographic and economic distribution of international health organizations to identify disparities in representation across income levels and world regions.

## Project Overview

This analysis investigates how 83 international organizations are distributed across different geographic regions and income classifications. By merging organizational data with UN demographic information, the project reveals significant concentration patterns and calculates population-adjusted representation metrics.

## Key Findings

- **70% of organizations** are headquartered in high-income countries
- **North America** accounts for 61% of organizations while representing only 4% of global population
- **Low-income countries** represent only 3.6% of organizational headquarters
- Significant disparities exist when comparing organizational presence to population distribution

## Datasets

1. **Awardee Organizations Dataset**: 83 organizations with headquarters country information
2. **UN Country Reference Data**: Country-level data including sub-region classifications, income levels, and population figures

## Technical Approach

### Data Processing
- Standardized country naming conventions across datasets
- Merged datasets on country identifiers
- Aggregated data by sub-region and income level
- Calculated population-relative metrics (organizations per million people)

### Analysis Components
1. **Income Level Distribution**: Analyzed concentration by World Bank income classifications
2. **Regional Distribution**: Examined geographic spread across UN sub-regions
3. **Population-Adjusted Analysis**: Normalized representation by regional population sizes

### Technologies Used
- **Python 3.x**
- **pandas**: Data manipulation and analysis
- **DuckDB**: SQL-based data querying
- **matplotlib**: Data visualization
- **numpy**: Numerical computations

## Visualizations

The analysis includes three key visualizations:
1. **Pie Chart**: Income level distribution of organizations
2. **Bar Chart**: Organizations by sub-region
3. **Stacked Bar Chart**: Combined view of income levels within each sub-region

## Key Insights & Limitations

### Insights
- Extreme geographic concentration in North America and high-income countries
- Significant under-representation of organizations in low and lower-middle income countries
- Population-adjusted metrics reveal stark disparities between organizational presence and demographic need

### Limitations
- Headquarters location may not reflect actual areas of operation or impact
- Population may not be the ideal denominator (disease burden or health needs data would be more appropriate)
- No information on funding amounts per organization
- Missing application pipeline data (selection vs. availability issue unknown)

## Project Structure

```
.
├── Global Health Equity Analysis.ipynb    # Main analysis notebook
├── README.md                  # Project documentation
└── data/                      # Data directory (not included)
    ├── Dataset 1 Awardees AFWH.csv
    └── Dataset 2 UN Countries.csv
```

## How to Run

1. Clone this repository:
```bash
git clone https://github.com/yourusername/global-health-equity-analysis.git
cd global-health-equity-analysis
```

2. Install required packages:
```bash
pip install pandas duckdb matplotlib numpy
```

3. Run the Jupyter notebook:
```bash
jupyter notebook Lever_for_change.ipynb
```

## Future Improvements

- Implement automated ETL pipeline with country name standardization
- Add data quality validation checks
- Incorporate funding amount analysis
- Include application pipeline data to distinguish selection from availability issues
- Add interactive visualizations using plotly or similar tools

## Assumptions

This analysis assumes:
- Data is complete and clean with no duplicates
- Each country maps to exactly one sub-region
- No data inconsistencies in country classifications
- Population data is current and accurate

## Author

Aditi Neema

## License

This project is available under the MIT License.

---

*Note: This analysis was completed as a time-constrained exploratory project. Data sources and specific organizational details have been anonymized.*
