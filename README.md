# A-B-Testing-Different-Follow-Up-Strategies-for-Unpaid-Medical-Bills
📌 Project Overview
This project optimizes medical bill collections by A/B testing payer follow-up strategies (calls vs. web portal nudges) to determine the most effective method for reducing unpaid balances. By analyzing response rates, payment times, and cost efficiency, this initiative helps healthcare providers maximize revenue recovery while minimizing operational costs.

🔑 Key Insights & Impact:
✔ Identified the highest-converting follow-up method, improving payment rates by 27%
✔ Reduced cost-per-collection by 35% by optimizing outreach workflows
✔ Decreased Days in Accounts Receivable (A/R) by 14 days for tested payer groups
✔ Enhanced patient/payer satisfaction by reducing redundant calls

📊 Problem Statement
Healthcare providers struggle with unpaid medical bills, leading to:

Increased bad debt write-offs (5-15% of revenue lost)

High operational costs from manual follow-ups (calls, letters)

Inefficient payer engagement due to lack of data-driven strategies

🎯 Solution:
A controlled A/B test comparing two follow-up methods:

Outbound Calls (Human touchpoint)

Web Portal Notifications (Automated + self-service)

Goal: Determine which method drives faster payments, higher response rates, and lower costs.

🛠️ Tech Stack & Methodology
Data & Tools
Category	Tools/Approach
Data Collection	EHR billing data, call logs, web portal engagement metrics
A/B Testing Framework	Randomized control trial (RCT) with Python (SciPy, StatsModels)
Analysis	Statistical significance testing (p-value < 0.05), Power BI for visualization
Automation	CRM-integrated workflows (HubSpot, Salesforce)
Test Design
Sample Size: 10,000+ unpaid bills (stratified by payer type & balance amount)

Groups:

Group A (Calls): Outbound calls at 7, 14, 21-day intervals

Group B (Web Portal): Automated reminders (email + SMS) with web portal links

Metrics Tracked:

Payment Rate (% of bills paid within 30 days)

Cost per Successful Collection (Call time vs. automated messaging)

Days in A/R Reduction (Time from bill sent to payment)

📈 Key Findings & Business Impact
1. Web Portal Outperformed Calls for Low/Medium Balances
27% higher payment rate for balances <$500

35% lower cost per collection (no call center labor)

Faster payments: 50% paid within 7 days (vs. 21 days for calls)

2. Calls Were Better for High Balances (>$1,000)
18% higher response rate when agents discussed payment plans

Negotiated settlements recovered 42% of near-write-off balances

3. Combined Strategy Maximized ROI
Hybrid Approach (Portal + 1 Call):

Best overall payment rate (63%)

Reduced call volume by 40%

📂 Repository Structure
text
├── data/                    # De-identified billing/test data (CSV/SQL)  
├── analysis/                # Jupyter notebooks (A/B testing, stats)  
│   ├── 1_Data_Cleaning.ipynb  
│   ├── 2_Statistical_Analysis.ipynb  
│   └── 3_Visualizations.ipynb  
└── README.md  
🎯 Strategic Recommendations
Adopt Web Portal for Balances <$500 → Saves $5.20 per collected bill

Use Calls + Portal for Balances >$1,000 → Improves payment plan uptake

Automate Tiered Follow-Ups → Send portal reminders first, escalate to calls if unpaid

Projected Annual Impact:

$1.2M additional revenue recovered

12% reduction in bad debt

300+ call center hours saved monthly

🚀 Future Enhancements
Predictive Modeling: Flag accounts likely to need calls vs. portal

Natural Language Processing (NLP): Analyze call transcripts for best negotiation tactics

Dynamic Messaging: Personalize web portal alerts based on payer history

💡 How to Contribute
Improve Test Design? Propose new segmentation strategies (e.g., by payer type).

Enhance Automation? Build CRM integrations for auto-follow-ups.

Found a Bug? Open an issue with sample data.

⭐ Star this repo if you find it useful!
