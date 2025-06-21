````markdown
# 📚 Goodreads Book Scraper (100 Pages)

A Python-based web scraper that collects book data from Goodreads' "Best Books Ever" list across 100 pages.  
It extracts **Title**, **Author**, and **Average Rating**, and saves the result to a clean CSV file.

---

## 🔍 Features

- Scrapes 100 pages from Goodreads
- Extracts title, author, and rating info
- Saves results to CSV
- Handles polite delays to avoid blocking
- Cleans rating info for analysis

---

## 📁 Output File

- `goodreads_best_books_100_pages.csv`

Columns:
- `Title`
- `Author`
- `Rating Info` (full string like "4.36 avg rating — 1,543,211 ratings")
- `Rating` *(optional: extracted float from the string)*

---

## 🚀 How to Run

1. Clone this repository or download the notebook
2. Install dependencies:

```bash
pip install requests beautifulsoup4 pandas
````

3. Run the `goodreads_scraper.ipynb` notebook

---

## 📊 Example Analysis

```python
# Top authors
df["Author"].value_counts().head(10)

# Books with high ratings
df[df["Rating"] >= 4.5]
```

---

## ⚠️ Notes

* Goodreads pages may take 5–10 seconds to load with parsing and delay
* `time.sleep(2)` is added to avoid getting blocked
* For educational and portfolio use only

---

## 🧠 Author

**Nisma Munawar**
GitHub: [@nisma](https://github.com/nisma)
(Replace with your actual GitHub username)

---

## 📄 License

MIT License

```
```

