# Sales Analysis Dashboard

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/yourusername/company-data-analysis/blob/main/LICENSE)
[![Python](https://img.shields.io/badge/python-3.11-blue)](https://www.python.org/downloads/release/python-311/)

Sales Analysis Dashboard is a web-based data visualization project that aims to provide insights into a retail company's sales data. The main goal of the project is to help the company understand its sales performance, identify trends, and make data-driven decisions to improve profitability and customer satisfaction.
## Features

- **Interactive Dashboard**: The project includes an **interactive web-based dashboard** that allows users to explore and analyze the sales data visually. Users can interact with different charts and graphs to gain deeper insights into the data.
- **Sales by Category**: The dashboard provides a breakdown of sales across different product categories. It helps the company identify which product categories are performing well and which ones may need improvement.
- **Customer Segmentation**:  The project enables the company to analyze sales based on customer segments. By understanding the sales distribution across **different customer** types (e.g., corporate, consumer, home office), the company can tailor its marketing and sales strategies for different customer segments.
- **Geographical Analysis**: The dashboard includes a **map visualization** that displays sales data for different geographical regions. This helps the company identify potential target areas and analyze sales performance in different regions.

## Technologies Used

- Python
- Pandas
- Plotly
- Dash (Python framework for building web applications)

## Installation

> 1. Clone the repository:

``
git clone https://github.com/your_username/sales-analysis-dashboard.git
``


> 2. Install the required dependencies:

``
pip install pandas plotly dash
``


## Usage

> 1. Navigate to the project directory:

``
cd sales-analysis-dashboard
``


> 2. Run the dashboard:

``
python app.py
``

> 3. Open a web browser and go to http://127.0.0.1:8050/ to access the dashboard.

# IMPORTANT NOTE:

Since Github doesn't show the interactive map, this is what does it look like:

Code:
```
fig = px.choropleth_mapbox(df, geojson='https://raw.githubusercontent.com/python-visualization/folium/master/tests/us-states.json', 
                           locations='State', 
                           featureidkey="properties.name",
                           color='Sales',
                           color_continuous_scale="Viridis",
                           range_color=(0, 12),
                           mapbox_style="carto-positron",
                           zoom=3, center = {"lat": 37.0902, "lon": -95.7129},
                           opacity=1,
                           labels={'Sales':'Sales'}
                          )
fig.update_layout(margin={"r":0,"t":0,"l":0,"b":0})
fig.show()
```

![map](https://github.com/psalmsdove/Sales-Data-Analysis/assets/48603868/a5da9e0e-06bc-4c5b-a871-4023733a0dbf)



## Data Source

The project uses a sample sales dataset that is included in the `sales.xlsx` file. The dataset contains information about orders, customers, products, sales, profits and much more.


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

