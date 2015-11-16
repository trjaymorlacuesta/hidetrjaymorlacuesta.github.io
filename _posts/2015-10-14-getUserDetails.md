---
category: Web Service Calls
path: '/msg/getUserDetails'
title: 'getUserDetails'
type: 'POST'

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
    </tbody>
</table>

***Sample Request***
```{
    "op": "getUserDetails", 
    "uid": "TWISTUSER001", 
    "sid": "2-4eed242594fc464787b8054ddc77de11"
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "personalInformation": {
        "username": "tan.tran",
        "title": "MR",
        "firstName": "Tan",
        "lastName": "Tran",
        "phoneNumber": "07 33725766",
        "mobileNumber": "",
        "emailAddress": "ttn@rpdata.com",
        "faxNumber": "",
        "photo": ""
      },
      "workInformation": {
        "emailAddress": "ttn@rpdata.com",
        "mobileNumber": "007",
        "phoneNumber": "",
        "faxNumber": ""
      },
      "agencyInformation": {
        "tradename": "Tan Tran - Staff Account",
        "address1": "C/- RP DATA",
        "address2": "",
        "suburb": "CLAYFIELD",
        "postcode": "4011",
        "state": "QLD",
        "country": "AUS",
        "phoneNumber": "07 38574411",
        "website": "",
        "faxNumber": "07 38574896",
        "industrySegment": "ST",
        "franchiseId": 48,
        "logo": "https://rpp.rpdata.com/rpp/images/logos/prdnational.gif"
      }
    }
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