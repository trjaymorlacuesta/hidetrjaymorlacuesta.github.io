---
category: Web Service Calls
path: '/msg/getMobileRentalAvm'
title: 'getMobileRentalAvm'
type: 'GET'

layout: nil
---

# getMobileRentalAvm

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
		<td>getMobileRentalAvm</td>
	</tr>
	<tr>
		<td>propertyId</td>
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
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?op=getMobileRentalAvm&uid=TWISTUSER001&sid=2-4eed242594fc464787b8054ddc77de11&propertyId=3976640
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
            "rentalAvm": {
                "rentalAvmEstimate": "1240",
                "rentalAvmEstimateFsdScore": "41",
                "rentalAvmEstimateHigh": "1747",
                "rentalAvmEstimateLow": "733",
                "rentalAvmPeriod": "W",
                "rentalAvmRunDate": "03/11/2015",
                "rentalAvmScore": "29",
                "rentalAvmValuationDate": "26/10/2015",
                "rentalAvmYield": "3.90",
                "rentalAvmYieldFsdScore": "45",
                "comparableProperties": [
                    "3982980",
                    "3983116",
                    "3979948",
                    "3987286",
                    "3986359",
                    "3987019"
                ]
            }
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