---
category: Web Service Calls
path: '/msg/getSalesHistory'
title: 'getSalesHistory'
type: 'POST'

layout: nil
---

# getSalesHistory

##Overview
This call is used to fetch the rental history of a specific property; it uses the BSGv2's GetPropertyDetail under sales history list node. 

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
</tbody>
</table>

***Sample Request***
```{
    "op": "getSalesHistory",
    "uid": "TWISTUSER001",
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "id": "9925956"
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "salesHistoryList": [
        {
          "saleDate": "21/12/2011",
          "salePrice": 350000,
          "vendors": [
            "Allan Rickards White"
          ],
          "saleType": ""
        },
        {
          "saleDate": "01/07/1986",
          "salePrice": 29000,
          "vendors": [
            ""
          ],
          "saleType": ""
        },
        {
          "saleDate": "15/12/1980",
          "salePrice": 34950,
          "vendors": [
            "Colin Booth",
            "Diana H Booth"
          ],
          "saleType": ""
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