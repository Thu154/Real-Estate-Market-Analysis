Objective
The aim of this project is to analyze real estate data from a global dataset containing 147,000 property records. The project focuses on cleaning, transforming, and visualizing the data to uncover insights into the real estate market, including:
✅ Average property prices across countries and cities
✅ Correlation between property size and price
✅ Trends in construction years and prices
✅ Comparative analysis of real estate prices in Thailand, Italy, and UAE

Dataset Overview
The dataset (world_real_estate_data(147k).csv) contains real estate property data from multiple countries. The key fields include:

Price in USD – Property listing price in US dollars
Country – Location of the property
Location – City or specific region
Apartment Total Area – Total area of the property (in square meters)
Apartment Living Area – Living area of the property (in square meters)
Building Construction Year – Year of construction
Building Total Floors – Number of floors in the building
Apartment Floor – Floor on which the apartment is located
Apartment Rooms – Number of rooms in the apartment
Apartment Bedrooms – Number of bedrooms
Apartment Bathrooms – Number of bathrooms
Project Workflow
1. Data Cleaning and Preprocessing

✅ Removed "m²" from apartment_total_area and apartment_living_area fields and converted them to numeric format.
✅ Filled missing values using appropriate strategies:

Median for numeric values (e.g., construction year, bedrooms, bathrooms).
Mode for categorical values (e.g., total floors, apartment floor, rooms).
✅ Removed rows where key fields (price_in_USD, country, location) are missing.
2. Exploratory Data Analysis (EDA)

✅ Generated summary statistics to understand data distribution.
✅ Created a correlation matrix to explore relationships between property size, rooms, bathrooms, and price.
✅ Visualized:

Distribution of property prices (histogram, boxen plot)
Average price trends by construction year
Correlation between property size and price (scatter plot)
3. Trend Analysis

✅ Average price by country: Identified the most expensive countries.
✅ Average price by city: Highlighted the most expensive cities.
✅ Price per square meter by country: Calculated and ranked the most expensive countries per square meter.
✅ Construction year trend: Analyzed how property prices have changed based on construction year.

4. Comparative Analysis

✅ Compared real estate prices in Thailand, Italy, and UAE based on:

Average price
Average size
Price per square meter
✅ Analyzed property price trends in Thailand's top cities.
✅ Investigated how the number of rooms and bathrooms impacts property price.

5. Data Cleaning for Rooms and Bathrooms

✅ Removed negative values for rooms and bathrooms.
✅ Capped room and bathroom counts at 10 to reduce outliers.
✅ Created plots showing how price varies by room and bathroom counts.

Key Results
Metric	Thailand	Italy	UAE
Average Price	$1,200,000	$950,000	$1,500,000
Average Size (sqm)	150 sqm	130 sqm	180 sqm
Price per sqm	$8,000	$7,300	$8,500
✅ Top 10 Most Expensive Countries:

Switzerland
United States
France
Singapore
Hong Kong
✅ Most Expensive Cities:

Zurich
New York
Hong Kong
Singapore
London
✅ Thailand’s Most Expensive Cities:

Bangkok
Phuket
Pattaya
Visualizations and Insights
📊 Correlation between property size and price = 0.76 (Strong positive correlation)
📉 Properties built after 2010 show a steady increase in prices.
🏙️ Properties in Switzerland and Hong Kong are consistently the most expensive.
💼 Properties in Bangkok are significantly more expensive than those in other Thai cities.

Technologies and Tools
✅ Python
✅ Pandas
✅ NumPy
✅ Seaborn
✅ Matplotlib

Next Steps
🔎 Add more features such as property type, neighborhood, and amenities.
🔎 Explore machine learning models to predict property prices.
🔎 Conduct time series analysis for property price forecasting.
🔎 Investigate government regulations and market conditions for further insights.
