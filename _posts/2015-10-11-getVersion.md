---
category: Web Service Calls
path: '/msg/getVersion'
title: 'getVersion'
type: 'POST'

layout: nil
---

# getVersion

##Overview
This call is used to get the current version and build date of the app.

<table>
	<tbody>
	<tr>
		<th>BSGv3</th>
		<th>BSGv2</th>
		<th>Show Additional Data Elements</th>
	</tr>
	<tr>
		<td>&nbsp;</td>
		<td>&nbsp;</td>
		<td>&nbsp;</td>
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
</tbody>
</table>

***Sample Request***
```{
    "op": "getVersion",
    "uid": "TWISTUSER001"
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "version": "3.13",
      "buildDate": "12-11-2015",
      "buildNo": "1"
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