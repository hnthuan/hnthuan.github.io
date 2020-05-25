# Add Ticket API

Add new ticket into MySQL server when driver drop the customer

> **POST /api/paymentgateway/addTicket**

| Attribute    | Type   | Description                                   |
|--------------|--------|-----------------------------------------------|
| fleetId      | String | Id of fleet, provided by QUp                  |
| bookId       | String | Id of booking                                 |
| distanceGG   | Double | Distance calculated base on Google API        |
| distanceTour | Double | Distance calculated base on GPS of the device |

## Example Request
```json
{
  "fleetId":"mycar",
  "bookId":"41813014",  
  "distanceGG":6270,
  "distanceTour":6840.666825771332
}
```
