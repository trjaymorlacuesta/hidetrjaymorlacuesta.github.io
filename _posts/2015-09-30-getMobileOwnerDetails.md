---
category: Web Service Calls
path: '/msg/getMobileOwnerDetails'
title: 'getMobileOwnerDetails'
type: 'POST'

layout: nil
---

# getMobileOwnerDetails

##Overview
This call is used to fetch the owner details of a specific property; it uses the BSGv2's GetPropertyDetail under owner list node. 

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
    "op": "getMobileOwnerDetails",
    "uid": "TWISTUSER001",
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "id": "7003499"
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "ownerName": "LIN MA",
      "ownerDetails": [
        {
          "ownerName": "LIN MA",
          "ownerAddress": "56 MAXWELL ST SOUTH TURRAMURRA NSW 2074"
        },
        {
          "ownerName": "XI ZHAO",
          "ownerAddress": "56 MAXWELL ST SOUTH TURRAMURRA NSW 2074"
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