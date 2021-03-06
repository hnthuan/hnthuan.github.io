# API estimatefare

| Parameters       | Type   | Regular | Flat | Hourly | Intercity | Description                         | Values                                                                                                                            |
|------------------|--------|:-------:|:----:|:------:|:---------:|-------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| fleetId          | String |    x    | x    | x      | x         | Id of fleet                         |                                                                                                                                   |
| distance         | Double |    x    |      |        |           | Required if bookType = 0/1/2        |                                                                                                                                   |
| vehicleTypeId    | UUID   |    x    | x    | x      | x         | Id of vehicle type                  |                                                                                                                                   |
| zipCodeFrom      |        |         |      |        |           |                                     |                                                                                                                                   |
| zipCodeTo        |        |         |      |        |           |                                     |                                                                                                                                   |
| duration         |        | x       | x    | x      |           | Required if bookType = 0/1/2        |                                                                                                                                   |
| pickup           |        | x       | x    | x      | x         |                                     |                                                                                                                                   |
| destination      |        | x       | x    |        | x         | Required if bookType = 0/1/2        |                                                                                                                                   |
| bookFrom         |        | x       | x    | x      | x         |                                     | - CC, API, Car-hailing, Web booking, Partner, mDispatcher, Kiosk, webBooking, partner <br>- Pax app name (ex: tappar, ecar, ....) |
| bookType         |        | x       | x    | x      |           |                                     | 0 - one way<br>1 - from airport<br>2 - to airport<br>3 - hourly<br>4 - round trip                                                 |
| pickupTime       |        | x       | x    | x      | x         |                                     |                                                                                                                                   |
| meetDriver       |        |         |      |        |           |                                     | - 1 - NA<br>0 - on curb<br>1 - meet driver                                                                                        |
| userId           |        |         |      |        | x         |                                     |                                                                                                                                   |
| city/timezone    |        | x       | x    | x      | x         |                                     |                                                                                                                                   |
| tip              |        |         |      |        |           |                                     |                                                                                                                                   |
| promoCode        |        |         |      |        |           |                                     |                                                                                                                                   |
| phone            |        |         |      |        |           |                                     |                                                                                                                                   |
| actualFare       |        |         |      |        |           |                                     |                                                                                                                                   |
| corporateId      |        |         |      |        |           |                                     |                                                                                                                                   |
| packageRateId    |        |         |      | x      |           | Required if bookType = 3            |                                                                                                                                   |
| pricingType      |        | x       | x    | x      | x         |                                     | 0: local<br>1: affiliate                                                                                                          |
| typeRate         |        | 0       | 1    | 2      | 3         |                                     | 0 - Regular <br>1 - Hourly<br>2 - Round trip<br>3 - Intercity                                                                     |
| services         |        |         |      |        |           | Additional service (list serviceId) |                                                                                                                                   |
| rv               |        | x       | x    | x      |           |                                     |                                                                                                                                   |
| extraDestination |        |         |      |        |           |                                     |                                                                                                                                   |
| seat             |        |         |      |        | x         |                                     |                                                                                                                                   |
| luggage          |        |         |      |        | x         |                                     |                                                                                                                                   |
| intercityRouteId |        |         |      |        | x         |                                     |                                                                                                                                   |
| routeNumber      |        |         |      |        | x         |                                     | 1 - round 1<br>2 - round 2                                                                                                        |

## Eta example

<panels:start>
<div:title-panel>

  (...) - Awesome title

<div:left-panel>

  (...) - Awesome explanation

<div:right-panel>


  (...) - Awesome example

<panels:end>
