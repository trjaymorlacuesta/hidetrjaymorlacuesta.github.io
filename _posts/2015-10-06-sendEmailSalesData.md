---
category: Web Service Calls
path: '/msg/sendEmailSalesData'
title: 'sendEmailSalesData'
type: 'GET'

layout: nil
---

# sendEmailSalesData

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
		<td>sendEmailSalesData</td>
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
		<td>saleDate</td>
		<td>-</td>
	</tr>
	<tr>
		<td>salePrice</td>
		<td>-</td>
	</tr>
	<tr>
		<td>saleType</td>
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
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?uid=TWISTUSER003&op=sendEmailListingData&id=7007111&address=1 Turramurra Avenue Turramurra NSW 2074&agentName=Robert Velasco&agentFlag=true&listingDate=7/1/2010&listingPriceFrom=200000&listingPriceTo=500000&sid=2-4eed242594fc464787b8054ddc77de11
		</td>
	</tr>
</tbody>
</table>
</div>

### Response

Success:
```{
    "response": {
        "status": "success"
    }
}```

Error:
```{
    "response": {
        "status": "error",
        "description": "error description"
    }
}```