# Wikipedia Web Scraping — Largest US Companies (Table Extraction)

## Overview
This project demonstrates an end-to-end web scraping workflow by extracting a structured HTML table from Wikipedia using **Requests** and **BeautifulSoup**, transforming it into a **pandas DataFrame**, and exporting the results to **CSV** for downstream analysis.

Target page:
- Wikipedia: *List of largest companies in the United States by revenue*

Primary output:
- A clean CSV table containing the companies and related fields pulled from the Wikipedia table.

---

## Business / Analytics Goal
Wikipedia often contains valuable “semi-structured” datasets in HTML table format.  
The goal of this project is to build a **reproducible pipeline** that:

1. Fetches a web page reliably (with headers + timeout)
2. Locates the target HTML table
3. Extracts headers + row values
4. Stores the result into a structured dataset (`.csv`) for analysis

---

## Tech Stack
- Python
- requests
- beautifulsoup4
- pandas

---

## Repository Structure
```text
wikipedia-web-scraping/
├── README.md
├── Source/
│   └── Source_txt               # data source reference / notes (e.g., Wikipedia URL)
├── code/
│   └── Web_Scraping_Project.ipynb  # notebook: scraping + parsing + export
└── table_output/
    └── Companies.csv            # exported table (final output)
