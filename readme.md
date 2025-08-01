# Book Sales and Ratings - Exploratory Data Analysis (EDA)

## 📊 Overview

This project performs an Exploratory Data Analysis (EDA) on a dataset of books, aiming to understand the relationship between book ratings, sales performance, genres, authors, and publishers.

---

## 🎯 Objective

To uncover insights from a collection of books regarding:

* What genres sell the most?
* Does a high rating influence units sold?
* Which authors and publishers generate the most revenue?
* How does language impact the reach and popularity of a book?

---

## 🗂️ Dataset Summary

* **Number of unique books**: *(computed with `df["Book Name"].nunique()`)*
* **Date range**: Books published after 1900
* **Key columns**:

  * `Book Name`
  * `Book_average_rating`
  * `Book_ratings_count`
  * `units sold`
  * `sale price`
  * `genre`
  * `Author`
  * `Publisher`
  * `language_code`

---

## 🔍 Key Findings

### Genre & Ratings

* Genres vary in popularity and rating distribution.
* Top genres identified by count and visualized with bar chart.
* Some genres consistently achieve higher ratings or more ratings per book.

### Sales & Pricing

* No strong correlation between price and units sold.
* Books priced higher do not necessarily sell more copies.

### Language Analysis

* English dominates as the primary language.
* Other languages like Spanish and French are underrepresented.

### Author & Publisher Analysis

* High-revenue authors include J.K. Rowling and George R.R. Martin.
* Author rating vs. units sold shows a weak positive trend.
* Publisher revenue is concentrated among a few large names.

### Correlation Insights

* Positive correlation between `Book_average_rating` and `Book_ratings_count`.
* Books with higher average ratings tend to have higher total rating counts.

---

## 📈 Visualizations

The notebook includes several visualizations:

* Bar plots (Genre distribution, Top Authors)
* Boxplots (Rating per Genre, Author Rating vs. Sales)
* Scatter plots (Price vs. Sales, Rating vs. Ratings Count)
* Pie chart (Language Proportion)

---

## 💡 Insights & Recommendations

* Promote books in popular genres like Fantasy and Young Adult.
* Focus on author brand-building to increase visibility and sales.
* Price optimization should be done carefully, since pricing alone doesn’t drive volume.
* Explore publishing strategies in underrepresented languages for niche markets.

---

## ⚠️ Limitations

* Time-based trends could not be analyzed due to lack of date granularity.
* Some columns require cleaning (e.g. whitespace in column names).
* No textual reviews available for sentiment analysis.

---

## 🚀 Future Work

* Incorporate publication date/time for trend analysis.
* Add review texts to enable NLP-based sentiment analysis.
* Build predictive models for sales based on ratings, genres, and other metadata.

---

## 📁 Repository Structure

```
📦eda-books-data
 ┣ 📜EDA_Books_Data.ipynb
 ┣ 📜README.md
 ┣ 📁images/
 ┃ ┗ 📜(visual outputs here)
 ┗ 📁data/
    ┗ 📜books_data.csv
```

---

## 🙌 Author

Created by **Rifqi Setiawan**

Feel free to fork, clone, and modify for your own analysis. Contributions and feedback are welcome!

---

## 📎 License

This project is licensed under the MIT License.
