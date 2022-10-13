# Housing-Search
## Project Goals
1. To gain a general understanding of the housing market in Israel.
2. To determine the best neighborhoods to do the housing search, based on personally relevant criteria, such as price, size, room numbers, travel time to work (by car and public transportation), distance to family, etc.
3. To map similar cities.
4. Create a simple visualization in Tableau of an overview of the housing market for others to use:
https://public.tableau.com/app/profile/hannah.lang8212/viz/HousingSearchinIsrael/HousingListingsinIsrael

![image](https://user-images.githubusercontent.com/68339279/190895481-2aec3c2b-9c17-4448-94f5-150731428091.png)
[Image taken from https://www.mashvisor.com/blog/3-investment-property-search-tools-multi-family/]
## Methods
1. Scraping all housing listings in Israel from https://www.onmap.co.il/.
2. Cleaning/preprocessing the data.
3. Adding commuting times to work during rush hour for each listing. These were scraped from Google Maps using Selenium and BeautifulSoup.
4. Adding travel times to parents during rush hour for each listing.
5. Using hierarchical clustering to group together similar cities.

## Files
1. *data_extraction_on_map.ipynb*: A notebook containing the code for scraping onmap.co.il for all listings in Israel.
2. *on_map_housing_project.ipynb*: A notebook that cleans and processes the housing listings data, gathers travel times from Google Maps, and performs EDA to determine the best cities to search for housing, according to our criteria. 
3.  <b>'data' folder </b>
- *housing_data.csv.csv*: All of the housing listings in Israel scraped from onmap.co.il on September 1st, 2022.
- *transport_details.csv*: Driving and public transportation times from each lisiting to Azrieli, TLV by 9:00AM. Data was scraped from Google Maps using Selenium and BeautifulSoup.
- *driving_time_to_parents.csv*: Driving times from my parents' house to each listing to arrive by 4:00 PM. Data was scraped from Google Maps using Selenium and BeautifulSoup.
- *tableau_housing.xls*: Excel file to be used in Tableau for analysis. The file contains the cleaned and combined data.
