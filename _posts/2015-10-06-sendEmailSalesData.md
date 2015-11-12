---
category: Web Service Calls
path: '/msg/sendEmailSalesData'
title: 'sendEmailSalesData'
type: 'GET'

layout: nil
---

# sendEmailSalesData

##Overview
This call is used to provide the information of the given property id to the Aaextracts team.

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

### Request

* The headers must include a **valid authentication token**.

<table>
	<tbody>
	<tr>
		<th>Parameter</th>
		<th>Description</th>
		<th>Required</th>
		
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
		<td>op</td>
		<td>Operation</td>
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
		<td>saleDate</td>
		<td>Sale Date</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>salePrice</td>
		<td>Sale Price</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>saleType</td>
		<td>Sale Type</td>
		<td>No</td>
		
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