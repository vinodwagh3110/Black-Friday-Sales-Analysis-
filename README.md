# Black Friday Sales Analysis

Hi! This is one more practice project I made to learn data analysis with Python. In this project, I analyzed Black Friday sales data to understand customer buying behaviour - like who buys more, which age group spends more, and from which city.

## What is this project about?

I took a Black Friday sales dataset (csv file) which has details of customers and their purchases, and did some analysis on it like:

- Checked the data for missing values and removed columns that had too many nulls
- Analyzed how many male and female customers are there and who spends more
- Checked which age group buys the most products
- Found which product is mostly bought by each age group
- Compared total purchase amount according to age
- Analyzed marital status of customers and its effect on shopping
- Compared genders with marital status using countplot
- Analyzed city category (A, B, C) - which city has more customers and which city spends more
- Used pie charts, bar charts and countplots to show everything visually

## Dataset used

File name: `BlackFriday.csv`

Some important columns in this dataset:

- **User_ID** – unique id of the customer
- **Product_ID** – unique id of the product
- **Gender** – Male or Female
- **Age** – age group of customer (like 0-17, 18-25, etc.)
- **Occupation** – occupation code of customer
- **City_Category** – city type (A, B, C)
- **Stay_In_Current_City_Years** – since how many years customer is living in that city
- **Marital_Status** – married(1) or unmarried(0)
- **Product_Category_1/2/3** – category of product bought
- **Purchase** – amount spent by customer

(Make sure this csv file is in the same folder as the notebook, otherwise it will give an error)

## Libraries used

I used these Python libraries:

```
pandas
numpy
matplotlib
seaborn
```

You can install them like this:

```bash
pip install pandas numpy matplotlib seaborn
```

## How to run

1. Keep the `BlackFriday.csv` file in the same folder as the notebook.
2. Open `Black_friday_sales_analysis.ipynb` in Jupyter Notebook.
3. Run all the cells one by one from top to bottom.
4. You will see different graphs (pie charts, bar charts, countplots) showing the analysis.

## What you will get after running

- Gender wise sales analysis (count and purchase amount)
- Age wise sales analysis (count, most bought product per age, purchase amount)
- Marital status wise analysis
- City category wise analysis (count and purchase amount)
- Multiple comparison graphs like Age vs Gender, Gender vs Marital Status, City vs Age etc.

## Things to keep in mind

- I removed `Product_Category_2` and `Product_Category_3` columns because they had a lot of missing values.
- Some graphs use `groupby()` + `plot()` and some use `seaborn countplot` - both give similar kind of insight, I used both just to practice different methods.

## What I learned from this project

- How to handle missing values in a dataset
- How to use groupby() to find useful insights
- How to make pie charts, bar charts and countplots
- How to compare two columns together using hue in seaborn
- How to read data and find patterns in customer behaviour

This is one of my beginner-level practice projects to learn data analysis. Feel free to suggest improvements!
