**End-to-End Data Analysis Project Using Power BI: Zomato Dashboard**

**Project Overview**

This project showcases an **interactive and visually engaging Power BI dashboard** built to analyze Zomato's restaurant data. The dashboard provides key insights into restaurant performance across various cities, countries, and cuisines. The goal is to demonstrate data analysis skills, data visualization, and Power BI's capabilities in creating actionable insights.

**Key Objectives**
1. Analyze and visualize restaurant data from Zomato.
2. Provide insights into the distribution of restaurants by city, country, and cuisine.
3. Highlight key metrics such as total restaurants, votes, price ranges, and ratings.
4. Create an interactive dashboard for decision-making and exploration.

**Dataset Description**
The dataset used in this project contains information on Zomato restaurants, including:
- Restaurant name
- Cuisine type
- Location (City, Country)
- Ratings and reviews
- Price range
- Currency type
- Geographic information (latitude and longitude)

**Source**: Publicly available Zomato data, cleaned and prepared for analysis.

**Dashboard Highlights**
The **Zomato Dashboard** consists of the following sections and visualizations:

**1. Key Metrics**
- **Total Cities:** Displays the number of cities covered in the dataset (147 cities).
- **Total Countries:** Represents the number of countries included (15 countries).
- **Total Votes:** Sum of customer reviews or votes (1M).
- **Total Latitude:** Reflects geospatial data for mapping (247.64K).

**2. Visualizations**
- **Bar Chart (Total Restaurants by City):**
  - Shows the number of restaurants in each city.
  - Highlights New Delhi as having the most restaurants (5,473).

- **Pie Chart (Total Restaurants by Country):**
  - Displays the proportion of restaurants by country.
  - India dominates with 90.53% of the total restaurants.

- **Pie Chart (Currency by Country):**
  - Depicts the currency distribution across countries.

- **Combination Chart (Price Range by Rating and Restaurant Name):**
  - Compares the sum of price ranges and count of ratings for each restaurant.

---

**Project Workflow**
**1. Data Collection and Cleaning**
- Imported raw Zomato data.
- Cleaned and transformed the dataset using Power BI’s Power Query Editor:
  - Removed duplicates.
  - Handled missing values.
  - Standardized column formats for consistency.
  - Added calculated columns (e.g., price categories, rating thresholds).

**2. Data Modeling**
- Established relationships between tables (if applicable).
- Ensured proper cardinality and direction for relationships.

**3. DAX Measures**
- Created custom DAX measures for key metrics:
  - Total Restaurants:
    ```DAX
    [Total Restaurants] = COUNTROWS('Restaurant Table')
    ```
  - Average Rating:
    ```DAX
    [Average Rating] = AVERAGE('Restaurant Table'[Rating])
    ```
  - Sum of Price Range:
    ```DAX
    [Sum of Price Range] = SUM('Restaurant Table'[Price])
    ```

**4. Dashboard Design**
- Designed an interactive and user-friendly layout:
  - Filters: Country, City, Currency, and Restaurant Name.
  - KPI cards for key metrics.
  - Interactive visuals with drill-through capabilities.
- Used consistent color themes to enhance readability.

**Key Insights**
1. **City Analysis**:
   - New Delhi has the highest number of restaurants (5,473), followed by Gurgaon (1,118) and Noida (1,080).
2. **Country Analysis**:
   - India dominates with over 90% of the restaurants in the dataset.
3. **Price vs. Rating**:
   - High-priced restaurants do not necessarily have the highest ratings, offering insights into customer behavior.

**How to Run the Project**
1. **Download the Repository**:
   - Clone this repository to your local machine.

2. **Load the Dataset**:
   - Place the dataset in the `Data` folder (if not already included).

3. **Open Power BI Dashboard**:
   - Open the `.pbix` file in Power BI Desktop.

4. **Interact with the Dashboard**:
   - Use the filters and slicers to explore different aspects of the data.

 **Tools and Technologies**
- **Power BI**: For data visualization and dashboard creation.
- **Power Query**: For data cleaning and transformation.
- **DAX (Data Analysis Expressions)**: For creating measures and calculated columns.

**Future Enhancements**
- Add geospatial maps for visualizing restaurant locations.
- Incorporate time-based trends (if timestamps are available in the data).
- Predict customer preferences using machine learning models.
- Add more datasets for deeper analysis (e.g., customer demographics).

**Conclusion**
This project demonstrates how to leverage Power BI to turn raw data into actionable insights. The Zomato Dashboard serves as a valuable tool for stakeholders to understand restaurant performance and customer preferences at a glance.

Feel free to fork this repository, explore the dashboard, and contribute enhancements!
