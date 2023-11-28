# Backend-API-for-Weather-Forecast
Weather api
Application Programming Interfaces that provide access to current & historical weather data on a global scale. There are several public weather APIs like OpenWeatherMap API, Dark Sky API, & Visual Crossing Weather API. These REST APIs can be used to build powerful weather apps
# Prerequisites

- Python
- Fladk
- Requests library
- Openweather API

# Brief Procedure
Install the required libraries.
Get your OpenWeatherMap API key.
Run the application.
Open Postman and create a new request to http://127.0.0.1:5000/weather with the GET method.
Add a query param location with the value being the city and state (eg: Bengaluru, KA).
Send the request and check the output.
NOTE: You can check the accuracy of the retrieved weather data by OpenWeatherMap.

# Weather API:  https://openweathermap.org
# Detailed explanation
Run the python script in VScode
In the terminal you can see the base url http://127.0.0.1:5000. When you click on this url, you will see 404 error.
Now go to your Postman workspace, set the request type to GET.
Enter the URL for your Flask API endpoint i.e, http://127.0.0.1:5000/weather?.
Click on the "Params" tab. In the "Key" column, enter location. In the "Value" column, enter the city and state for which you want to retrieve the weather information.
Click the send button to make the request.
Now go back to the base url, inorder to fetch the weather data, you have to append the base url with the api endpoint i.e, http://127.0.0.1:5000/weather?location=city,state (eg: http://127.0.0.1:5000/weather?location=Bengaluru, Karnataka&location=Shivamogga, Karnataka).
Now you can see the json file.

# Screenshots

![2023-11-28 (4)](https://github.com/VickyVikramS/Weather-Forcast/assets/152264791/0eef0c23-999e-43a5-8a93-fa6d22547b8c)
![2023-11-28 (5)](https://github.com/VickyVikramS/Weather-Forcast/assets/152264791/24628adf-4ed3-45a9-8b9c-481df4289cc1)
![2023-11-28 (6)](https://github.com/VickyVikramS/Weather-Forcast/assets/152264791/3f8c150e-915b-493d-b98c-a03c3c6b4a3c)
![2023-11-28 (7)](https://github.com/VickyVikramS/Weather-Forcast/assets/152264791/97a16a9a-320e-4b41-a47e-a08ea085d3b3)

# Additionals
This python script accepts multiple query parameters. The code includes the ability to retrieve weather information for multiple locations through the /weather endpoint.
The code includes try-except blocks to catch and handle exceptions that may occur during API requests or data processing.
Appropriate status codes are returned in the API responses, such as 400 for bad requests, 200 for response and 500 for internal server errors.
