# Stock Data Scraper

This script automates the extraction of financial data from a stock analysis website using Selenium and Requests. It checks the availability of URLs, scrapes data, and saves the results into a CSV file.

## Features
- Reads a list of stock tickers from a CSV file.
- Checks if the target URLs are accessible before scraping.
- Extracts stock price, LPA (Earnings per Share), and VPA (Book Value per Share) using Selenium.
- Saves extracted data into `stock_data.csv`.
- Logs URL status into `url_status_log.csv`.

## Requirements
- Python 3.x
- Google Chrome
- ChromeDriver

## Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/GustavoVaradi/StockDataScraper.git
   cd StockDataScraper
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Ensure `acoes-listadas-b3.csv` exists with a column named `Ticker`.

## Usage
Run the script with:
```sh
python stock_scraper.py
```

## Output Files
- **stock_data.csv**: Contains extracted financial data.
- **url_status_log.csv**: Logs the status of URLs accessed.

## Configuration
You can modify:
- `OUTPUT_FILE`: Path for saving stock data.
- `LOG_FILE`: Path for logging URL statuses.
- `BASE_URL`: Base URL for stock data extraction.
- `XPATHS`: Adjust if the website structure changes.

## License
This project is licensed under the MIT License.

## Author
[Varadi Gustavo]

