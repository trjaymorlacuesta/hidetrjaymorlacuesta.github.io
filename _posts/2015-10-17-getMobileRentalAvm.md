---
category: Web Service Calls
path: '/msg/getMobileRentalAvm'
title: 'getMobileRentalAvm'
type: 'POST'

layout: nil
---

# getMobileRentalAvm

##Overview
This call is used to fetch rental automated valuation model (RAVM) for residential property (Houses & Units) that includes the rental estimate, rental range, confidence score and forecast standard deviation (FSD) along with a list of comparable property IDs; it uses rental avm service under BSGv3.

<table>
	<tbody>
	<tr>
		<th>BSGv3</th>
		<th>BSGv2</th>
		<th>Show Additional Data Elements</th>
	</tr>
	<tr>
		<td>Yes</td>
		<td>No</td>
		<td></td>
	</tr>

</tbody>
</table>

### Additional Information

For further reading regarding BSG Elements: 

* [Rental AVM Service](http://confluence.rpdata.local/display/BA/Rental+AVM+Service)

### Request

***Parameters***

<table>
	<tbody>
	<tr>
		<th>Parameter</th>
		<th>Description</th>
		<th>Required</th>
		
	</tr>
	<tr>
		<td>op</td>
		<td>Operation</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>uid</td>
		<td>User ID</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>sid</td>
		<td>Session ID</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>propertyId</td>
		<td>Property Id</td>
		<td>Yes</td>
		
	</tr>
</tbody>
</table>

***Sample Request***
```{
    "op": "getMobileRentalAvm",
    "uid": "TWISTUSER001",
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "propertyId": "3976640"
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "rentalAvm": {
        "rentalAvmEstimate": "1230",
        "rentalAvmEstimateFsdScore": "42",
        "rentalAvmEstimateHigh": "1747",
        "rentalAvmEstimateLow": "712",
        "rentalAvmPeriod": "W",
        "rentalAvmRunDate": "13/11/2015",
        "rentalAvmScore": "29",
        "rentalAvmValuationDate": "02/11/2015",
        "rentalAvmYield": "3.86",
        "rentalAvmYieldFsdScore": "46",
        "comparableProperties": [
          "3982980",
          "3983116",
          "3979948",
          "3987019",
          "3976917",
          "3976809"
        ]
      }
    }
  }
}```

Error:
```{
    "response": {
        "status": "error",
        "description": "error description"
    }
}```