# CodeAlpha Web Scraping

A beginner-friendly Python web scraping project that collects book listing information from **Books to Scrape**.

## Project files

```text
CodeAlpha_Web_Scraping/
├── CodeAlpha_Web_Scraping.ipynb
├── CodeAlpha_Web_Scraping_Final.csv
└── README.md
```

## Target website

https://books.toscrape.com/

Books to Scrape is a public practice website intended for learning web scraping. Its prices and ratings are fictional.

## Data collected

| Column | Description |
|---|---|
| `title` | Full book title |
| `price_gbp` | Book price in GBP |
| `rating` | Rating converted to a number from 1 to 5 |
| `availability` | Stock availability text |
| `product_url` | Absolute URL of the book detail page |
| `category` | Reserved category field (blank in this listing-only version) |

## Tools and libraries

- Python
- Requests
- BeautifulSoup
- Pandas
- Jupyter Notebook

## How to run

1. Download or clone this repository.
2. Open a terminal in the project folder.
3. Install dependencies:

   ```bash
   pip install requests beautifulsoup4 pandas notebook
   ```

4. Start Jupyter:

   ```bash
   jupyter notebook
   ```

5. Open `CodeAlpha_Web_Scraping.ipynb`.
6. Run all cells from top to bottom.
7. The notebook scrapes the paginated catalogue, cleans the records, performs basic checks, and writes `CodeAlpha_Web_Scraping_Final.csv`.

## Output

The final CSV is generated in the same working directory as the notebook. The notebook includes an export validation step to confirm that the saved row count matches the DataFrame.

**Important:** The CSV included with this starter package is a header-only output template because the execution environment used to prepare these files did not have outbound internet access. Run the notebook on your computer with an internet connection to populate it with the live scraped records.

## Responsible scraping

- Use this project only with the designated practice website.
- Keep request delays in place.
- Do not bypass access controls, CAPTCHAs, or authentication.
- Check the target website's terms and policies before scraping any other website.
