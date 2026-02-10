# Web Scraping Practice Project

A beginner-friendly web scraping project using Python to extract book data from [Books to Scrape](https://books.toscrape.com/) - a safe practice website designed for learning web scraping.

## 📚 Project Overview

This is my practice project to learn web scraping fundamentals. I scraped data from all 50 pages of the Books to Scrape website, extracting information about 1000 books in total.

**What this project does:**

- Downloads 50 HTML pages using the `requests` library
- Parses HTML content with `BeautifulSoup`
- Extracts book titles, prices, and ratings
- Stores all data in a CSV file using `pandas`

## 🎯 What I Learned

Through building this project, I practiced:

- Making HTTP requests to retrieve web pages
- Handling errors with try-except blocks
- Parsing HTML using CSS selectors
- Extracting specific data from HTML elements
- Working with loops to process multiple pages
- Storing and exporting data to CSV files

## 🛠️ Technologies Used

- **Python 3.x**
- **requests** - for downloading web pages
- **BeautifulSoup4** - for parsing HTML
- **pandas** - for data manipulation and export
- **lxml** - HTML parser

## 📁 Project Structure

```
08_Scrapping/
│
├── 01_download_pages.ipynb      # Step 1: Download HTML pages from website
├── 02_parse_and_extract.ipynb   # Step 2: Parse HTML and extract book data
├── data.csv                     # Output file with extracted book data
├── requirements.txt             # Python package dependencies
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

## 📝 Sample Output

Here's what the data looks like:

| Book Title                  | Price | Rating |
| --------------------------- | ----- | ------ |
| A Light in the Attic        | 51.77 | Three  |
| Tipping the Velvet          | 53.74 | One    |
| Soumission                  | 50.10 | One    |
| Sharp Objects               | 47.82 | Four   |
| Sapiens: A Brief History... | 54.23 | Five   |

## ⚠️ Important Notes

- This project uses **Books to Scrape** (https://books.toscrape.com/), which is specifically designed for web scraping practice
- Always check `robots.txt` and respect website terms of service when scraping
- This is a **learning project** - not intended for commercial use
- The website doesn't require authentication or rate limiting

## 💡 Key Features

- ✅ Error handling for failed requests
- ✅ Processes all 50 pages automatically
- ✅ Clean, well-commented code
- ✅ Exports data in CSV format
- ✅ Structured in easy-to-follow notebooks

## 🎓 Skills Demonstrated

- **Web Scraping**: Using BeautifulSoup and requests
- **Data Extraction**: CSS selectors and HTML parsing
- **Error Handling**: Try-except blocks for robust code
- **Data Processing**: Working with pandas DataFrames
- **File I/O**: Reading/writing HTML and CSV files
- **Python Basics**: Loops, functions, and string manipulation

## 📈 Possible Future Enhancements

Some ideas to extend this project:

- [ ] Add data visualization (charts showing price distribution, rating analysis)
- [ ] Implement data cleaning (converting ratings to numbers, price to float)
- [ ] Add statistical analysis of the book data
- [ ] Create a SQLite database instead of CSV
- [ ] Build a simple dashboard with the data

## 🤝 About This Project

This is a personal learning project I created to practice web scraping and data extraction. I'm sharing it on GitHub to document my learning journey and help others who are also learning web scraping!

Feel free to fork this project and experiment with it. If you have suggestions for improvements, I'd love to hear them!

---

**Project Type:** Practice/Learning Project  
**Status:** Complete  
**Created:** As part of my Data Science learning journey

Made with 💻 while learning Python and web scraping!
