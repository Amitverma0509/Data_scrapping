# Amazon Data Scraper

## Project Overview

This project automates the process of scraping product data from Amazon's website using Selenium and BeautifulSoup. The collected data is stored in HTML files and later extracted into a CSV file for further analysis.

## Features

- **Web Scraping with Selenium:** Automatically browses Amazon's search results and saves the HTML content of each product listing.
- **Data Extraction with BeautifulSoup:** Parses the saved HTML files to extract product titles, prices, and links.
- **Data Storage:** Saves the extracted data into a CSV file for easy access and analysis.

## Requirements

- Python 3.x
- Selenium
- BeautifulSoup
- pandas
- Microsoft Edge WebDriver

## Setup and Usage

### 1. Install Required Python Packages
Install the necessary Python packages using pip:

```bash
pip install selenium beautifulsoup4 pandas
```

### 2. Set Up WebDriver
Download the Microsoft Edge WebDriver that matches your browser version

### 3. Run the Scripts

#### **Step 1: Collect HTML Data**
Run the `project.py` script to scrape data from Amazon and save it as HTML files:

```bash
python project.py
```

This script will store the HTML files in the `data` directory.

#### **Step 2: Extract Data from HTML**
Run the `collect.py` script to parse the HTML files and extract the product information into a CSV file:

```bash
python collect.py
```

The extracted data will be saved in a `data.csv` file in the project directory.

## Project Structure

```plaintext
├── project.py          # Script to scrape data from Amazon and save as HTML files
├── data/               # Directory to store HTML files
├── collect.py          # Script to extract data from HTML files and save to CSV
├── data.csv            # Output CSV file with extracted data
└── README.md           # Project documentation (this file)
```

## Notes

- The script currently scrapes data from the first 19 pages of Amazon search results. You can adjust the number of pages by modifying the `for` loop in `project.py`.
- **If you want to run the script before that delete the data folder and csv file**
