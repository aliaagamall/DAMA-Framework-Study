# Data Quality

This file covers data quality concepts from the DAMA Framework, including definitions, dimensions, management process, and tools, based on my study of the DAMA-DMBOK.

## Introduction to Data Quality
- Data quality ensures data is fit for use in organizations.
- Goals: Prepare for CDMP exam, understand importance, roles, and responsibilities in data quality management.
- Outputs: Knowledge of dimensions, policies, procedures; how to achieve high-quality, reliable data.
- Part of DAMA wheel: Central to data management, surrounded by aspects like security and metadata.

## Definition of Data Quality
- Data quality: Measure if data meets standards and is ready for use (fit for purpose).
- Involves planning, execution, and activities to assess data against criteria.
- Importance: Enables accurate decisions, improves reputation, reduces risks (e.g., wrong medical diagnosis from poor data).
- Quality is a continuous process, not a one-time project; no data is 100% perfect.

## Dimensions of Data Quality
- Key metrics to measure quality (not all apply equally):
  - **Accuracy**: Data matches reality (e.g., valid phone number).
  - **Completeness**: No missing values (e.g., all fields filled).
  - **Consistency**: Uniform across systems (e.g., "Sudan" spelled the same way everywhere).
  - **Timeliness**: Up-to-date and available when needed (e.g., real-time sales data).
  - **Validity**: Conforms to rules (e.g., date not in future).
  - **Uniqueness**: No duplicates.
- Focus on critical data elements (CDEs) that impact business.

## Data Quality Management Process
- A cycle: Plan → Assess → Analyze → Improve → Monitor.
- **Plan**: Define goals, metrics, and tools; identify critical data.
- **Assess**: Use data profiling to detect issues (e.g., missing/duplicated values).
- **Analyze (Root Cause)**: Use "5 Whys" to find why issues occur (e.g., why missing data? → Poor training?).
- **Improve**: Clean data (e.g., remove duplicates, fill missing values with averages).
- **Monitor**: Track KPIs via dashboards (e.g., error rate <5%, resolution time 2 days).

## Common Data Quality Issues
- Missing values, duplicates, inaccuracies, outdated data.
- Causes: Lack of controls, system design flaws, input errors.
- Impacts: Wrong decisions, wasted resources, risks (e.g., legal issues from poor personal data quality).

## Tools and Practical Examples
- Tools: Power BI/Excel for profiling and cleaning; Informatica for advanced cleansing.
- Example in Power BI: Import CSV, profile columns (count empties/duplicates), clean (remove blanks, change types, replace values).
- Focus: Handle outliers (extreme values) using stats (e.g., box plots in Python).

## Challenges and Solutions
- Challenges: Continuous effort needed; not all issues solvable (e.g., can't fix inherently bad data).
- Solutions: Focus on critical data; use governance for oversight; training to prevent errors.
- Compliance: Align with laws like SDAIA (Saudi Arabia) for high-quality personal data.

## Applying Data Quality
- Start with awareness and goals; assess via profiling.
- Example Questions: "What dimension measures no duplicates?" (Uniqueness); "What process finds root causes?" (5 Whys).
- Real-world: In call centers, poor quality leads to duplicate tickets; clean data reduces calls by unifying sources.

## Data Quality Example

This file provides a practical example of data quality management using DAMA principles.

### Scenario
You’re a data quality manager at "Smart Electronics," an online retailer. Customer data (names, phones, addresses, sales) is poor:
- Duplicated customers (e.g., "Mohamed" and "Mohammed" as separate entries).
- Missing values (e.g., 20% incomplete phone numbers).
- Inconsistent formats (e.g., addresses vary across systems).

#### Issues
- Delayed deliveries from wrong addresses.
- Inaccurate sales reports (overstated due to duplicates).
- Compliance risks (poor personal data quality violates SDAIA/GDPR).

### Applying Data Quality Management
1. **Plan**: Goals: 95% accuracy in customer data. Focus on critical elements (phones, addresses).
2. **Assess**: Profile in Power BI: Import from Excel/CRM, find 15% duplicates, 20% missing phones.
3. **Analyze**: "5 Whys": Why missing? → Optional fields. Why? → Poor system design. Why? → No training.
4. **Improve**: Clean: Remove duplicates, fill missing with defaults, standardize formats (e.g., unify "Sudan").
5. **Monitor**: Dashboard KPIs: Error rate drops to 5%; monitor monthly.

### Results
- Accurate data: Deliveries on time (50% reduction in delays).
- Better decisions: Precise sales forecasts save costs.
- Improved reputation: Compliant, trusted data boosts customer satisfaction.

### Key Takeaways
- Continuous process: Focus on critical data; use tools like Power BI.
- Prevents risks: High quality enables reliable decisions.
