---
category: Web Service Calls
path: '/msg/getMobilePropertyTimeline'
title: 'getMobilePropertyTimeline'
type: 'POST'

layout: nil
---

# getMobilePropertyTimeline

##Overview
This call is used to fetch the timeline of a particular property.

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
		<td>propertyId</td>
		<td>Property Id</td>
        <td>Yes</td>
        
	</tr>
</tbody>
</table>

***Sample Request***
```{
    "op": "getMobilePropertyTimeline",
    "uid": "TWISTUSER001",
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "propertyId": "7823011"
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "yearBuild": "1975",
      "propertyTimeLine": [
        {
          "listingType": "Sold",
          "listingMethod": "",
          "listingDate": "22/04/2014",
          "daysOnMarket": "",
          "agentName": "",
          "agentContact": "",
          "agencyName": "Mcgrath Gosford - Wyoming",
          "priceDescription": "Sold for $370,000",
          "period": "",
          "vendorList": [
            {
              "id": "24098154",
              "person": {
                "firstName": "",
                "middleNames": "",
                "initials": "",
                "lastName": "Mawby-Wilkinson"
              },
              "company": {
                "companyName": "",
                "abn": "",
                "acn": ""
              },
              "mailingAddress": {
                "careOf": "",
                "line1": "24 MAYA ST",
                "line2": "WYOMING NSW",
                "suburb": "",
                "state": "",
                "postcode": "2250",
                "country": "",
                "doNotMail": false
              }
            }
          ]
        },
        {
          "listingType": "For Sale",
          "listingMethod": "Normal Sale",
          "listingDate": "02/04/2014",
          "daysOnMarket": "21",
          "agentName": "Steve Farthing",
          "agentContact": "0418 436 666",
          "agencyName": "Mcgrath Gosford - Wyoming",
          "priceDescription": "OVER $360,000",
          "period": "",
          "vendorList": []
        },
        {
          "listingType": "Sold",
          "listingMethod": "",
          "listingDate": "30/07/2011",
          "daysOnMarket": "",
          "agentName": "",
          "agentContact": "",
          "agencyName": "L J Hooker Gosford",
          "priceDescription": "Sold for $340,000",
          "period": "",
          "vendorList": [
            {
              "id": "24143078",
              "person": {
                "firstName": "",
                "middleNames": "",
                "initials": "",
                "lastName": "Latif"
              },
              "company": {
                "companyName": "",
                "abn": "",
                "acn": ""
              },
              "mailingAddress": {
                "careOf": "",
                "line1": "24 MAYA ST",
                "line2": "WYOMING NSW",
                "suburb": "",
                "state": "",
                "postcode": "2250",
                "country": "",
                "doNotMail": false
              }
            }
          ]
        },
        {
          "listingType": "For Sale",
          "listingMethod": "Auction",
          "listingDate": "30/06/2011",
          "daysOnMarket": "31",
          "agentName": "Garry Morris",
          "agentContact": "0408 438 651",
          "agencyName": "L J Hooker Gosford",
          "priceDescription": "Not Disclosed",
          "period": "",
          "vendorList": []
        },
        {
          "listingType": "For Sale",
          "listingMethod": "Normal Sale",
          "listingDate": "25/11/2010",
          "daysOnMarket": "7",
          "agentName": "Kariong'S No.1 Real Estate Team",
          "agentContact": "4340 2424",
          "agencyName": "George Brand Real Estate Kariong",
          "priceDescription": "$395,000",
          "period": "",
          "vendorList": []
        },
        {
          "listingType": "Sold",
          "listingMethod": "",
          "listingDate": "13/08/2001",
          "daysOnMarket": "",
          "agentName": "",
          "agentContact": "",
          "agencyName": "",
          "priceDescription": "Sold for $267,500",
          "period": "",
          "vendorList": [
            {
              "id": "24084752",
              "person": {
                "firstName": "",
                "middleNames": "",
                "initials": "",
                "lastName": "Price"
              },
              "company": {
                "companyName": "",
                "abn": "",
                "acn": ""
              },
              "mailingAddress": {
                "careOf": "",
                "line1": "24 MAYA ST",
                "line2": "WYOMING NSW",
                "suburb": "",
                "state": "",
                "postcode": "2250",
                "country": "",
                "doNotMail": false
              }
            }
          ]
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