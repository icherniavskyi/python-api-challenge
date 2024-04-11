# python-api-challenge

## VacationPy

This Python script performs data preprocessing and generates two maps. One map displays a point for every city where the size of the point reflects the humidity in each city. Another map displays cities with their corresponding weather conditions and nearby hotels based on specified criteria.

##### Dependencies
- Python 3
- pandas module
- hvplot.pandas module
- requests module
- geoapify_key (from api_keys)

##### Setup and Usage

1. Open script: VacationPy.ipynb
2. Install the required dependencies by running:
``` pip install pandas hvplot requests ```
3. Replace the api_keys.py file with your Geoapify API key.
4. Before running the script specify the input data file path. Ensure data is saved in the appropriate location.
5. Run the script.

 
##### Results and Features

- Visualizes cities on a map, with point sizes reflecting the humidity levels.
- Narrows down cities in the initial dataset based on weather conditions such as temperature, humidity, wind speed, and cloudiness.
- Searches for nearby hotels located within 10,000 meteres of each city using coordinates and the Geoapify API.
- Generates a map that allows users to hover over city points to view hotel names and countries.


## WeatherPy

This Python script generates a random cities list and retrieves weather data for each city. Next, the script creates scatter plots and computes linear regressions to explore the relationship between various weather variables and latitude.

##### Dependencies
- Python 3
- pandas module
- numpy module
- matplotlib.pyplot module
- requests module
- time module
- citipy module
- linregress (from scipy.stats)
- weather_api_key (from api_keys)

##### Setup and Usage

1. Open script: WeatherPy.ipynb
2. Install the required dependencies by running:
``` pip install matplotlib pandas numpy requests citipy ```
3. Replace the api_keys.py file with your OpenWeatherMap API key.
4. Before running the script specify the input data file path. Ensure data is saved in the appropriate location.
5. Run the script.

##### Results and Features

- Generates a random cities list based on a range of geographic coordinates using the citipy library.
- Retrieves weather data for the cities in generated list using the OpenWeatherMap API.
- Creates scatter plots to show relationships between latitude and weather variables (temperature, humidity, cloudiness, and wind speed).
- Performs linear regression analysis (separately for Northern and Southern Hemispheres) to determine the correlation between latitude and each weather variable.
- Saves scatter plots to output_data folder.
