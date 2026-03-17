Workflow Identification
Last Updated: March 2026
Owner: Dipti Ghadge (dips.here@gmail.com)
Trigger Configuration
Type: Schedule by Zapier (Monthly)

Frequency: Every month
Day: 1st of the month
Time: 8:00 AM (timezone-aware)
Recurrence Pattern: Monthly (repeats indefinitely)
Actions
Action 1: Gmail Send Email
App: Gmail (GoogleMailV2CLIAPI)
Action Type: Create and send email

Recipients: dips.here@gmail.com
From Address: testingsel2025@gmail.com
From Name: Dipti Ghadge
Subject: Monthly Financial Report - {{trigger.timestamp | date('MMMM YYYY')}}
Dynamic: Updates monthly (e.g., "Monthly Financial Report - March 2026")
Body Type: HTML
Body: Professional HTML template with:
Executive summary section
Key metrics table (Net Profit Margin, Revenue Growth Rate, ROI, Cash Flow)
Detailed metric analysis
Trends and insights section
Strategic recommendations
Footer with generation timestamp
Data Sources Integrated
Source	Type	Purpose
Copy of global-semiconductor-industry-outlook-2025.pdf	Google Drive PDF	Industry context for financial analysis
Copy of mckinsey-technology-trends-outlook-2025.pdf	Google Drive PDF	Strategic trends and market insights
Copy of DI_Tech-trends-2026.pdf	Google Drive PDF	Technology trends for sector analysis
Agent Integration
Agent Name: NovaCart: Vector DB Agent
Purpose: Retrieve and analyze financial data including historical trends and performance metrics
Data Retrieved: 
Net Profit Margin
Revenue Growth Rate
ROI
Cash Flow
Historical trends and anomalies
Authentication Requirements

✅ Gmail Account: testingsel2025@gmail.com (connected)
✅ Google Drive: Access to PDF files (connected)


⏳ NovaCart Vector DB Agent: Must be configured and accessible
Email Template Structure
Monthly Financial Report
├── Report Date (dynamic)
├── Executive Summary
├── Key Financial Metrics Table
│   ├── Net Profit Margin
│   ├── Revenue Growth Rate
│   ├── ROI
│   └── Cash Flow
├── Detailed Metric Analysis
├── Trends and Insights
├── Recommendations
└── Generation Timestamp
