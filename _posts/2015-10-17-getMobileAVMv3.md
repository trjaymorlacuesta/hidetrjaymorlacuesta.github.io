---
category: Web Service Calls
path: '/msg/getMobileAVMv3'
title: 'getMobileAVMv3'
type: 'GET'

layout: nil
---

# getMobileAVMv3

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
		<td>getMobileAVMv3</td>
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
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?op=getMobileAVMv3&uid=TWISTUSER001&sid=2-4eed242594fc464787b8054ddc77de11&propertyId=7003499
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
            "avmFaresDetail": {
                "faresCode": "0",
                "faresCondition": "SUCCESS",
                "faresDescription": "SUCCESS",
                "faresFSDScore": "8",
                "faresReferenceId": "NSW:1446531200442-47484034",
                "faresRunDate": "03/11/2015",
                "faresScore": "90",
                "faresValuationDate": "03/11/2015",
                "faresValueEstimate": "1799385",
                "faresValueHigh": "1937726",
                "faresValueLow": "1661043",
                "otmProperties": [
                    "6312242",
                    "6312333",
                    "6313311",
                    "6311902",
                    "6313520",
                    "6314108"
                ],
                "soldProperties": [
                    "6312307",
                    "6312935",
                    "6313640",
                    "6314504",
                    "6313540",
                    "6313676"
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