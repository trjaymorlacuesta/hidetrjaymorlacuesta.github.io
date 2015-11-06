---
category: Web Service Calls
path: '/msg/getMobileMarketingContact'
title: 'getMobileMarketingContact'
type: 'GET'

layout: nil
---

# getMobileMarketingContact

##Overview
This method allows users to retrieve stuff.

<table>
	<tbody>
	<tr>
		<th>BSGv3</th>
		<th>BSGv2</th>
		<th>Show Additional Data Elements</th>
	</tr>
	<tr>
		<td>Yes</td>
		<td>No</td>
		<td>-</td>
	</tr>

</tbody>
</table>

### Request

* The headers must include a **valid authentication token**.

<table>
	<tbody>
	<tr>
		<th>Parameter</th>
		<th>Value</th>
	</tr>
	<tr>
		<td>uid</td>
		<td>TWISTUSER001</td>
	</tr>
	<tr>
		<td>sid</td>
		<td>2-4eed242594fc464787b8054ddc77de11</td>
	</tr>
	<tr>
		<td>op</td>
		<td>getMobileMarketingContact</td>
	</tr>
	<tr>
		<td>propertyIds</td>
		<td>-</td>
	</tr>
	<tr>
		<td>insertedDate</td>
		<td>-</td>
	</tr>
	<tr>
		<td>homeOwner</td>
		<td>-</td>
	</tr>
	<tr>
		<td>canCall</td>
		<td>-</td>
	</tr>
	<tr>
		<td>canMail</td>
		<td>-</td>
	</tr>
	<tr>
		<td>firstContact</td>
		<td>-</td>
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
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?op=getMobileMarketingContact&propertyIds=15348008,15793615,1593403,15057202,3698774&uid=TWISTUSER001&sid=2-4eed242594fc464787b8054ddc77de11
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
            "marketingContacts": [
                {
                    "propertyId": 1593403,
                    "contactType": "Marketing",
                    "person": {
                        "firstName": "Y",
                        "middleNames": "",
                        "initials": "Y",
                        "lastName": "Cai"
                    },
                    "mailingAddress": {
                        "careOf": "",
                        "line1": "5477 Braidwood Rd",
                        "line2": "",
                        "suburb": "BRISBANE GROVE",
                        "state": "NSW",
                        "postcode": "2580",
                        "country": "Australia",
                        "doNotMail": false
                    },
                    "phone": {
                        "phoneNumber": "0403258574",
                        "doNotCall": false
                    },
                    "headOfHousehold": false,
                    "homeOwner": false,
                    "income": "0-13000",
                    "peoplePerHousehold": "1",
                    "directResponsive": false,
                    "lastValidatedDate": "11/10/2013",
                    "expirationDate": "15/03/2014",
                    "lastModifiedDate": "14/03/2014"
                },
                {
                    "propertyId": 3698774,
                    "contactType": "Marketing",
                    "person": {
                        "firstName": "B",
                        "middleNames": "",
                        "initials": "B",
                        "lastName": "Hunt"
                    },
                    "mailingAddress": {
                        "careOf": "",
                        "line1": "60 Early St",
                        "line2": "",
                        "suburb": "CRESTWOOD",
                        "state": "NSW",
                        "postcode": "2620",
                        "country": "Australia",
                        "doNotMail": false
                    },
                    "phone": {
                        "phoneNumber": "",
                        "doNotCall": true
                    },
                    "headOfHousehold": false,
                    "homeOwner": false,
                    "income": "52000-73000",
                    "peoplePerHousehold": "3",
                    "directResponsive": false,
                    "lastValidatedDate": "01/11/2013",
                    "expirationDate": "15/03/2014",
                    "lastModifiedDate": "14/03/2014"
                },
                {
                    "propertyId": 15793615,
                    "contactType": "Marketing",
                    "person": {
                        "firstName": "Kathryn",
                        "middleNames": "",
                        "initials": "K",
                        "lastName": "Alexander"
                    },
                    "mailingAddress": {
                        "careOf": "",
                        "line1": "104 Rous River Way",
                        "line2": "",
                        "suburb": "MURWILLUMBAH",
                        "state": "NSW",
                        "postcode": "2484",
                        "country": "Australia",
                        "doNotMail": false
                    },
                    "phone": {
                        "phoneNumber": "",
                        "doNotCall": true
                    },
                    "headOfHousehold": false,
                    "gender": "F",
                    "homeOwner": false,
                    "income": "34000-52000",
                    "peoplePerHousehold": "2",
                    "directResponsive": false,
                    "lastValidatedDate": "24/01/2014",
                    "expirationDate": "15/03/2014",
                    "lastModifiedDate": "14/03/2014"
                },
                {
                    "propertyId": 15793615,
                    "contactType": "Marketing",
                    "person": {
                        "firstName": "Lionel",
                        "middleNames": "",
                        "initials": "L",
                        "lastName": "Alexander"
                    },
                    "mailingAddress": {
                        "careOf": "",
                        "line1": "104 Rous River Way",
                        "line2": "",
                        "suburb": "MURWILLUMBAH",
                        "state": "NSW",
                        "postcode": "2484",
                        "country": "Australia",
                        "doNotMail": false
                    },
                    "phone": {
                        "phoneNumber": "",
                        "doNotCall": true
                    },
                    "headOfHousehold": false,
                    "gender": "M",
                    "homeOwner": false,
                    "age": "55-59",
                    "income": "34000-52000",
                    "peoplePerHousehold": "2",
                    "directResponsive": false,
                    "lastValidatedDate": "24/01/2014",
                    "expirationDate": "15/03/2014",
                    "lastModifiedDate": "14/03/2014"
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