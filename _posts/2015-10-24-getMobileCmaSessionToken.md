---
category: Web Service Calls
path: '/msg/getMobileCmaSessionToken'
title: 'getMobileCmaSessionToken'
type: 'POST'

layout: nil
---

# getMobileCmaSessionToken

##Overview
This call is used to generate a session token and by pass the login procedures of rpp site; the user need to pass the page.

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
	<tr>
		<td>sid</td>
		<td>Session ID</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>page</td>
		<td>Page</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>propertyId</td>
		<td>Property Id</td>
		<td>Yes</td>
		
	</tr>
</tbody>
</table>

***Sample Request***
```{
    "op": "getMobileCmaSessionToken",
    "uid": "TWISTUSER001",
    "sid": "2-4eed242594fc464787b8054ddc77de11",
	"username": "bsguser.vivant",
	"password": "RNPgN5bx",
	"appCode": "rppipad",
	"page": "8",
	"propertyId": "3604024"
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "sessionToken": "https://rpp.rpdata.com/rpp/flow/avm.html?src=test&timestamp=2015-11-13T17:00:04+10:00&token=2-4eed242594fc464787b8054ddc77de11&apiKey=a95607eba0d92ffdee24b3b13d2c1e899b868000&hash=3c568aea2c3b3ffa6922d2bd65c63bd8d868bc87"
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