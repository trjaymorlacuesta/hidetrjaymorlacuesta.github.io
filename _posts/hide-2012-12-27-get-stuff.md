---
category: Stuff
path: '/stuff'
title: 'Get stuff'
type: 'GET'

layout: nil

exercises: [Burpees, Squats, Pull ups, Push ups]
reps: [50, 40, 30, 20, 10]
---

This method allows users to retrieve stuff.

### Request

* The headers must include a **valid authentication token**.

### Response

Sends back a collection of things.

```Status: 200 OK```
```{
    {
        id: thing_1,
        name: 'My first thing'
    },
    {
        id: thing_2,
        name: 'My second thing'
    }
}```

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
</tbody>
</table>




For errors responses, see the [response status codes documentation](#response-status-codes).