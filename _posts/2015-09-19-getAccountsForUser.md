---
category: Web Service Calls
path: '/msg/getAccountsForUser'
title: 'getAccountsForUser'
type: 'GET'

layout: nil
---

# getAccountsForUser

##Overview
This method takes userName and password input and returns all active customer id(s) the user id is associated to; it uses BSGv2's getCustomersForUser under session services.

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
		<td>user</td>
		<td>User</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>passwd</td>
		<td>Password</td>
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
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?uid=TWISTUSER001&op=getAccountsForUser&user=bsguser.rpmob3.apple&passwd=bsgdevpass
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
            "customerList": [
                {
                    "customerName": "RPData-BSG Staging (National-NoVIC)",
                    "customerId": "26233"
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