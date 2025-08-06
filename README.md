# 📩 Phishing Email Analysis

phishing-analysis, cybersecurity, email-security.

## Overview
This project analyzes phishing emails to detect malicious patterns, spoofed senders, and suspicious links.  
It is designed for cybersecurity research and training purposes.

## Objectives
- Parse and investigate email headers.
- Identify phishing tactics and patterns.
- Detect malicious links and attachments in a safe environment.
- Present statistical trends and visualizations.

## Tools & Technologies
- Python 3.x
- Pandas, Matplotlib
- Email Parser (`email` library)
- WHOIS lookup
- Thunderbird
- URLScan / VirusTotal API

## Project Workflow
1. **Data Collection** – Gather sanitized phishing samples in `.eml` format.
2. **Header Analysis** – Extract sender IP, SPF/DKIM/DMARC results.
3. **Link Analysis** – Extract and check URLs against security APIs.
4. **Attachment Analysis** – Identify potentially malicious files.
5. **Visualization** – Create charts for attack trends.

## Results (Example)
- 45% used brand impersonation.
- 30% from newly registered domains (<3 months old).
- Top lure subjects: "Password Reset", "Invoice", "Account Suspension".

## How to Run
```bash
# Install dependencies
pip install -r requirements.txt

# Run analysis
python analyze_emails.py
