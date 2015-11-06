---
category: Web Service Calls
path: '/msg/sendEmailNewCustomer'
title: 'sendEmailNewCustomer'
type: 'GET'

layout: nil
---

# sendEmailNewCustomer

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
		<td>sendEmailNewCustomer</td>
	</tr>
	<tr>
		<td>name</td>
		<td>-</td>
	</tr>
	<tr>
		<td>phone</td>
		<td>-</td>
	</tr>
	<tr>
		<td>email</td>
		<td>-</td>
	</tr>
	<tr>
		<td>date</td>
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
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?uid=TWISTUSER001&op=sendEmailNewCustomer&name=Hohn%20Doe&phone=09153633987&email=john-tooltwist.doe@gmail.com&date=02/02/11&sid=2-4eed242594fc464787b8054ddc77de11
		</td>
	</tr>
</tbody>
</table>
</div>

### Response

Success:
```{
    "response": {
        "status": "success"
    }
}```

Error:
```{
    "response": {
        "status": "error",
        "description": "error description"
    }
}```