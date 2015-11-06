---
category: Web Service Calls
path: '/msg/getOTMHistory'
title: 'getOTMHistory'
type: 'GET'

layout: nil
---

# getOTMHistory

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
		<td>getOTMHistory</td>
	</tr>
	<tr>
		<td>id</td>
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
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?uid=TWISTUSER003&op=getOTMHistory&id=4890425&maxResult=5&sid=2-4eed242594fc464787b8054ddc77de11
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
            "listings": [
                {
                    "latestListedPrice": 0,
                    "latestListedPriceDescription": "PRICE GUIDE OVER $975,000",
                    "latestListDate": "12/12/2010",
                    "listingTypeDescription": "Auction",
                    "daysListed": 20,
                    "agencyName": "Mcgrath - Leichhardt",
                    "agentName": "Kate Webster"
                },
                {
                    "latestListedPrice": 345000,
                    "latestListedPriceDescription": "",
                    "latestListDate": "07/06/1997",
                    "listingTypeDescription": "Normal Sale",
                    "daysListed": 1,
                    "agencyName": "Raine & Horne N'Town",
                    "agentName": ""
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