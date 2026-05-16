# Executive Summary: Marketing Campaign Analysis

### Project Goal
The primary objective of this project is to analyze customer demographic, financial, and behavioral data from a banking marketing campaign. By identifying the key drivers that lead to a successful "Subscription" (Target = Yes), this analysis provides data-driven strategies to optimize future marketing efforts and maximize conversion rates.

### Key Findings (Top 3)
1. **The Power of Previous Success:** Customers who converted in previous campaigns have a **64% conversion rate** in the current campaign, compared to the overall average of ~12%. Historical success is the strongest predictor of future behavior.
2. **Engagement is Critical:** There is a direct correlation between **Call Duration** and conversion. Successfully converted customers have significantly higher average call durations, indicating that engagement quality is a key driver of sales.
3. **High-Value Segments:** Customers without **housing loans** and those with **University degrees** represent the most receptive segments, showing nearly double the conversion rates of other demographic groups.

###  Final Result & Impact
* **Identified Class Imbalance:** Noted a significant imbalance (88.2% No vs 11.8% Yes), highlighting the need for targeted rather than mass-marketing approaches.
* **Strategic Optimization:** Provided actionable recommendations to shift focus toward high-propensity segments (previous successes and high-education groups), which can lead to a more efficient allocation of marketing budget and higher ROI.


## Data Dictionary

| Column Category | Feature Name | Description |
| :--- | :--- | :--- |
| **Identification** | `id` | Unique identifier for each customer record. |
| **Demographic** | `age` | Age of the customer. |
| | `gender` | Gender of the customer (Male/Female). |
| | `job` | Type of job (Management, Technician, Blue-collar, etc.). |
| | `marital` | Marital status (Married, Single, Divorced). |
| | `education` | Education level (Primary, Secondary, Tertiary, Unknown). |
| **Financial** | `balance` | Average yearly balance in Euros. |
| | `accountBalance` | Specific current balance in the customer's account. |
| | `default` | Has credit in default? (Yes/No). |
| | `housing` | Has a housing loan? (Yes/No). |
| | `loan` | Has a personal loan? (Yes/No). |
| **Campaign** | `contact` | Communication type (Cellular, Telephone, Unknown). |
| | `day` | Last contact day of the month. |
| | `month` | Last contact month of the year. |
| | `duration` | Last contact duration in seconds. |
| | `campaign` | Number of contacts performed during this current campaign. |
| | `numberOfContacts` | Total frequency of contacts made for this specific customer. |
| **History** | `pdays` | Days since the customer was last contacted (-1 = never contacted). |
| | `daySinceLastCampaign` | Specific interval of days since the previous campaign outreach. |
| | `previous` | Number of contacts performed before this campaign. |
| | `poutcome` | Outcome of the previous marketing campaign (Success/Failure). |
| **Target** | `target` | **Has the client subscribed? (Yes/No)** |
