---
category: Web Service Calls
path: '/msg/getUserDetails'
title: 'getUserDetails'
type: 'GET'

layout: nil
---

# getUserDetails

##Overview
This call is used to fetch the user details of a given sid. Returned data includes the personal, agency and work information.

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

</tbody>
</table>

<div id="msgtesturl">
<table>
	<tbody>
	<tr>
		<th>Test URL MSG Agent -MSGSIT:</th>
	</tr>
	<tr>
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?op=getUserDetails&uid=TWISTUSER001&sid=404-b9cae2209ddfbdf992e0ad54558716f3
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
        "description": "error.invalid.sessiontoken",
        "message": "You cannot be authenticated. You have recently either logged in on a different device, or changed your password. Please login again."
    }
}```