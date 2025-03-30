## **Project Overview**
This project aims to analyze vehicle sales data to uncover key market trends, customer behavior, and product performance over time. The dataset includes various transaction details for a wide range of vehicles, such as make, model, year, transmission type, body type, condition, mileage, and more. The goal is to understand how these features impact pricing, sales trends, and market fluctuations.

### **Dataset and Data Preparation**
The "Vehicle Sales and Market Trends Dataset" includes information on sales transactions for a variety of vehicles, covering:

- **Vehicle Details**: Make, model, trim, body type, year of manufacture, condition rating, odometer reading.
- **Transaction Information**: Selling prices, sale dates, and payment methods.
- **Market Trends**: Manheim Market Report (MMR) values, which help assess the market value of each vehicle.
  
Before analysis, data cleaning and pre-validation were performed to ensure data integrity. A major challenge was the presence of 10,301 missing values in the "make" column, which were addressed by using the **NHTSA API** to decode the VINs and fill in the missing vehicle details. 

- **Dataset**: [Vehicle Sales and Market Trends Dataset on Kaggle](https://www.kaggle.com/datasets/syedanwarafridi/vehicle-sales-data)
- **NHTSA API**: [Vehicle Information API (NHTSA)](https://vpic.nhtsa.dot.gov/api)

### **Key Metrics Calculated**
- **Selling Price vs. MMR**: Comparison of the selling price with the estimated market price (MMR) to identify trends and price discrepancies.
- **Mileage and Price**: Analysis of how mileage affects vehicle prices.
- **Price Trends**: Examination of price trends based on year of manufacture and market shifts.
- **Color and Condition**: Impact of exterior and interior colors and vehicle condition on selling prices.
- **Brand Popularity**: Identification of the most popular car brands based on sales volume in different states.
  
### **Technologies Used**
- **Python**: Data manipulation, analysis, and integration with the NHTSA API.
- **Power BI**: Visualization of trends and patterns.
- **SQL**: Data extraction and aggregation.
- **Libraries**: Pandas, Matplotlib, Seaborn, Scipy for analysis and visualization.
- **NHTSA API**: To decode VINs and fill in missing make and model values.

### **Key Insights**
1. **MMR and Selling Price**: Strong positive correlation (0.98) between MMR and selling price. Higher mileage negatively affects the price.
2. **Price Trends**: Prices increase significantly after 2000, especially post-2005, suggesting improved vehicle features and demand.
3. **Color Trends**: Uncommon colors like "other," black, and brown have higher average prices, while bright colors like yellow and turquoise are less expensive.
4. **Brand Popularity**: Ford dominates sales, especially in states like Texas, California, and Florida. Sedans are the most common body type.
5. **Price vs. MMR**: The selling price is significantly lower than the MMR, with an average difference of $144.86.
6. **Interior/Exterior Combinations**: Black exterior with black interior is the most common combination, showing strong correlation.

### **Proposed Improvements**
- **Dynamic Pricing**: Incorporating market trends and demand fluctuations into pricing strategies for better profitability.
- **Targeted Marketing**: Focusing on specific regions and vehicle types that show higher demand (e.g., Ford in Texas).
- **Color and Condition-Based Promotions**: Offering discounts or premium pricing for popular color and condition combinations.

## Dashboard
Explore the interactive analysis and key insights in the dashboard:
[Vehicle Sales and Market Trends Dashboard](https://app.powerbi.com/view?r=eyJrIjoiZjI5YTAwYWMtYmIwZS00NGY2LTg1MGMtZWY4ZTVjMjkzMTQ2IiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9)

