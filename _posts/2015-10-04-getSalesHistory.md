---
category: Web Service Calls
path: '/msg/getSalesHistory'
title: 'getSalesHistory'
type: 'GET'

layout: nil
---

# getSalesHistory

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
		<td>getSalesHistory</td>
	</tr>
	<tr>
		<td>id</td>
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
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?uid=TWISTUSER003&op=getSalesHistory&id=9925956&sid=2-4eed242594fc464787b8054ddc77de11
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
            "salesHistoryList": [
                {
                    "saleDate": "21/12/2011",
                    "salePrice": 350000,
                    "vendors": [
                        "Allan Rickards White"
                    ],
                    "saleType": ""
                },
                {
                    "saleDate": "01/07/1986",
                    "salePrice": 29000,
                    "vendors": [
                        ""
                    ],
                    "saleType": ""
                },
                {
                    "saleDate": "15/12/1980",
                    "salePrice": 34950,
                    "vendors": [
                        "Colin Booth",
                        "Diana H Booth"
                    ],
                    "saleType": ""
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