---
category: Web Service Calls
path: '/msg/getMobileSuggestionList'
title: 'getMobileSuggestionList'
type: 'GET'

layout: nil
---

# getMobileSuggestionList

##Overview
This call is used to fetch suggestion list that matches the search term; it uses suggest service under BSGv2.

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

### Request

* The headers must include a **valid authentication token**.

<table>
	<tbody>
	<tr>
		<th>Parameter</th>
		<th>Description</th>
		<th>Required</th>
		
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
		<td>op</td>
		<td>Operation</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>suggestion</td>
		<td>Suggestion Keyword</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>category</td>
		<td>Category</td>
		<td>Yes</td>
		
	</tr>
	<tr>
		<td>maxResult</td>
		<td>Maximum Result</td>
		<td>Yes</td>
		
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