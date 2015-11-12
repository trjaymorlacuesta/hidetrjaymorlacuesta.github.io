---
category: Web Service Calls
path: '/msg/getMobilePropertyAdditionalInfo'
title: 'getMobilePropertyAdditionalInfo'
type: 'GET'

layout: nil
---

# getMobilePropertyAdditionalInfo

##Overview
This call is used when the property details need to append the other fields coming from property service BSGv3 that aren't available on BSGv2 such as folio, volumn and siteValueList; it uses BSGv3's property service.

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
		<td>propertyId</td>
		<td>Property Id</td>
		<td>Yes</td>
		
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
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?op=getMobilePropertyAdditionalInfo&uid=TWISTUSER001&sid=2-4eed242594fc464787b8054ddc77de11&propertyId=7764519
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
            "occupancyType": "Owner Occupied",
            "mapReference": "UBD NSW: CCT40, L4",
            "folio": "",
            "volume": "",
            "saleDate": "17/09/2009",
            "salePrice": "415000",
            "siteValueLists": [ ],
            "isAgentAdvised": false
        }
    }
}```

Error:
```{
    "response": {
        "status": "error",
        "description": ""
    }
}```