---
category: Web Service Calls
path: '/msg/getMobileAvm'
title: 'getMobileAvm'
type: 'POST'

layout: nil
---

# getMobileAvm

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
		<td>Yes</td>
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
* [Method_getPropertySummaryList](http://confluence.rpdata.local/display/BA/Method_getPropertySummaryList)
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
</tbody>
</table>

***Sample Request***
```{
    "op": "getmobileavm", 
    "uid": "TWISTUSER003", 
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "id": "7003499"
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "fsdScore": 8,
      "value": 1798976,
      "high": 1937281,
      "low": 1660672,
      "salePrice": "",
      "saleDate": "",
      "propertyList": []
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