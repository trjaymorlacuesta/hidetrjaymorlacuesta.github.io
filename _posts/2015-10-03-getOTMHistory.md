---
category: Web Service Calls
path: '/msg/getOTMHistory'
title: 'getOTMHistory'
type: 'POST'

layout: nil
---

# getOTMHistory

##Overview
This call is used to fetch the for sale history of a specific property; it uses the BSGv3's property service under forSalePropertyCampaignList node and the BSGv3's for-sale-advertisements. 

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
		<td></td>
	</tr>

</tbody>
</table>

### Additional Information

For further reading regarding BSG Elements: 

* [Property Detail Service](http://confluence.rpdata.local/display/BA/Property+Detail+Service)
* [Property For Sale Advertisements](http://confluence.rpdata.local/display/BA/Property+For+Sale+Advertisements)

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
		<td>maxResult</td>
		<td>Maximum Result</td>
		<td>No</td>
		
	</tr>
</tbody>
</table>

***Sample Request***
```{
    "op": "getOTMHistory",
    "uid": "TWISTUSER001",
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "id": "4890425",
    "maxResult": "5"
}```

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