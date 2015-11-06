---
category: Web Service Calls
path: '/msg/getMobileSuggestionList'
title: 'getMobileSuggestionList'
type: 'GET'

layout: nil
---

# getMobileSuggestionList

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
		<td>getMobileSuggestionList</td>
	</tr>
	<tr>
		<td>suggestion</td>
		<td>-</td>
	</tr>
	<tr>
		<td>category</td>
		<td>-</td>
	</tr>
	<tr>
		<td>maxResult</td>
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
			<td>http://msgsit.rpdata.com/ttsvr/msgdebug?op=getMobileSuggestionList&uid=8C5830F0-816A-54C5-9271-8F06AD36CE2D&suggestion=carlton&category=1&maxResult=20&sid=2-4eed242594fc464787b8054ddc77de11
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
            "suggestionList": [
                {
                    "suburb": "Carlton Street Newcastle",
                    "state": "NSW",
                    "postcode": "2300"
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