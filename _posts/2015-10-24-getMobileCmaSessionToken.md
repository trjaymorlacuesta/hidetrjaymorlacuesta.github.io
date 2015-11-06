---
category: Web Service Calls
path: '/msg/getMobileCmaSessionToken'
title: 'getMobileCmaSessionToken'
type: 'GET'

layout: nil
---

# getMobileCmaSessionToken

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
		<td>-</td>
		<td>-</td>
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
		<td>getMobileCmaSessionToken</td>
	</tr>
	<tr>
		<td>page</td>
		<td>-</td>
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
		<td>https://msgsit.rpdata.com/ttsvr/msgdebug?uid=TWISTUSER003&sid=2-4eed242594fc464787b8054ddc77de11&op=getMobileCmaSessionToken&username=bsguser.vivant&password=RNPgN5bx&appCode=rppipad&page=8&propertyId=3604024
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
            "sessionToken": "https://rpp.rpdata.com/rpp/flow/avm.html?src=test&timestamp=2015-11-03T16:28:36+10:00&token=2-4eed242594fc464787b8054ddc77de11&apiKey=a95607eba0d92ffdee24b3b13d2c1e899b868000&hash=65c585c6feb682215f7752400fd59f3da9565b96"
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