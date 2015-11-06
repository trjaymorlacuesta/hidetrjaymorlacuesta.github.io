---
category: Web Service Calls
path: '/msg/getMobileRentalAvmPdf'
title: 'getMobileRentalAvmPdf'
type: 'GET'

layout: nil
---

# getMobileRentalAvmPdf

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
		<td>getMobileRentalAvmPdf</td>
	</tr>
	<tr>
		<td>propertyId</td>
		<td>-</td>
	</tr>
	<tr>
		<td>prepareForFirstName</td>
		<td>-</td>
	</tr>
	<tr>
		<td>prepareForLastName</td>
		<td>-</td>
	</tr>
	<tr>
		<td>prepareByFirstName</td>
		<td>-</td>
	</tr>
	<tr>
		<td>prepareByLastName</td>
		<td>-</td>
	</tr>
	<tr>
		<td>prepareByPhone</td>
		<td>-</td>
	</tr>
	<tr>
		<td>prepareByEmail</td>
		<td>-</td>
	</tr>
</tbody>
</table>

### Response

Success:
```{
    "response": {
        "status": "success",
        "result": {
            "results": "Results"
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