# python-api-challenge
WeatherPy and VacationPy Report

This project is split into two key activities: WeatherPy and VacationPy.

WeatherPy:

In WeatherPy, a Python script is used to visualize weather data for over 500 cities at varying distances from the equator. The cities are randomly generated using the Citipy library, and weather data is retrieved via the OpenWeatherMap API.

The following relationships between weather parameters and latitude are explored through scatter plots:

Latitude vs. Temperature

Latitude vs. Humidity

Latitude vs. Cloudiness

Latitude vs. Wind Speed

Next, the dataset is split into two hemispheres:

Northern Hemisphere: Cities with latitude ≥ 0°

Southern Hemisphere: Cities with latitude < 0°

For each hemisphere, linear regression is applied to the following relationships:

Temperature vs. Latitude

Humidity vs. Latitude

Cloudiness vs. Latitude

Wind Speed vs. Latitude

These analyses help to identify correlations between latitude and various weather parameters in both hemispheres. Finally, the processed data is saved into a CSV file for further use.

VacationPy:

In VacationPy, a map is created to visualize each city from the WeatherPy dataset, with the size of the points representing humidity levels.

A new dataframe is created using specific vacation-friendly criteria which are as follows:

Temperature: Between 21°C and 27°C

Wind Speed: Less than 4.5 m/s

Cloudiness: 0% (clear skies)

For each selected city, the first hotel within 10,000 meters of the city's coordinates is located using the Geoapify API. The map is updated to display these hotels, with hover messages providing the hotel name and country for each city.

This visualization can be used to identify ideal vacation spots based on weather conditions.

Conclusion:
WeatherPy reveals significant correlations between latitude and weather variables, showing how proximity to the equator affects temperature, humidity, cloudiness, and wind speed.
VacationPy provides a practical application of the weather data, helping users identify cities with ideal vacation conditions and nearby accommodations.
