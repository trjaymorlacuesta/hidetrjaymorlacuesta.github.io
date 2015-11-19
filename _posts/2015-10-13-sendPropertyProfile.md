---
category: Web Service Calls
path: '/msg/sendPropertyProfile'
title: 'sendPropertyProfile'
type: 'POST'

layout: nil
---

# sendPropertyProfile

##Overview
This call is used to fetch the property profile report of a particular property; it uses the BSGv2.

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

### Additional Information

For further reading regarding BSG Elements: 

* [Method_getPropertyProfile](http://confluence.rpdata.local/display/BA/Method_getPropertyProfile)

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
		<td>propertyId</td>
		<td>Property Id</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>bedroom</td>
		<td>Number of Bedroom</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>bathroom</td>
		<td>Number of Bathroom</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>carspace</td>
		<td>Number of Carspace</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>email</td>
		<td>Email Address</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>firstname</td>
		<td>First Name</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>surname</td>
		<td>Surname</td>
		<td>No</td>
		
	</tr>
</tbody>
</table>

***Sample Request***
```{
	"op": "sendPropertyProfile", 
	"uid": "TWISTUSER001", 
	"sid": "2-4eed242594fc464787b8054ddc77de11", 
	"email": "dennis.salibio@tooltwist.com", 
	"propertyId": "7007111", 
	"firstname": "dennis", 
	"surname": "salibio", 
	"bedroom": "1", 
	"bathroom": "1", 
	"carspace": "1"
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "response": "success",
      "doneTransaction": true
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