# Airline-Routes-API
Static airline route data that provides general but useful information on operating airline routes globally.

<div id="header" align="center">
  <img src="https://media.giphy.com/media/LRZc4dV2kf787nbOB3/giphy.gif" width="100"/>
</div>

[Aviyair’s Airline Routes API]( https://aviyair.com/airline-routes-api/) provides useful details on airline routes that operate between international airports around the world. The API has clear data on airline routes that point out the departure and arrival airport, flight times, numbers, aircraft and other details as well as the waypoints in the air.

The airline routes data is accessible via GET requests and data is returned in JSON format. Other formats may be added in the future. Let us know if you have a demand for a specific format!

Get complete airline route data in a single call or narrow down the data to routes of a certain airline, flight number, departure or arrival airport, aircraft registration number and more.

--------

## Main Endpoint and Filters with Description

**GET** `https://data.aviyair.com/data/v1/airlineroutes?key=[APIKEY]`

Add at least one of the parameters below to fetch data accordingly. It is possible to fetch all routes by adding a high limit value, too.
You can add the below filters to narrow down the airline routes in the response.

| Request Parameter  | Description |
| ------------- | ------------- |
| airport_iata | Filter the flights based on the three-letter IATA code of the airport |
| airline_iata  | Filter the flights based on the aircraft status as either depature or arrival   |
| airline_icao  | Filter the flights based on the flight status designated as (started, en-route, landed, unknown) For outputs limit the value  |
| flight_number| Filter the flights based on the three-letter IATA code of the departure airport |

------

## 200 OK Response Example

```
{
  "status": {
    "message": "Success"
  },
  "results": {
    "airlineIata": "0B",
    "airlineIcao": "BMS",
    "arrivalIata": "TRN",
    "arrivalIcao": "LIMF",
    "arrivalTerminal": null,
    "arrivalTime": "10:45:00",
    "codeshares": null,
    "departureIata": "OTP",
    "departureIcao": "LROP",
    "departureTerminal": null,
    "departureTime": "09:15:00",
    "flightNumber": "101",
    "regNumber": "YR-BAP"
  }
}
```

-------


## Full Documentation

Please visit our [website](https://aviyair.com/documentation/).

-------
## Combine Airline Routes Data with Other APIs

In addition to the static airline route data, you can also combine this API to track the status and position of these routes in real time by using our Flight Tracker and Status API and Global Flight Schedules API. See our complete list of GitHub repos to get inspired or contact us if you have a specific project in mind. Our team will get back to you with the most useful endpoints to combine so you can integrate the exact data you need.

------

## Most Popular Use Cases

These are the most common use cases for the Airline Routes API but there are no limitations regarding how the API can be useful for you. If you have any concerns about the Terms and Conditions for the real-time flight delay data, you may visit the hyperlink below or contact us to ask about it.

-	Flight booking websites can integrate the Airline Routes API to display available routes from and to certain airports of their clients’ choices. The data displays route details such as flight times.
-	Travel planning and tourism websites and mobile apps can add a feature on their website that helps users create the perfect travel plan they wish by selecting a single destination or multiple legs.
-	Especially when combined with Aviyair flight schedule or flight delay data, the Airline Routes API can be a useful tool to analyze route efficiency, popularity and analytics (such as average delay and cancellation, flight time, demand and other metrics).
-	Also, when combined with other APIs, airlines can use the Airline Routes API to track their own performance and see patterns and trends related to flight delays and cancellations. Based on the reports, it is easier for airlines and airports to come up with solutions. Likewise, they can use this data to measure their competitors’ performances to come up with competitive and profitable solutions.
- 	Route efficiency analysis for airlines and airports

---------

## License

[Terms and Conditions of Use](https://aviyair.com/terms-and-conditions/) apply. If you have any questions or concerns about your use case of the Airline Routes API, please [contact us](https://aviyair.com/contact-aviyair/). 

--------

## How to Access

The API key to access static airline routes data is possible by creating an API subscription. The subscriptions do not require any commitments. It is possible to cancel anytime or make changes to your subscription level.

[View the prices and get an API key here.](https://aviyair.com/pricing-subscription-plans/)
