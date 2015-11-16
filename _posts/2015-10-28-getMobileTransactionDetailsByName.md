---
category: Web Service Calls
path: '/msg/getMobileTransactionDetailsByName'
title: 'getMobileTransactionDetailsByName'
type: 'POST'

layout: nil
---

# getMobileTransactionDetailsByName

##Overview
This call will return transactions' transfer and related property information for the name searched i.e. will find all transactions which a person or company was involved in either as buyer or seller.

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
		<td>firstName</td>
		<td>First Name</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>lastName</td>
		<td>Last Name</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>companyName</td>
		<td>company Name</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>state</td>
		<td>State</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>country</td>
		<td>Country</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>firstNameBeginsWith</td>
		<td>First Name Begins With</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>lastNameBeginsWith</td>
		<td>Last Name Begins With</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>companyNameBeginsWith</td>
		<td>Company Name Begins With</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>pageNumber</td>
		<td>Page Number</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>pageSize</td>
		<td>Page Size</td>
		<td>No</td>
		
	</tr>
</tbody>
</table>

***Sample Request***
```{
    "op": "getMobileTransactionDetailsByName",
    "uid": "TWISTUSER001",
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "lastName": "salway",
    "firstName": "michael allan",
    "state": "nsw",
    "country": "AUS",
    "firstNameBeginsWith": "false",
    "lastNameBeginsWith": "false",
    "companyNameBeginsWith": "false"
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "transactionDetailsList": [
        {
          "propertyId": 5243888,
          "transferId": 52443719,
          "currentOwner": false
        },
        {
          "propertyId": 5243888,
          "transferId": 52443720,
          "currentOwner": false
        },
        {
          "propertyId": 7823008,
          "transferId": 0,
          "currentOwner": true
        },
        {
          "propertyId": 7823008,
          "transferId": 53701452,
          "currentOwner": false
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