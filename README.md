FRED Macroeconomic Analysis

Project Overview

This project analyzes long-term U.S. macroeconomic relationships using FRED (Federal Reserve Economic Data), focusing on:  
	•	Inflation  
	•	Unemployment  
	•	Interest rates  
	•	Housing prices  

The analysis combines exploratory data analysis (EDA), linear regression models, and scenario analysis to extract structural insights rather than short-term forecasts.  

⸻⸻⸻⸻⸻⸻

Repository Structure   

FRED-project    

.
├── data  
│   ├── raw  
│   │   ├── Source:  
│   │   │   └── https://www.stlouisfed.org/research/economists/mccracken/fred-databases  
│   │   └── FRED-MD_YYYYmMM.csv  
│   └── clean  
│       └── fred_clean.csv  
│  
├── python  
│   ├── FRED_analysis.ipynb  
│   └── README.md       # Technical insights from Python analysis  
│  
├── Executive_Insights.md  
└── README.md            # (this file)  
 

⸻⸻⸻⸻⸻⸻

Data Source  
	•	Primary source: FRED-MD (Federal Reserve Bank of St. Louis)  
	•	Coverage: 1988–2024 (aligned to housing price availability)  
	•	Frequency: Monthly  

All data is publicly available and downloaded directly from the official FRED repository.  

⸻

Methods  

Exploratory Data Analysis (EDA)  
	•	Trend analysis of CPI, unemployment, interest rates, and housing prices  
	•	Distribution analysis and correlation checks  
	•	Identification of structural breaks (2008, 2020)  

Linear Regression Models  
	•	Inflation modeled as a function of unemployment and lagged interest rates  
	•	House price inflation modeled using inflation and lagged interest rates  
	•	Lag structure (12–24 months) used to reflect delayed policy transmission  

Scenario Analysis  
	•	“What-if” analysis under alternative macroeconomic conditions  
	•	Focus on interpretability rather than point prediction  

⸻

How to Run the Code  

Requirements   
	•	Python 3.9+  
	•	Libraries:  

pandas  
numpy  
matplotlib  
seaborn  
scikit-learn  


open jupyter notebook python/FRED_analysis.ipynb  


	.	Run cells top-to-bottom to:  
	•	Load and clean data
	•	Perform EDA
	•	Train regression models
	•	Generate scenario analysis

⸻

Key Outputs  
	•	Cleaned macroeconomic dataset  
	•	Regression coefficients with economic interpretation  
	•	Scenario tables for inflation and housing outcomes  
	•	Diagnostic plots and residual analysis  

⸻

Notes  
	•	This project emphasizes economic intuition and interpretability  
	•	Results are not intended as short-term forecasts  
	•	Power BI visuals are optional and used only for high-level storytelling  

⸻

Author  

Faiz K. Alharthi
