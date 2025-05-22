# Dashboard Documentation

## Overview

This dashboard provides insights into company performance based on the Fortune 1000 data, focusing on financial metrics, leadership profiles, and geographical distribution. It includes interactive elements such as PivotTables, charts, and slicers for dynamic data exploration.

## Components

### 1. Data Source

- **Source**: Fortune 1000 dataset (CSV format).
- **Key Fields**:
  - Company Name
  - Market Capitalization
  - Revenues
  - Profits
  - Country
  - Headquarters City
  - Leadership Information (e.g., CEO Gender, Founder Status)

### 2. Data Processing

Data was processed using Power Query (M Language) to:
- Clean and transform text fields.
- Convert numerical fields to appropriate data types.
- Add calculated fields such as Profit Margin and Growth Rate.

### 3. PivotTables

#### A. Market Cap by Country

- **Rows**: Country
- **Values**: Sum of MarketCap_March28_M
- **Description**: Displays total market capitalization by country.

#### B. Revenue by Industry

- **Rows**: Industry
- **Values**: Sum of Revenues_M
- **Description**: Shows total revenues categorized by industry.

#### C. Headquarters City Analysis

- **Rows**: HeadquartersCity
- **Values**: Sum of MarketCap_March28_M or Revenues_M
- **Description**: Analyzes financial metrics based on headquarters location.

### 4. Visualizations

#### A. Map Chart

- **Type**: Filled Map
- **Data Source**: Market Cap by Country PivotTable
- **Description**: Visualizes total market capitalization distribution across countries.

#### B. Bar/Column Charts

- **Type**: Bar Chart for Market Cap by Sector
- **Type**: Column Chart for Revenue by Industry
- **Description**: Visual representations of financial data providing quick insights.

### 5. Slicers

Slicers enhance interactivity by allowing users to filter data dynamically.

#### A. Added Slicers

- **Fields**:
  - Sector
  - Country
  - Leadership Profile
- **Functionality**: Users can select specific categories to filter all connected PivotTables and charts accordingly.

### 6. Dashboard Layout

- **Arrangement**: 
  - Callout cards for key metrics at the top.
  - PivotTables displayed centrally.
  - Charts positioned for visual impact.
  - Slicers placed for easy access at the side.

### 7. User Interaction

- **Filtering**: Users can click on slicers to filter the entire dashboard based on selected criteria.
- **Data Exploration**: Hovering over charts provides additional data insights.

### 8. Final Notes

- **Save Your Work**: Ensure the workbook is saved periodically to avoid data loss.
- **Testing**: Regularly check that all slicers and connections function correctly after any updates.

### Conclusion

This dashboard serves as a comprehensive tool for analyzing the Fortune 1000 dataset, offering valuable insights into company performance and leadership dynamics. It combines data processing, visualization, and interactivity to facilitate informed decision-making. If you need further modifications or additional features, please feel free to reach out!
