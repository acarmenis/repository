# repository
Contains code
This is a mavenized springboot Rest Api Application.

------------------------------------------------------------
Contains the follow modules
------------------------------------------------------------
ferry-scanner, model, services, web  
------------------------------------------------------------

Run
------------------------------------------------------------
Please, do the follow to run the application
Import to IDE i.e. IntelliJ
Do clean, install
Run the App class
 

Description.
------------------------------------------------------------
Request requirements
------------------------------------------------------------
   The API endpoint must accept an ISO 3166-1 alpha-2 country code2 using a proper HTTP request method.

Response requirements
------------------------------------------------------------
  The API endpoint must return a list of all the available weather station names for the given country, along with the current corresponding temperature. The applicant has complete freedom to use as many services as the web services of geonames.org either by using the provided credentials of the user ferryscanner or by creating a new one. 
See services: countryInfo, cities, weatherJSON

The MVP outcome will be a Spring Boot application containing the requested REST API endpoint and being completely autonomous and self-hosted using with an embeded servlet container preferably tomcat or undertow.

Testing
------------------------------------------------------------
  The API consumer can be an integration test producing sufficient output, a Postman6 collection or even a simple web page.
For testing the app, please use the Postman Api (https://www.getpostman.com/)
i.e.  http://localhost:8080/weather/country/US, where US would be any valid ISO 3166-1 alpha-2 country code.
Type: Basic Auth
Username: jerome
Password: jerome123

Sample of Output:
----------------------------------------------------------------------
{
    "countryCode": "US",
    "stationNameTemperatures": [
        {
            "stationName": "GARRETT CO",
            "temperature": "3"
        },
        {
            "stationName": "DRIGGS REED MEM",
            "temperature": "1"
        },
        {
            "stationName": "ROANOKE RAPIDS",
            "temperature": "14"
        }.....
 }

