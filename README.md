# NETRA-Network_Threat_Radar_and_Analysis
NETRA is an advanced web vulnerability scanner built with Python and a modern React + Tailwind CSS frontend. It performs both quick and deep scans to detect critical security flaws based on the OWASP Top 10 vulnerabilities.
## 🔒 Features

- ✅ **Quick Scan**
  - Checks HTTPS usage
  - Analyzes secure cookie flags
  - Detects missing or weak security headers

- 🔍 **Deep Scan**
  - **SQL Injection** (Error-based & Time-based)
  - **Cross-Site Scripting (XSS)** – Reflected, Stored, and DOM-Based
  - **Open Redirect** vulnerability checks
  - Full website crawling with multithreaded scanning

- 📄 **PDF Report Generation**
  - Automatically generates a detailed security report
  - Summarizes vulnerabilities, affected URLs, and risk levels

- 🧩 **Modular Design**
  - Separate modules under `vuln_modules/` for easy extensibility

## 🛠 Tech Stack

| Component     | Technology            |
|---------------|------------------------|
| Frontend      | React + Tailwind CSS   |
| Backend       | Python (Flask)         |
| Database      | SQLite                 |
| Reporting     | ReportLab (PDF)        |
| Crawling      | BeautifulSoup, Requests|
| Concurrency   | ThreadPoolExecutor     |

## 🗂️ Project Structure
netra/
├── app.py # Main Flask backend
├── frontend/ # React + Tailwind frontend
├── vuln_modules/ # Modular vulnerability scanners
│ ├── sqli.py
│ ├── xss.py
│ ├── redirect.py
│ ├── headers.py
│ └── https_cookie.py
├── templates/ # HTML templates (for report or fallback UI)
├── static/ # CSS/JS assets (if needed)
└── README.md
