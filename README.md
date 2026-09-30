# Python DA Assignment 2 – Data Visualization

## 📌 Project Overview

This project focuses on analyzing and visualizing taxi trip data using **Python, Pandas, Matplotlib, and Seaborn**.

The main objective is to clean the dataset, handle missing values, analyze taxi trip patterns, and create different visualizations to understand **fare, distance, payment methods, pickup locations, tips, and customer behavior**.

---

## 📂 Dataset

The project uses the built-in **Taxis dataset** available in the Seaborn library.

```python
import seaborn as sns

df = sns.load_dataset("taxis")
```

The dataset contains information such as:

- Pickup and drop-off timestamps
- Number of passengers
- Trip distance
- Fare
- Tip
- Tolls
- Total amount
- Payment method
- Pickup and drop-off zones
- Pickup and drop-off boroughs

---

## 🛠️ Technologies Used

- Python
- Google Colab
- Pandas
- Matplotlib
- Seaborn

---

## 🧹 Data Cleaning

The following data-cleaning operations were performed:

- Checked the dataset for missing values.
- Identified numerical and categorical columns containing missing data.
- Filled numerical missing values using an appropriate statistical method such as the **median**.
- Filled categorical missing values using the **mode**.
- Converted the `pickup` column into datetime format.
- Sorted pickup timestamps for time-based visualization.

---

## 📊 Matplotlib / Pandas Visualizations

### 1. Line Chart – Fare Over Time

A line chart was created using:

- **X-axis:** Pickup timestamp
- **Y-axis:** Fare

This visualization helps understand how taxi fares change over time.

### 2. Bar Chart – Total Fare by Pickup Borough

The data was grouped by `pickup_borough`, and the total fare for each borough was calculated.

This chart compares the total fare generated from different pickup boroughs.

### 3. Pie Chart – Payment Method Distribution

A pie chart was created using the count of trips for each payment method.

This visualization shows the proportion of trips paid using different payment methods such as **credit card and cash**.

### 4. Histogram – Trip Distance Distribution

A histogram was created to analyze the distribution of taxi trip distances.

The number of bins was customized to provide a clearer representation of the distance distribution.

### 5. Box Plot – Tips by Pickup Borough

A box plot was created to compare tip amounts across different pickup boroughs.

It helps identify:

- Median tip amounts
- Distribution of tips
- Variation between boroughs
- Potential outliers

---

## 📈 Seaborn Visualizations

### 6. Count Plot – Trips by Pickup Borough

A count plot was created to show the number of taxi trips originating from each pickup borough.

### 7. Scatter Plot – Distance vs Fare

A scatter plot was created using:

- **X-axis:** Distance
- **Y-axis:** Fare
- **Hue:** Pickup Borough

This visualization helps analyze the relationship between trip distance and taxi fare.

### 8. Correlation Heatmap

A correlation matrix was generated for:

- Distance
- Fare
- Tip
- Tolls
- Total

A Seaborn heatmap was used to visualize the strength of relationships between these numerical variables.

### 9. Pair Plot

A pair plot was created for:

- Distance
- Fare
- Tip
- Total

The data points were differentiated using `pickup_zone`.

This visualization helps explore pairwise relationships between important numerical variables.

### 10. Violin Plot – Fare by Payment Method

A violin plot was created using:

- **X-axis:** Payment Method
- **Y-axis:** Fare

This visualization helps compare the distribution and density of fares across different payment methods.

---

## 🔍 Key Insights

- Taxi fare generally increases as trip distance increases.
- Trip frequency varies across pickup boroughs.
- Payment methods can be compared based on their share of total trips.
- Tip amounts vary across different pickup boroughs.
- The correlation heatmap helps identify relationships between fare, distance, tip, tolls, and total amount.
- The pair plot provides a detailed view of relationships among major numerical variables.
- Violin plots make it easier to compare fare distributions across payment methods.

---

## 🎯 Project Objective

The objective of this assignment was to gain practical experience in:

- Data loading
- Data cleaning
- Missing-value handling
- Data manipulation using Pandas
- Data visualization using Matplotlib
- Data visualization using Seaborn
- Correlation analysis
- Understanding taxi trip patterns

---

## ✅ Conclusion

This project demonstrates the complete basic workflow of **data cleaning, exploratory data analysis, and data visualization** using Python.

By using Pandas, Matplotlib, and Seaborn, raw taxi trip data was transformed into meaningful visualizations that help identify patterns, distributions, relationships, and customer behavior.

The assignment provided practical experience in using Python visualization libraries for real-world data analysis.

---

## 👤 Author

**Subramaniyam R**

Aspiring Data Analyst
