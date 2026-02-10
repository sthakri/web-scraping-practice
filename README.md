# Web Scraping Practice Project

A beginner-friendly web scraping project using Python to extract book data from [Books to Scrape](https://books.toscrape.com/) - a safe practice website designed for learning web scraping.

## 📚 Project Overview

This is my practice project to learn web scraping fundamentals. I scraped data from all 50 pages of the Books to Scrape website, extracting information about 1000 books in total.

**What this project does:**

- Downloads 50 HTML pages using the `requests` library
- Parses HTML content with `BeautifulSoup`
- Extracts book titles, prices, and ratings
- Stores all data in a CSV file using `pandas`

## 📁 Project Structure

```
08_Scrapping/
│
├── 01_download_pages.ipynb      # Step 1: Download HTML pages from website
├── 02_parse_and_extract.ipynb   # Step 2: Parse HTML and extract book data
├── data.csv                     # Output file with extracted book data           
├── htmls/                       # Folder containing downloaded HTML pages
│   ├── page1.html
│   ├── page2.html
│   └── ... (50 pages total)
├── .gitignore                   # Git ignore file
└── README.md                    # Project documentation
```

## 🚀 How to Run This Project

### Prerequisites

1. Make sure you have Python 3.x installed
2. Install required packages:

```bash
pip install -r requirements.txt
```

### Steps to Run

**Step 1: Download HTML Pages**

- Open `01_download_pages.ipynb` in Jupyter Notebook
- Run all cells to download 50 pages from Books to Scrape
- Pages will be saved in the `htmls/` folder

**Step 2: Extract and Save Data**

- Open `02_parse_and_extract.ipynb`
- Run all cells to parse HTML and extract book information
- Data from all 1000 books will be saved to `data.csv`

## 📊 Data Collected

I extracted data from **1000 books** across 50 pages. For each book, I collected:

- **Book Title** - Full title of the book
- **Price** - Price in GBP (£)
- **Rating** - Star rating (One to Five stars)

## ⚠️ Important Notes

- This project uses **Books to Scrape** (https://books.toscrape.com/), which is specifically designed for web scraping practice
- Always check `robots.txt` and respect website terms of service when scraping
- This is a **learning project** - not intended for commercial use
- The website doesn't require authentication or rate limiting

Made with 💻 while learning Python and web scraping!
