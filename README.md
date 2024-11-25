# website_weather
LINK:  https://andreilucacel.github.io/website_weather/
The weather website I created utilizes JavaScript to provide real-time weather information based on user input or geolocation.
API Integration: The website leverages two APIs: one for geolocation and another for weather forecasting. The API_GEOLOCATION_URL fetches city coordinates, while the API_FORECAST_URL retrieves weather data based on those coordinates.

User Interface Interaction: Users can either input a city name through a form or click a button to get their current location. The event listeners handle these interactions, triggering functions to fetch and display weather data.

Fetching Data:

When a user submits a city name, the onCityFormSubmit function prevents the default form submission, clears any previous content, and validates the input. If the input is valid, it fetches the city coordinates and then retrieves the weather data using the fetched coordinates.
If the user opts for location-based weather, the onLocationBtnClick function uses the browser's geolocation feature to get the user's current position and then fetches the corresponding weather data.
Data Processing: The fetched weather data is processed in the parseApiData function, which organizes the current weather conditions and forecasts into a structured format. This includes extracting details like temperature, wind speed, humidity, and weather codes.

Displaying Results: The displayWeather function updates the user interface with the current weather and the forecast for the coming days. It creates sections for today’s weather and future forecasts, utilizing helper functions to build panels that display the data visually.

User Experience Enhancements: The website includes loading indicators to inform users when data is being fetched and error handling to display messages when something goes wrong (like if the city name cannot be found or if geolocation fails).

Dynamic Weather Icons: The weather conditions are represented visually using icons, which are dynamically selected based on the weather codes returned from the API, adjusting for day or night.

Overall, this weather website combines user-friendly design with robust functionality to provide accurate weather updates, making it a valuable tool for users seeking weather information for specific locations or their current position.
