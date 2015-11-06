---
category: Web Service Calls
path: '/msg/getMobileTransactionDetailsByName'
title: 'getMobileTransactionDetailsByName'
type: 'GET'

layout: nil
---

# getMobileTransactionDetailsByName

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
		<td>No</td>
		<td>Yes</td>
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
		<td>getMobileTransactionDetailsByName</td>
	</tr>
	<tr>
		<td>firstName</td>
		<td>-</td>
	</tr>
	<tr>
		<td>lastName</td>
		<td>-</td>
	</tr>
	<tr>
		<td>companyName</td>
		<td>-</td>
	</tr>
	<tr>
		<td>state</td>
		<td>-</td>
	</tr>
	<tr>
		<td>country</td>
		<td>-</td>
	</tr>
	<tr>
		<td>firstNameBeginsWith</td>
		<td>-</td>
	</tr>
	<tr>
		<td>lastNameBeginsWith</td>
		<td>-</td>
	</tr>
	<tr>
		<td>companyNameBeginsWith</td>
		<td>-</td>
	</tr>
	<tr>
		<td>pageNumber</td>
		<td>-</td>
	</tr>
	<tr>
		<td>pageSize</td>
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
			<td>http://msgsit.rpdata.com/ttsvr/msgdebug?uid=TWISTUSER001&sid=2-4eed242594fc464787b8054ddc77de11&op=getMobileTransactionDetailsByName&lastName=salway&firstName=michael%20allan&country=&state=nsw&country=AUS&firstNameBeginsWith=false&lastNameBeginsWith=false&companyNameBeginsWith=&false
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