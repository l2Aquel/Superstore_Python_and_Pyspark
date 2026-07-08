# Superstore_Python_and_Pyspark
This project presents a systematic data analysis of the Superstore dataset, 
designed to evaluate and contrast the syntax, performance, and operational logic of two industry-standard data processing tools: Pandas and PySpark.

## Project Overview
The core objective of this project was to answer 15 distinct analytical questions covering data cleaning, transformation, and business intelligence. By implementing the solution for every question in both Pandas and PySpark, I aimed to gain a deeper understanding of how local in-memory dataframes differ from distributed data processing frameworks.

## Dataset
- Source: Superstore Dataset
- Domain: Retail / E-commerce sales data.
- Key Attributes: Order Date, Ship Date, Sales, Quantity, Discount, Profit, Category, and Geographical information.

## Methodology & Objectives
The project is structured around 15 progressive-difficulty questions, including:
- Temporal Analysis: Parsing date strings to datetime objects and calculating shipping durations.
- Exploratory Data Analysis (EDA): Utilizing descriptive statistics to identify outliers and distributions.
- Aggregations: Performing complex group by operations to find total sales volumes, average profits, and regional performance metrics.
- Conditional Logic: Creating derived features (e.g., categorizing revenue into 'High', 'Medium', 'Low' tiers) using vectorized operations and conditional branching.

## Tooling Comparison
Pandas
- Use Case: Ideal for small-to-medium datasets (fitting in local RAM).
- Syntax Style: Imperative, highly expressive, and standard for rapid prototyping.
- Key Operations: astype(), groupby(), agg(), sort_values(), and standard Python list comprehensions.

PySpark
- Use Case: Designed for Big Data and large-scale parallel processing.
- Syntax Style: Declarative and lazy-evaluated, focusing on the execution plan.
- Key Operations: withColumn(), groupBy(), when().otherwise(), and native SQL-like expression handling.

## Key Learnings
- Syntactic Differences: While the logic remains the same, the API differences 
(e.g., Pandas' index-based approach vs. Spark's schema-based approach) 
highlight the trade-offs between flexibility and distributed scalability.
- Performance Considerations: Observed how PySpark handles data partitioning compared to the monolithic data frame approach of Pandas.
- Data Quality: Gained experience in handling standard data issues like date format inconsistencies and data type casting, ensuring consistency across both implementation environments.
