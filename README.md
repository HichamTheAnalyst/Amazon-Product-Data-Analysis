# 📦 Amazon Product Data Analysis

**Project Overview**  
This project explores a dataset of Amazon products to analyze product pricing, ratings, discount percentages, and user reviews. The goal is to derive meaningful business insights through exploratory data analysis (EDA) and visualization techniques.

---

## 📂 Dataset

The dataset (`amazon.csv`) includes 1465 entries and 16 columns:

- `product_id`, `product_name`, `category`
- `discounted_price`, `actual_price`, `discount_percentage`
- `rating`, `rating_count`
- `about_product`
- `user_id`, `user_name`
- `review_id`, `review_title`, `review_content`
- `img_link`, `product_link`

---

## 🛠️ Tools and Libraries Used

- **Python 3** (ipykernel)
- **Pandas** — Data manipulation
- **NumPy** — Numerical operations
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical data visualization

---

## 🔥 Steps Performed

1. **Data Loading**  
   Loaded the Amazon product data into a Pandas DataFrame.

2. **Data Preprocessing**
   - Removed special characters (₹, spaces, commas) from price columns.
   - Converted price columns to numerical types.
   - Handled missing values using mean or default values.
   - Cleaned and formatted the dataset for analysis.

3. **Exploratory Data Analysis (EDA)**
   - Studied distribution of discounted and actual prices.
   - Analyzed ratings vs. product prices.
   - Explored category-wise discounts and rating averages.
   - Identified top-selling and highly rated products.
   - Visualized customer review trends.

4. **Visualizations**
   - **Scatter plot** of Price vs Rating.
   - **Histograms** of price distributions.
   - **Bar charts** of top product categories.
   - **Pie charts** for category share.
   - **WordCloud** of customer review content (optional).

---

## 📊 Key Insights

- Significant discounts are common across multiple categories, especially electronics.
- Higher product prices don't always correlate with better ratings.
- Certain products with lower prices still maintain strong ratings and high review counts.
- A few users contribute a large number of product reviews.

---

## 📈 Example Visualization

### Price vs Rating

```python
plt.figure(figsize=(8,5))
sns.scatterplot(x='actual_price', y='rating', data=df)
plt.title('Price vs Rating')
plt.show()
```

---

## 🚀 Future Work

- Build a recommendation system based on product reviews and ratings.
- Predict rating counts or sales using regression models.
- Analyze seasonal trends in discounts and prices.
