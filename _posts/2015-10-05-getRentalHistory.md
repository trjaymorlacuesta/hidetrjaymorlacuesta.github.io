---
category: Web Service Calls
path: '/msg/getRentalHistory'
title: 'getRentalHistory'
type: 'GET'

layout: nil
---

# getRentalHistory

##Overview
This method allows users to retrieve stuff.

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
		<td>-</td>
	</tr>

</tbody>
</table>

### Request

* The headers must include a **valid authentication token**.

<table>
	<tbody>
	<tr>
		<th>Parameter</th>
		<th>Value</th>
	</tr>
	<tr>
		<td>uid</td>
		<td>TWISTUSER001</td>
	</tr>
	<tr>
		<td>sid</td>
		<td>2-4eed242594fc464787b8054ddc77de11</td>
	</tr>
	<tr>
		<td>op</td>
		<td>getRentalHistory</td>
	</tr>
	<tr>
		<td>id</td>
		<td>-</td>
	</tr>
	<tr>
		<td>maxResult</td>
		<td>-</td>
	</tr>
</tbody>
</table>

<div id="msgtesturl">
<table>
	<tbody>
	<tr>
		<th>Test URL MSG Agent -MSGSIT:</th>
	</tr>
	<tr>
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?uid=TWISTUSER003&op=getRentalHistory&id=13093202&maxResult=5&sid=2-4eed242594fc464787b8054ddc77de11
		</td>
	</tr>
</tbody>
</table>
</div>

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