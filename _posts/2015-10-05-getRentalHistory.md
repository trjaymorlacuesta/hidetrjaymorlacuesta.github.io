---
category: Web Service Calls
path: '/msg/getRentalHistory'
title: 'getRentalHistory'
type: 'POST'

layout: nil
---

# getRentalHistory

##Overview
This call is used to fetch the rental history of a specific property; it uses the BSGv2's GetPropertyDetail under rental list node. 

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
		<td>maxResult</td>
		<td>Maximum Result</td>
		<td>No</td>
		
	</tr>
</tbody>
</table>

***Sample Request***
```{
    "op": "getRentalHistory", 
    "uid": "TWISTUSER003", 
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "id": "13093202", 
    "maxResult": "5" 
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "listings": [
        {
          "latestListedPrice": 450,
          "latestListDate": "28/11/2014",
          "agencyName": "Biggin & Scott Real Estate Prahan",
          "agentName": "Tasha Rai"
        },
        {
          "latestListedPrice": 450,
          "latestListDate": "11/11/2014",
          "agencyName": "Biggin & Scott - Toorak/Prahran",
          "agentName": "Tasha Rai"
        },
        {
          "latestListedPrice": 400,
          "latestListDate": "30/05/2014",
          "agencyName": "Biggin & Scott Real Estate Prahan",
          "agentName": "Tasha Rai"
        },
        {
          "latestListedPrice": 450,
          "latestListDate": "13/02/2014",
          "agencyName": "Biggin & Scott - Toorak/Prahran",
          "agentName": "Tasha Rai"
        },
        {
          "latestListedPrice": 450,
          "latestListDate": "06/11/2013",
          "agencyName": "Biggin & Scott Real Estate Prahan",
          "agentName": "Martin Joughin"
        }
      ]
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