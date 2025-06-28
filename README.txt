Project: LinkedIn Job Scraper

This script scrapes LinkedIn job postings for roles like Frontend Developer, Backend Developer, and QN Writer, extracting:
1. Job Title
2. Company
3. Location
4. Job Type & Salary
5. Job Link
6. Parsed Qualifications

The data is saved in one Excel file with auto-adjusted column widths.

Features:
1. Automated scrolling & job link collection
2. Detail extraction using Selenium + BeautifulSoup
3. Regex-based qualification filtering
4. Output formatted using pandas + openpyxl

Limitations:
1. Not portable: May not run on all systems without adjusting ChromeDriver setup.
2. HTML structure sensitive: Breaks if LinkedIn updates its layout or class names.
3. Hardcoded login: Email/password are embedded for demo; not secure.
4. LinkedIn terms: Scraping may violate LinkedIn’s Terms of Service—use only for internal/demo purposes.
5. Bot detection: Excessive use may trigger account restrictions.

Requirements:
Install dependencies with:

pip install -r requirements.txt
requirements.txt

beautifulsoup4
selenium
requests
pandas
openpyxl
lxml

Output:
All job data is saved in a single Excel file:
linkedin_jobs.xlsx