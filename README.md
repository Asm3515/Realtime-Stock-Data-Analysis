### Real-Time Stock Data Project

This project retrieves real-time stock data from Google Finance for three stocks (AAPL, META, TSLA) and stores the data in a CSV file. It also uploads the CSV file to an Amazon S3 bucket. The data includes various attributes such as stock price, market cap, volume, and more.

#### Installation

- Ensure you have Python installed (preferably Python 3.x).
- Install the required libraries using pip:

![Installation Image](https://github.com/Asm3515/Realtime-Stock-Data-Analysis/assets/75804184/7b5faf81-a565-455a-90b8-3dcf23d7485b)

#### Usage

1. Run the Flask app to start the API.
2. Access the API using the specified routes, e.g., `http://localhost:5000/stock_data/<stock_symbol>`.
3. Run the CSV creation script to continuously fetch and store data.




4. The script will create a CSV file for each fetch and upload it to the specified Amazon S3 bucket.

#### Configuration

- Update the `stock_urls` dictionary in `app.py` with the correct URLs for each stock.
- Modify the `bucket_name` variable in `csv_creator.py` to specify the Amazon S3 bucket to upload the CSV files.

#### Dependencies

- Flask: Web framework for the API.
- Requests: HTTP library for making requests to web servers.
- BeautifulSoup: Library for web scraping.
- Pyngrok: Library for creating secure tunnels to localhost.
- Pandas: Library for data manipulation and analysis.
- Boto3: AWS SDK for Python to interact with Amazon S3.

#### Disclaimer

This project is for educational purposes only. Always verify the data from multiple sources before making any financial decisions based on it.
