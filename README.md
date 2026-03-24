# AI-Powered MSFT Daily Stock Report Automation

An n8n workflow that automatically fetches real-time Microsoft (MSFT) 
stock data, generates a professional analyst report using OpenAI, and 
delivers it to stakeholders via Gmail every morning at 9am.

## Business Problem
Financial and operations teams spend significant time manually pulling 
stock data, interpreting trends, and writing stakeholder updates. This 
workflow eliminates that manual effort entirely — saving an estimated 
30-45 minutes of analyst time per day.

## Workflow Architecture
Schedule Trigger (9am daily)
→ HTTP Request (Alpha Vantage API — live MSFT stock data)
→ OpenAI GPT-4o-mini (generates professional analyst narrative)
→ Gmail (delivers report to stakeholder inbox)

## Tools & Technologies
- n8n (workflow automation)
- Alpha Vantage API (real-time financial data)
- OpenAI GPT-4o-mini (AI narrative generation)
- Gmail API (automated email delivery)

## Sample Report Output
The workflow generates a structured report including:
- Latest closing price vs previous 3 days
- Volume analysis and anomaly detection
- Trend summary (bullish/bearish/sideways)
- Stakeholder recommendation

## BA Deliverables
This project includes standard Business Analyst documentation:
- Workflow process flow (as-is → to-be)
- Business requirements: automate daily financial reporting
- Stakeholder: Finance/Investment teams
- ROI: ~30 min/day analyst time saved = 130+ hours/year

## How to Run
1. Import workflow.json into your n8n instance
2. Add credentials: Alpha Vantage API key, OpenAI API key, Gmail OAuth
3. Update the recipient email in the Gmail node
4. Activate the workflow

## Author
Tareesh Muluguru — Business Analyst
[LinkedIn](https://linkedin.com/in/your-profile) | 
[Email](mailto:tmuluguru@gmail.com)
