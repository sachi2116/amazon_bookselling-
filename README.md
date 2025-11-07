# amazon_bookselling-
Amazon best selling books 

## Project overview

This project analyzes Amazon book sales to understand which books and categories perform best. The dashboard highlights key metrics like sales, ratings, reviews, and price trends to help improve marketing and sales strategies. Insights support better decision-making on pricing, promotions, and inventory planning.

## Data description 

•	Book Title – Name of the book on Amazon

•	Author – Name of the writer

•	Category / Genre – Type of book (subject/theme)

•	Price – Current selling price

•	Discount % – Percentage of discount offered

•	Rating – Average customer rating (out of 5)

•	Reviews Count – Number of reviews received

•	Sales – Units sold or sales performance

•	Publication Year (optional) – Year the book was released

•	ISBN (optional) – Unique book identification number


## Business objective 

•	Improve book sales performance on Amazon

•	Identify top-selling books and categories

•	Understand customer preferences using ratings and reviews

•	Optimize pricing and discounts for higher revenue

•	Support better marketing and stock decisions

## Tools and Techniques  

Microsoft Power BI

•	Data Cleaning & Transformation:

•	Used Power Query to remove duplicate/blank book entries.

•	Standardized category names and corrected spelling mistakes.

•	Converted data types for Price, Rating, and Reviews.

•	Handled missing values in Ratings/Reviews by replacing or removing.

•	Created new calculated fields like Final Price after Discount (if applicable).



DAX Measures Created:

•	Total Sales = SUM('Books'[Sales])

•	Total Revenue = SUMX('Books', 'Books'[Price] * 'Books'[Sales])

•	Average Rating = AVERAGE('Books'[Rating])

•	Total Reviews = SUM('Books'[Reviews])

•	Top Category = CALCULATE(MAX('Books'[Category]), …) (if used)


Visuals Used:

•	Donut Chart: Sales distribution by category.

•	Bar Chart: Top-selling books / authors comparison.

•	Line Chart: Monthly or trend analysis of revenue (if date available).

•	Card Visuals: Total Sales, Total Revenue, Avg Rating, Total Reviews.

•	Scatter Chart: Rating vs Sales performance (optional).

•	Slicers/Filters: Category, Rating, Price, Author.

## Deliverables

•	Cleaned and well-structured Amazon book sales dataset

•	Power BI data model with accurate relationships and measures

•	Interactive dashboard with KPIs and visual insights

•	Category-wise and rating-wise sales analysis

•	Detailed charts showing best-performing books and authors

•	Actionable insights for improving book sales strategy

•	Project documentation including overview, objectives & conclusion

## Key insights 

•	Fiction and Educational categories generate the highest sales.

•	Books with higher ratings show better sales performance.

•	Low-priced books attract more customers and get more reviews.

•	A few top authors contribute a major share of total revenue.

•	Books with more discount offers show increased sales.

•	Some categories have good ratings but low sales, indicating lack of promotion.

•	Customer interest is strongly influenced by reviews and visibility.



## Future Enhancements 

•	Add time-based data to track monthly/annual sales trends

•	Include customer demographics for deeper analysis

•	Compare book performance across different platforms (Flipkart, Kindle etc.)

•	Use forecasting in Power BI to predict future sales

•	Add sentiment analysis on reviews for quality improvement

•	Automate data refresh for live performance tracking

•	Expand dataset with publisher and stock details for better planning

