

````markdown
# 📚 Goodreads Book Scraper (100 Pages)

This project is a Python-based web scraper that collects data from Goodreads' public book list:  
**[Best Books Ever](https://www.goodreads.com/list/show/1.Best_Books_Ever)**.

The scraper uses `requests` and `BeautifulSoup` to extract information from the first 100 pages of the list and saves the data into a structured CSV file.

---

## 🔍 Features

- ✅ Scrapes book **titles**, **authors**, and **average rating info**
- ✅ Handles 100 pages automatically with polite delays
- ✅ Cleans and exports the data to `CSV`
- ✅ Extracts numeric ratings for analysis
- ✅ Ready for data analysis or integration into a data pipeline

---

## 📁 Output File

- `goodreads_best_books_100_pages.csv`  
  Contains clean data with columns:
  - `Title`
  - `Author`
  - `Rating Info`
  - (Optional: `Rating` as float, if you added rating extraction)

---

## 🚀 How to Run

1. Clone the repo or download the `.ipynb` notebook
2. Install dependencies:

```bash
pip install requests beautifulsoup4 pandas
````

3. Run the notebook cells or execute the scraping function in Python.

---

## 📊 Sample Usage

After scraping, you can analyze the data:

```python
# Top authors
df["Author"].value_counts().head(10)

# Filter books with high ratings
df[df["Rating"] >= 4.5]
```

---

## ⚠️ Notes

* This scraper uses a `time.sleep(2)` delay between pages to respect Goodreads' servers
* Goodreads may throttle or block excessive scraping. This version scrapes responsibly and avoids detection.
* Data is collected for **educational and portfolio** purposes only.

---

## 📌 Technologies Used

* Python
* Requests
* BeautifulSoup4
* Pandas
* Jupyter Notebook

---

## 📂 Project Structure

```
goodreads-scraper/
├── goodreads_scraper.ipynb
├── goodreads_best_books_100_pages.csv
├── README.md
```

---

## 🧠 Author

**Nisma Munawar**
Aspiring Python Developer | Data Enthusiast
GitHub: [@nimsa](https://github.com/nimsa) *(replace with your actual username)*

---

## 📄 License

This project is licensed under the MIT License.

```

