# 🛍️ Tokopedia Product Web Scraper

This project is a **Python-based web scraping tool** that extracts product information such as **title**, **price**, and **date** from a Tokopedia product page.  
It uses the **BeautifulSoup** and **Requests** libraries to fetch and parse HTML content from the website.

---

## 📌 Project Overview

This project demonstrates how to:

- Connect to a Tokopedia product URL using the `requests` library.
- Extract specific HTML elements (product name and price) using `BeautifulSoup`.
- Store the collected data into a **CSV file**.
- Automate daily scraping with a time delay using the `time` library.
- (Optional) Send an **email notification** when the price drops below a certain threshold.

The project can serve as a starting point for building e-commerce monitoring or price-tracking applications.

---

## 🧩 Tech Stack

- **Python 3**
- **BeautifulSoup4**
- **Requests**
- **CSV**
- **Pandas**
- **smtplib (for email notification)**

---

## ⚙️ Installation

### 1. Clone this repository
```bash
git clone https://github.com/yourusername/python-tokopedia-product-web-scraper.git
cd python-tokopedia-product-web-scraper
```

### 2. Install the required libraries
```bash
pip install beautifulsoup4 requests pandas
```

### 3. Open the Notebook

Open the Jupyter Notebook or Python script file to run the scraping process.

---

# 🧠 How It Works
* **Step 1 — Import Libraries**

  Import all required Python libraries for scraping, time handling, and file writing.

* **Step 2 — Connect to the Website**

  Use the Requests library to send an HTTP request to the Tokopedia product page using proper headers.

* **Step 3 — Parse the HTML Content**

  Feed the page content into BeautifulSoup to structure and extract HTML tags.

* **Step 4 — Extract Product Information**

  Find and extract:

  * Product Title → `<h1>` tag with `data-testid="lblPDPDetailProductName"`

  * Product Price → `<div>` tag with `data-testid="lblPDPDetailProductPrice"`

* **Step 5 — Save Data to CSV**

  Store the extracted title, price, and current date in a `.csv file`.

* **Step 6 — Automate the Scraping**

  Run the scraping function every 24 hours (`86400 seconds`) to check for updated prices.

* **Step 7 — Optional: Send Email Notification**

  Send yourself an alert email when the product price drops below a chosen threshold.

---

# 🧰 Files in This Repository

| File                                  | Description                                        |
| ------------------------------------- | -------------------------------------------------- |
| `Tokopedia Web Scraper Project.ipynb` | Main notebook containing all code and explanations |
| `TokopediaWebScraperDataset.csv`      | Generated dataset file containing scraped data     |
| `README.md`                           | Documentation file                                 |

---


