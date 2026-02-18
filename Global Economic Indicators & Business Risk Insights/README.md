---
# Public API JSON Economic Analysis
**Macroeconomic Stability & Business Risk Assessment**
---

## Project Overview  

	This project demonstrates structured analysis of public macroeconomic data retrieved via the World Bank Open Data API. The objective is to extract, validate, and communicate insights from JSON-based economic indicators — with an emphasis on reproducibility, documentation clarity, and business interpretation.

	The analysis evaluates long-term trends in:

	* GDP Growth (annual %)
	* Inflation (annual %)

	Across three economies:

	* Nigeria
	* Ghana
	* Kenya

	The project is designed to showcase not only data analysis skills, but disciplined technical documentation, traceable methodology, and structured insight communication.

---

## Analytical Objective

	**Primary Question:**

	How do inflation trends and GDP growth volatility differ across selected African economies, and what are the macroeconomic risk implications?

	This project explores:

	* Long-term volatility patterns
	* Inflation–growth co-movement
	* Comparative macroeconomic stability
	* Business risk implications

---

## Data Source

	Data is retrieved directly from the World Bank Indicators API.

	Official API Documentation:
	[https://datahelpdesk.worldbank.org/knowledgebase/articles/889392-about-the-indicators-api-documentation](https://datahelpdesk.worldbank.org/knowledgebase/articles/889392-about-the-indicators-api-documentation)

	Indicators Used:

	* GDP Growth: `NY.GDP.MKTP.KD.ZG`
	* Inflation (Consumer Price Index): `FP.CPI.TOTL.ZG`

	Example API Endpoint:

	```
	http://api.worldbank.org/v2/country/NGA;GHA;KEN/indicator/FP.CPI.TOTL.ZG?format=json
	```

	Data is returned in nested JSON format and normalized into analysis-ready tabular structures using Python.

---

## Technical Stack

	* Python
	* Pandas
	* NumPy
	* Matplotlib
	* Requests (API retrieval)
	* Jupyter Notebook

---

## Workflow Summary

	The notebook follows a structured analytical workflow:

	### 1. Problem Definition

	Clear articulation of the macroeconomic question and stakeholder relevance.

	### 2. JSON Data Ingestion

	* API request handling
	* Inspection of nested JSON structure
	* Separation of metadata from observation records

	### 3. Data Normalization

	* Use of `pandas.json_normalize()`
	* Column selection and renaming
	* Structured tabular transformation

	### 4. Data Validation

	* Missing value analysis
	* Year consistency checks
	* Country-level completeness validation

	### 5. Indicator Merging

	* Alignment of GDP and Inflation datasets
	* Join methodology documentation
	* Explanation of merge assumptions

	### 6. Exploratory Analysis

	* Inflation trends over time
	* GDP growth volatility
	* Cross-country comparisons
	* GDP vs Inflation scatter analysis

	### 7. Insight Interpretation

	* Structured “Key Findings”
	* Volatility assessment
	* Inflation-growth co-movement analysis

	### 8. Business Implications

	* Macroeconomic risk assessment
	* Strategic investment considerations
	* Risk-adjusted planning insights

	### 9. Reproducibility Notes

	* API endpoints documented
	* Retrieval date noted
	* Environment dependencies listed

---

## Key Analytical Themes

	* Volatility amplitude comparison
	* Macroeconomic stability differentiation
	* Growth-inflation correlation patterns
	* Structural stabilization trends

	The notebook emphasizes transparency in assumptions and methodological traceability throughout.

---

## Repository Structure

	```
	01-json-economic-analysis/
	│
	├── economic_risk_analysis.ipynb
	├── data/
	│   └── sample_api_response.json
	├── outputs/
	│   ├── cleaned_dataset.csv
	│   └── visualizations/
	└── requirements.txt
	```

---

## ▶️ How to Run

	1. Clone the repository:

	```
	git clone <repository-url>
	```

	2. Install dependencies:

	```
	pip install -r requirements.txt
	```

	3. Open the notebook:

	```
	jupyter notebook economic_risk_analysis.ipynb
	```

	4. Run cells sequentially from top to bottom.

---

## 🔎 Reproducibility & Documentation Standards

	This project prioritizes:

	* Explicit assumption documentation
	* Transparent data cleaning logic
	* Clear reasoning for transformation steps
	* Structured interpretation before business translation
	* Version-aware environment notes

	All analytical conclusions are derived from documented and reproducible steps.

---

## Limitations

	* Public data may contain reporting lags.
	* Macroeconomic indicators are subject to revision.
	* Correlation does not imply causation.
	* Analysis does not control for structural policy differences.

---

## Why This Project Matters

	This notebook demonstrates:

	* Comfort working with JSON-based public datasets
	* Structured technical documentation in notebooks
	* Analytical reasoning transparency
	* Clear communication of quantitative findings
	* Translation of macroeconomic data into actionable insights

	It reflects the intersection of data analysis and disciplined technical writing.

---

## Contact

	Opeyemi Sadiku
	LinkedIn: [Your LinkedIn URL]
	Email: [Your Email]

---
