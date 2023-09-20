# Project Name: Exploratory Data Analysis for Sample Superstore
________________________________________
## Project Objective: Find out weak areas where profit can be increased
________________________________________
## Data Sourcing
Data was provided by The Sparks Foundation in a [csv](https://bit.ly/3i4rbWl) file
________________________________________
## Data Transformation



A data model was created consisting of three tables: "Orders", "Geography," and "Category." Each table underwent a series of transformations to clean and structure the data appropriately.
### Orders Table 

The "Orders" table contains information related to segments, ship modes, sub-categories, sales, quantity, discounts, profits, and a custom "Geo ID" column. The following transformations were applied:

1. **Data Type Adjustments:** The data types of specific columns were modified to match their intended data types. For example, text, number, and percentage data types were assigned as appropriate.

2. **Geo ID Creation:** A custom column called "Geo ID" was added to the table. This column combines the "Postal Code" and "City" columns using a hyphen separator, providing a unique identifier for geographic locations.

3. **Column Removal:** Certain columns, including "Country," "City," "State," "Region," "Postal Code," and "Category," were removed from the table as they were deemed unnecessary for this table.

4. **Currency Data Types:** The data types of the "Sales" and "Profit" columns were changed to "Currency" to ensure consistent and accurate handling of monetary values.

5. **Percentage Data Type:** The data type of the "Discount" column was changed to "Percentage" to represent discounts appropriately.

6. **Measures Creation:** Two measures, "% Profit" and "Cost," were created to enhance the analytical capabilities of the dataset.

### Geography Table 

The "Geography" table was created to contain information about geographic locations, including "Geo ID," "Region," "State," "Country," "City," and "Postal Code." The following transformations were applied:

1. **Data Type Adjustments:** The data types of columns within the "Geography" table were adjusted to match their intended data types.

2. **Geo ID Creation:** Similar to the "Orders" table, a custom column called "Geo ID" was added to the "Geography" table. This column combines the "Postal Code" and "City" columns using a hyphen separator.

3. **Column Selection:** Only specific columns ("Geo ID," "Country," "City," "State," "Postal Code," and "Region") were retained in the table, ensuring that only relevant geographical information was included.

4. **Duplicate Removal:** Duplicate rows in the "Geography" table were removed to maintain data integrity.

### Category Table 

The "Category" table was created to contain information about product categories and sub-categories. The following transformations were applied:

1. **Data Type Adjustments:** The data types of columns within the "Category" table were adjusted to match their intended data types.

2. **Column Selection:** Only two columns, "Category" and "Sub-Category," were selected to be retained in the table, as these were the relevant attributes for analysis.

3. **Duplicate Removal:** Duplicate rows in the "Category" table were removed to ensure data accuracy and consistency.

________________________________________
## Insights and Recommendations

1. **Product Portfolio Review:**
   - Tables, furnishings and bookcases in the furniture category, as well as appliances, binders, machines, storage and supplies, are performing poorly. Consider discontinuing these products or reevaluating the pricing and marketing strategies for these products to ensure profitability.

1. **Discount Strategy:**
   - Given that sales, profit, and quantity consistently decrease as discount rates increase, it's advisable to consider removing or significantly reducing discounts, especially in the central and south regions. This can help improve overall profitability. Extreme discounts (e.g. 80%) on products like binders and appliances that lead to losses should be removed.
3. **Regional Focus Optimization:**
   - Given that the central and south regions are not as profitable as the east and west regions, consider reallocating resources and focusing more on the higher-performing regions to maximize profits.
7. **Customer-Centric Approach:**
   - Market research should be conducted to better understand customer preferences and needs in the central and south regions. Marketing and sales strategies should be tailored to the customer segments accordingly in order to focus on profitable products and pricing.

5. **Targeted Marketing:**
   - Low-quantity, high-profit-margin products like labels, envelopes, copiers, appliances, and fasteners should be targeted. Develop targeted marketing and promotion strategies to increase sales of these products. This can include advertising, bundling, or cross-selling with more popular items.


8. **State-Level Performance Monitoring:**
   - Keep a close eye on the performance of states like Tennessee, North Carolina, and Florida in the south region, Texas and Illinois in the central region, Ohio and Pennsylvania in the east region and Colorado, Arizona and Oregon in the west region. Consider adjusting pricing or discontinuing poor performing products in these states.

9. **Regular Performance Review:**
   - The data should be continuously monitored and reviewed regularly to gauge the impact of any changes made based on these recommendations while strategies are adjusted as needed to maintain and improve profitability of the store.

