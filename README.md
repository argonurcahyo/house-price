# House Price Scraper

This project is a web scraping tool designed to gather and analyze house price data from online real estate platforms. Specifically, it is configured to scrape data from [Rumah123.com](https://www.rumah123.com) for regions in Indonesia.

## Features

- **Web Scraping**: Utilizes Python libraries like `requests` and `BeautifulSoup` to extract data.
- **Dynamic User-Agent Rotation**: Avoids IP bans by rotating through multiple user-agent strings.
- **Data Processing**: Processes and cleans the scraped data using `pandas`.
- **Region-Specific Scraping**: Allows for targeted data collection by specifying a region.

## Prerequisites

Before you begin, ensure you have the following installed:

- Python 3.7+
- `requests` library
- `beautifulsoup4` library
- `pandas` library

Install the required libraries using pip:

```bash
pip install requests beautifulsoup4 pandas
```

## How to Use

1. Clone this repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the project directory:
   ```bash
   cd house-price-scraper
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook house-price.ipynb
   ```
4. Modify the `region` variable in the notebook to target your desired location. Example:
   ```python
   region = 'badung'
   base_url = f"https://www.rumah123.com/jual/{region}/rumah/"
   ```
5. Run the notebook cells to scrape and process the data.

## Output

The scraped data will be saved in a structured format (e.g., CSV or DataFrame) for further analysis. You can customize the output format by modifying the code in the notebook.

## Important Notes

- **Respect Terms of Service**: Ensure that your usage complies with the terms of service of the website being scraped.
- **Rate Limiting**: To avoid being blocked, the scraper includes randomized delays between requests.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contributing

Contributions are welcome! Feel free to fork the repository and submit a pull request.

## Contact

For questions or feedback, please contact [Your Name or Contact Info].
