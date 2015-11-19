---
category: Web Service Calls
path: '/msg/checkMobileAvm'
title: 'checkMobileAvm'
type: 'POST'

layout: nil
---

# checkMobileAvm

##Overview
This call is used to fetch live automated valuation model (AVM) for a property that includes the valuation estimate, value range, confidence score and forecast standard deviation (FSD) along with a list of comparable property IDs; it uses under avm service under BSGv2.

If appCode is rpm3 is passed as appCode, it will avm service under BSGv3.

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

* [Method_getAVM](http://confluence.rpdata.local/display/BA/Method_getAVM)
* [Method_getPropertySummaryList](http://confluence.rpdata.local/display/BA/Method_getPropertySummaryList)
* [Method_getOtmPropertySummaryList](http://confluence.rpdata.local/display/BA/Method_getOtmPropertySummaryList)
* [Method_search](http://confluence.rpdata.local/display/BA/Method_search)

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
		<td>id</td>
		<td>Property ID</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>useLiveAvm</td>
		<td>Use Live Avm</td>
		<td>No</td>
		
	</tr>
</tbody>
</table>

***Sample Request***
```{
    "op": "checkMobileAVM", 
    "uid": "TWISTUSER003", 
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "id": "7007111" 
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "FSDScore": 17,
      "valuationPrice": "870000 - 1099999",
      "value": 1038186,
      "FSDBand": 2,
      "high": 1211041,
      "low": 865331,
      "hasAVM": true
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