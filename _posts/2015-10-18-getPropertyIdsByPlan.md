---
category: Web Service Calls
path: '/msg/getPropertyIdsByPlan'
title: 'getPropertyIdsByPlan'
type: 'GET'

layout: nil
---

# getPropertyIdsByPlan

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
		<td>getPropertyIdsByPlan</td>
	</tr>
	<tr>
		<td>searchString</td>
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
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?op=getPropertyIdsByPlan&uid=TWISTUSER001&sid=2-4eed242594fc464787b8054ddc77de11&searchString=DP635%20BERALA%20NSW
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
            "propertyIdList": [
                1392165,
                1392167,
                1392178,
                1392180,
                1392182,
                1392184,
                1392191,
                1392193,
                1392195,
                1392196,
                1392197,
                1392198,
                1392199,
                1392200,
                1392201,
                1392202,
                1393417,
                1393418,
                1393419,
                1393420,
                1393421,
                1393422,
                1393423,
                1393424,
                1393425,
                1393426,
                1393427,
                1393428,
                1393429,
                1393430,
                1393431,
                1393432,
                1393433,
                1393434,
                1393435,
                1393436,
                1393437,
                1393438,
                1393439,
                1393440,
                1393441,
                1393442,
                1393443,
                1393444,
                1393445,
                1393446,
                1393447,
                1393448,
                1393549,
                1393550,
                1393551,
                1393552,
                1393553,
                1393554,
                1393555,
                1393556,
                1393557,
                1393558,
                1393559,
                1393560,
                1393561,
                1393562
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