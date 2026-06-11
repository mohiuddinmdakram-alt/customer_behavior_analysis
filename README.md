📊 Customer Shopping Behavior AnalysisAn end-to-end data analytics project analyzing 3,900 e-commerce transactions across 18 customer attributes. This project demonstrates a complete data workflow: cleaning and preparing raw data using Python, running business-focused exploratory analysis in PostgreSQL (SQL), and building an interactive dashboard in Power BI to drive marketing and retention strategies. 

<img width="1427" height="694" alt="image" src="https://github.com/user-attachments/assets/41b373e4-94c6-4c87-8897-5efd29214411" />

 🛠️ Project Workflow
 
 🐍 Data Preparation & Cleaning (Python)
  In this phase, I handled data loading, data quality checks, and feature engineering using the pandas library: 
Missing Data Handling: Identified 37 missing values in the Review Rating column and imputed them using the median rating of each specific product category to keep the data balanced. 

Feature Engineering: Grouped customer ages into clear categories (Young Adult, Adult, Middle-aged, and Senior) to make demographic analysis simpler.  

Database Integration: Cleaned and structured the final data table, then used Python to connect directly to PostgreSQL and load the dataset for deep SQL querying.  

2. 🗄️ Exploratory Data Analysis (PostgreSQL)
  I wrote 10 targeted SQL queries to extract insights on key business metrics. Some major findings include:
Revenue by Gender: Found that Male customers generated significantly more revenue ($157,890) than Female customers ($75,191). 
 
 Subscription Behavior: Analyzed the performance of the 1,053 subscribers vs. 2,847 non-subscribers. While non-subscribers make up 73% of the audience, the 27% subscriber base provides a highly steady and predictable revenue stream ($62,645).  

Demographic Performance: Calculated total revenue by age groups, revealing that the Young Adult cohort is the top financial contributor with $62,143 in sales. 

3. 📉  Data Visualization (Power BI)
   Finally, I connected the PostgreSQL database to Power BI to build an interactive executive dashboard for tracking retail performance metrics:  Core KPIs tracked: Easily monitors total customer volume (3.9K), Average Purchase Amount ($59.76), and Average Review Rating (3.75).
     Interactivity: Built-in dynamic filters (slicers) allowing users to filter all charts instantly by Subscription Status, Gender, Product Category, and Shipping Type.  Visual Highlights: Side-by-side bar charts clearly displaying that the Clothing category drives the highest sales volume and revenue compared to Accessories, Footwear, and Outerwear
