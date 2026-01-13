🏥 Health Insurance Claims Fraud Analysis (Statistical Approach)

📌 Background

U.S. health insurance providers process millions of medical claims every year, making fraud detection a mission-critical function. Undetected fraudulent activity leads to:

	•	💸 Higher claim payouts and medical loss ratios
	•	⏱️ Slower claims adjudication and member dissatisfaction
	•	⚠️ Increased regulatory and compliance risk

Traditional fraud detection approaches—such as manual audits and static rule-based systems—are increasingly resource-intensive, slow, and difficult to scale.


🎯 Purpose of This Analysis

This project demonstrates how statistical hypothesis testing can support early fraud signal detection within a healthcare claims processing workflow. All analyses are implemented using Python and standard statistical libraries to reflect real-world insurer analytics environments.

Rather than replacing existing systems, these tests act as:

	•	🔍 Automated screening mechanisms
	•	🚨 Risk flags for deeper investigation
	•	🤖 Inputs for future machine learning models


🧪 Analytical Scope

The analysis explores claim cost and encounter-level behavior across healthcare providers and organizations, focusing on:

	•	Detecting unusually high average claim costs
	•	Comparing claim cost distributions across similar entities
	•	Evaluating whether cost differences are statistically meaningful


🔍 Part 1: Individual Provider Cost Anomaly


🧾 Scenario

Internal monitoring has raised concerns that a healthcare provider may be billing at a higher-than-expected rate relative to peers within the same specialty. 
This analysis helps distinguish between legitimate practice variation and potential overbilling behavior.

🧠 Objective

	•	Compare the provider’s average total claim cost against similar providers
	•	Determine whether observed differences are statistically significant
	•	Assess whether the provider should be flagged for additional review

🏢 Part 2: Claim Cost Comparison Between Organizations


🧾 Scenario

Two healthcare organizations with comparable characteristics are expected to exhibit similar total claim cost patterns. 
This step supports fairness, consistency, and early identification of cost anomalies.

🧠 Objective:

	•	Test whether differences in total claim costs are statistically significant
	•	Identify whether cost disparities fall outside normal variation

🏥 Part 3: Comparative Review Across Multiple Practices


🧾 Scenario

The insurer evaluates a group of private clinical practices to ensure consistent and reasonable claim cost behavior across similar entities. 
This approach helps insurers prioritize investigative resources efficiently.

🧠 Objective:

	•	Compare average claim costs across multiple practices simultaneously
	•	Identify outliers with significantly higher or lower costs
	•	Highlight entities that may require targeted review


📊 Part 4: Encounter-Type Proportion Analysis


🧾 Scenario

Differences in claim costs are not always fraudulent and may be driven by the mix of encounter types handled by providers (e.g., inpatient vs outpatient). This analysis reduces false positives by separating structural differences from abnormal billing patterns.

🧠 Objective:

	•	Compare the distribution of encounter classes across providers
	•	Determine whether differences in service mix explain observed cost variation


🧰 Tools & Methods:

	•	🐍 Python
	•	📦 pandas, numpy
	•	📐 scipy.stats
	•	Independent t-tests
	•	ANOVA
	•	Chi-square tests

✅ Value to U.S. Health Insurance Providers:

	•	🚨 Enables early identification of potential fraud
	•	📉 Reduces manual review workload
	•	⚖️ Supports explainable, audit-friendly decisions
	•	🤖 Provides a foundation for scalable ML fraud detection
