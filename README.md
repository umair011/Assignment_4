# BCIT Course Data Scraper

## Project Overview

This project extracts information from BCIT course pages and converts unstructured HTML data into a structured dataset.

Using Python and BeautifulSoup, the notebook scrapes course pages and collects information such as:

- Course title
- Course overview
- Prerequisites
- Credits
- Learning outcomes

---

## Data Source

All data was collected from publicly available BCIT course pages:

https://www.bcit.ca/courses/

Example pages used in this project:

- https://www.bcit.ca/courses/applied-data-management-for-analytics-babi-4000/
- https://www.bcit.ca/courses/computers-and-the-law-blaw-3600/
- https://www.bcit.ca/courses/dqm-with-python-babi-4005/

---

## Ethical Scraping

This project uses a very small number of requests and includes delays between requests to avoid placing unnecessary load on the BCIT website.

The scraper:

- Uses a small list of manually selected course pages
- Adds a delay between requests
- Does not crawl or repeatedly access pages

---
 

---

## How to Run

1. Install required packages:
pip install -r requirements.txt

2. Open the notebook:
notebooks/scrape_bcit.ipynb

3. Run the notebook cells from top to bottom.

The notebook will scrape the course pages and save the extracted data into the **data/** folder.

---

## AI Use Statement

AI tools (ChatGPT Auto) were used to assist with structuring the scraping workflow, suggesting parsing strategies, and improving code readability.  
All code was reviewed, simplified, and tested to ensure it runs correctly and meets the requirements of the assignment.

---

## Output

The project produces three datasets to be used:

- **courses_cleaned.csv** – structured course information
- **prerequisite_map.csv** – course prerequisite relationships
- **learning_objectives.csv** – learning outcomes linked to courses