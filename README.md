This report section employs a data-driven approach to identify the five most populated cities in the United Kingdom. 
Utilizing code, the author retrieved real-time weather data for these cities, including temperature, humidity, and wind speed, through weather data APIs. 
The information is visually presented using data visualization techniques, enabling a quick and comparative analysis of meteorological patterns across cities.
This intersection of technology, geography, and meteorology enhances the report's depth and engagement, showcasing the dynamic relationship between urban landscapes and modern data methodologies.

While acknowledging the efficacy of the OpenWeatherMap API, it is imperative to note that its free version lacks the capability to access historical data. 
Consequently, for the purpose of demonstrating specific metrics and obtaining historical weather data, the OpenWeatherMap API has been substituted with the http://api.weatherapi.com/v1.
This alternative API facilitates the retrieval of historical weather information, thereby enhancing the comprehensiveness of the data analysis in the given activity report.

Retrieves weather forecast data from a list of URLs using the requests library, extracts relevant information from the JSON responses, and organizes it into a structured panda DataFrame.
The script begins by initializing an empty list named weather_data, which will store dictionaries representing individual hourly weather data. It then iterates through a list of URLs (urls_list) corresponding to weather forecast APIs. 
For each URL, it sends a request to the API, retrieves the JSON response, and extracts various weather parameters for each hour of the forecast.
The extracted information includes date and time, location details (country, city, region), precipitation probabilities (chance of rain and snow), cloud cover, humidity, visibility, wind direction, wind speed, and various daily average and extreme weather metrics.
This data is stored as a dictionary (row) for each hour and appended to the weather_data list.
Finally, a panda DataFrame (weather_df) is created from the list of dictionaries, and the resulting DataFrame is displayed, providing a tabular representation of the extracted weather forecast information.
