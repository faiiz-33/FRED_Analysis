Exploratory Data Analysis (EDA)

Macroeconomic Trends
	•	Consumer Price Index (CPI) and house price index both exhibit strong long-run upward trends from 1988 to 2024, reflecting persistent price growth and asset appreciation in the U.S. economy.
	•	The house price index increased from approximately 60 in 1988 to over 325 by 2024, indicating substantial long-term growth with notable accelerations after 2000 and post-2020.

Inflation Dynamics
	•	Inflation (year-over-year CPI growth) remains relatively stable for most of the sample, with only one deflationary episode observed between 1988 and 2024.
	•	Inflation reached below −2% only once, following the 2008 global financial crisis, highlighting the rarity of sustained deflation in the U.S.
	•	Post-2020 inflation displays unusually high volatility, signaling a structural break driven by supply shocks and fiscal stimulus.

Interest Rates
	•	Policy interest rates range from near 0% to approximately 10% across the sample.
	•	The highest concentration of observations lies between 0–2%, reflecting extended periods of accommodative monetary policy.
	•	Interest rates drop sharply toward zero following major economic shocks, notably:
	•	2008 financial crisis
	•	2020 COVID-19 pandemic
	•	This behavior confirms the role of interest rates as a reactive policy instrument.

Labor Market Behavior
	•	The unemployment rate is most frequently observed around 5%, representing normal labor market conditions.
	•	Extreme unemployment values are rare and crisis-driven.
	•	During the COVID-19 pandemic, unemployment spiked to approximately 14%, the highest level observed in the entire 1988–2024 period, before recovering rapidly.

Housing Market Volatility
	•	House price inflation is significantly more volatile than CPI inflation.
	•	During the housing market collapse of 2009, house price inflation fell to approximately −12.7%, substantially deeper than CPI deflation.
	•	This highlights the housing market’s heightened sensitivity to financial stress and credit conditions.

Structural Breaks
	•	Two major structural breaks are evident:
	•	2008–2009: demand-driven financial collapse
	•	2020–2022: supply-driven pandemic shock
	•	Outside these periods, macroeconomic relationships appear relatively stable.

⸻

Modeling Insights

Inflation Model (24-Month Interest Rate Lag)

A linear regression was estimated to model year-over-year inflation as a function of unemployment and lagged monetary policy:

Coefficients (24-month lag):
	•	unemployment_rate: −0.147
	•	fed_funds_lag24: +0.176

Interpretation:
	•	A 1 percentage-point increase in unemployment is associated with a 0.15 percentage-point decrease in inflation, holding interest rates constant.
	•	A 1 percentage-point increase in interest rates 24 months earlier is associated with a 0.18 percentage-point increase in current inflation.
	•	The negative unemployment coefficient is consistent with a flattened Phillips Curve, indicating that labor market slack affects inflation gradually.
	•	The positive interest-rate coefficient reflects monetary policy reaction, as rates tend to be raised during periods of persistent inflationary pressure rather than causing inflation directly.

⸻

House Price Inflation Model (24-Month Interest Rate Lag)

A second regression modeled house price inflation using general inflation and lagged interest rates:

Coefficients (24-month lag):
	•	inflation_rate: +0.661
	•	interest_rate_lag24: −0.618

Interpretation:
	•	A 1 percentage-point increase in CPI inflation is associated with a 0.66 percentage-point increase in house price inflation, indicating strong inflation pass-through into housing markets.
	•	A 1 percentage-point increase in lagged interest rates is associated with a 0.62 percentage-point decrease in house price inflation, confirming the delayed cooling effect of tighter monetary policy.
	•	The relatively large inflation coefficient reflects both direct cost pressures and omitted demand-side factors, particularly during post-2020 housing market dynamics.

⸻

Key Takeaways
	•	Inflation dynamics are weakly linked to unemployment in the short run but strengthen over longer horizons.
	•	Monetary policy effects operate with long lags and are best interpreted as reactive rather than causal.
	•	Housing markets amplify macroeconomic shocks, responding strongly to both inflation and interest-rate changes.
	•	Linear regression provides meaningful structural and scenario-based insights, but cannot fully capture extreme regime shifts such as the 2020–2022 period.
