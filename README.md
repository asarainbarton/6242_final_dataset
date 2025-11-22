COLUMNS

month_date_yyyymm
postal_code
zip_name
median_listing_price
new_listing_count
active_listing_count
total_listing_count
price_reduced_count
price_increased_count
median_listing_price_per_square_foot
median_square_feet
mean_num_bedrooms
mean_num_bathrooms
median_income
unemployment_rate
DGS10

************************************************************************

INDIVIDUAL COLUMN COVERAGE FOR ADDED COLUMNS

Column	Rows with Data	Coverage %	Rows Missing
unemployment_rate	2,865,291	99.24% 	21,990 (0.76%)
median_income	    2,844,123	98.51% 	43,158 (1.49%)
mean_num_bedrooms	2,001,446	69.32%	885,835 (30.68%)
mean_num_bathrooms	2,001,446	69.32%	885,835 (30.68%)

************************************************************************

DATA SOURCES

** Bulk of the Data **

https://www.realtor.com/research/data/

** Bedroom and Bathroom Data **

https://www.zillow.com/research/data/

** Income Data **

Main API
https://api.census.gov/data.html

Request URL and params for fetching data

url = f"https://api.census.gov/data/{year}/acs/acs5"
params = {
            'get': 'NAME,B19013_001E',
            'for': 'zip code tabulation area:*'
}


** Unemployment Rate Data **

https://fred.stlouisfed.org/searchresults/?st=unemployment&isTst=1


