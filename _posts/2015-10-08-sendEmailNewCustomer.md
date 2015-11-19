---
category: Web Service Calls
path: '/msg/sendEmailNewCustomer'
title: 'sendEmailNewCustomer'
type: 'POST'

layout: nil
---

# sendEmailNewCustomer

##Overview
This call is used to provide the given information to the Websales team.

<table>
	<tbody>
	<tr>
		<th>BSGv3</th>
		<th>BSGv2</th>
		<th>Show Additional Data Elements</th>
	</tr>
	<tr>
		<td>No</td>
		<td>No</td>
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
		<td>name</td>
		<td>Customer Name</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>phone</td>
		<td>Phone Number</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>email</td>
		<td>Email Address</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>date</td>
		<td>Date</td>
		<td>Yes</td>
		
	</tr>
</tbody>
</table>

***Sample Request***
```{
    "op": "sendEmailNewCustomer", 
    "uid": "TWISTUSER001", 
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "name": "John Doe", 
    "phone": "09153633987", 
    "email": "john-tooltwist.doe@gmail.com", 
    "date": "02/02/11" 
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "response": "Ok"
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