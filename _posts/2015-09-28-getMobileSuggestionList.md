---
category: Web Service Calls
path: '/msg/getMobileSuggestionList'
title: 'getMobileSuggestionList'
type: 'POST'

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

### Additional Information

For further reading regarding BSG Elements: 

* [Method_getSuggestionList](http://confluence.rpdata.local/display/BA/Method_getSuggestionList)

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

***Sample Request***
```{
    "op": "getMobileSuggestionList", 
    "uid": "8C5830F0-816A-54C5-9271-8F06AD36CE2D", 
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "suggestion": "carlton", 
    "category": "1", 
    "maxResult": "20"
}```

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