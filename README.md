# Content Aggregator
**Below is information on how my `ebay-dl.py` file scrapes product data from eBay and returns a JSON file with the information on that product.**

---

## JSON: Store Scraped Data in a JSON File
![Web Scraping Meme](https://github.com/keirkeenan/hw_03/blob/main/web_scraping.jpg)

By using python, you can scrape the html code of eBay's website to collect product data. The `ebay-dl.py` file will take a *product name* as input and return a JSON file with data from the first 10 pages of search results. The data scraped in this project includes: `name`, `price`, `status`, `freereturns`, and `items_sold`.  Try this yourself by downloading the `ebay-dl.py` file. 

The `ebay-dl.py` file does the following:
1. sets command line arguments
2. loops over the eBay webpages 
    1. builds the url
    2. downloads the html
    3. processes the html
    4. loops over the items in the page
3. writes the JSON to a file

In the terminal, run the following command with a search term of choice:
```
python ebay-dl.py 'search term'
```

For example, to search for `iphone charger` I put the following command in the terminal:
```
python ebay-dl.py 'iphone charger'
```
to produce the [iphone charger.json](https://github.com/keirkeenan/hw_03/blob/main/iphone%20charger.json) file.

To search for `iphone` I put:
```
python ebay-dl.py 'iphone'
```
to produce the [iphone.json](https://github.com/keirkeenan/hw_03/blob/main/iphone.json) file.

To search for `airpods` I put:
```
python ebay-dl.py 'airpods'
```
to produce the [airpods.json](https://github.com/keirkeenan/hw_03/blob/main/airpods.json) file.

---
