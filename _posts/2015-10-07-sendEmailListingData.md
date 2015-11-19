---
category: Web Service Calls
path: '/msg/sendEmailListingData'
title: 'sendEmailListingData'
type: 'POST'

layout: nil
---

# sendEmailListingData

##Overview
This call is used to provide the information of the given property id to the Otmreports team.

<table>
	<tbody>
	<tr>
		<th>BSGv3</th>
		<th>BSGv2</th>
		<th>Show Additional Data Elements</th>
	</tr>
	<tr>
		<td>No</td>
		<td>Yes</td>
		<td></td>
	</tr>

</tbody>
</table>

### Additional Information

For further reading regarding BSG Elements: 

* [Method_getPropertyDetail](http://confluence.rpdata.local/display/BA/Method_getPropertyDetail)

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
		<td>id</td>
		<td>Property ID</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>address</td>
		<td>Address</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>agentName</td>
		<td>Agent Name</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>agentFlag</td>
		<td>Agent Flag</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>listingPriceFrom</td>
		<td>Listing Price From</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>listingPriceTo</td>
		<td>listing Price To</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>listingDate</td>
		<td>listing Date</td>
		<td>Yes</td>
		
	</tr>
</tbody>
</table>

***Sample Request***
```{
    "op": "sendEmailListingData", 
    "uid": "TWISTUSER003", 
    "sid": "2-4eed242594fc464787b8054ddc77de11", 
    "id": "7007111", 
    "address": "1 Turramurra Avenue Turramurra NSW 2074", 
    "agentName": "Robert Velasco", 
    "listingPriceFrom": "200000", 
    "listingPriceTo": "500000", 
    "listingDate": "7/1/2010"
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "response": "true"
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