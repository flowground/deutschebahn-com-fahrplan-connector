# ![LOGO](logo.png) Fahrplan-Free **flow**ground Connector

## Description

A generated **flow**ground connector for the Fahrplan-Free API (version v1).

Generated from: https://api.apis.guru/v2/specs/deutschebahn.com/fahrplan/v1/swagger.json<br/>
Generated at: 2019-05-07T17:40:12+03:00

## API Description

A RESTful webservice to request a railway journey - FREE plan with restricted access (max. 10 requests per minute). Please ignore the message in the API Console about the access token.

Register to use an less restricted version, which requires an access token.

## Authorization

This API does not require authorization.

## Actions

### Get arrival board of a location

> Get arrival board at a given location at a given daten and time.

#### Input Parameters
* `id` - _required_ - Id of location. Use attribute 'id' from the result of 'location'
* `date` - _required_ - Date and time in ISO-8601 format, yyyy-mm-ddThh:mm:ss, example: 2017-04-01 or 2017-04-01T10:30

### Get departure board of a location

> Get departure board at a given location at a given daten and time.

#### Input Parameters
* `id` - _required_ - Id of a location. Use attribute 'id' from the result of 'location'
* `date` - _required_ - Date and time in ISO-8601 format, yyyy-mm-ddThh:mm:ss, example: 2017-04-01 or 2017-04-01T10:30

### Get details about a single journey

> Retrieve details of a journey. The id of journey should come from an arrival board or a departure board.

#### Input Parameters
* `id` - _required_ - Id of a journey. Use attribute 'detailsId' from the result of  'arrivalBoard' or 'departureBoard'

### Get location information

> Get information about locations matching the given name or name fragment

#### Input Parameters
* `name` - _required_ - Name or name fragment of a location

## License

**flow**ground :- Telekom iPaaS / deutschebahn-com-fahrplan-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
