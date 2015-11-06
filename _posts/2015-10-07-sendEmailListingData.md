---
category: Web Service Calls
path: '/msg/sendEmailListingData'
title: 'sendEmailListingData'
type: 'GET'

layout: nil
---

# sendEmailListingData

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
		<td>sendEmailListingData</td>
	</tr>
	<tr>
		<td>id</td>
		<td>-</td>
	</tr>
	<tr>
		<td>address</td>
		<td>-</td>
	</tr>
	<tr>
		<td>agentName</td>
		<td>-</td>
	</tr>
	<tr>
		<td>agentFlag</td>
		<td>-</td>
	</tr>
	<tr>
		<td>listingPriceFrom</td>
		<td>-</td>
	</tr>
	<tr>
		<td>listingPriceTo</td>
		<td>-</td>
	</tr>
	<tr>
		<td>listingDate</td>
		<td>-</td>
	</tr>
</tbody>
</table>

### Response

Success:
```{
    "response": {
        "status": "success",
        "result": {
            "results": "Results"
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