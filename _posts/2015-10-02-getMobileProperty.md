---
category: Web Service Calls
path: '/msg/getMobileProperty'
title: 'getMobileProperty'
type: 'POST'

layout: nil
---

# getMobileProperty

##Overview
This call is used to fetch all property details of the given  search string, it can be full address search, street, suburb or postcode; it uses BSGv2's Search method. Results can be filtered by the status of the property such as for sale, for rent or sales. 

When the showAdditionalDataElements is true, it will use the BSGv3's property service to show the additional fields that aren't available on BSGv2.

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
		<td>searchString</td>
		<td>Search String</td>
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
		<td>No</td>
		
	</tr>
	<tr>
		<td>house</td>
		<td>Having House Property Type</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>unit</td>
		<td>Having Unit Property Type</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>commercial</td>
		<td>Commercial</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>land</td>
		<td>Land</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>others</td>
		<td>Others</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>listedDays</td>
		<td>Listed Days</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>soldDays</td>
		<td>Sold Days</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>bedrooms</td>
		<td>Number of Bedrooms</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>bathrooms</td>
		<td>Number of Bathrooms</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>parking</td>
		<td>Parking</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>landSize</td>
		<td>Land Size</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>forSale</td>
		<td>For Sale</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>recentlySold</td>
		<td>Recently Sold</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>forRentOnly</td>
		<td>For RentOnly</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>other</td>
		<td>Other</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>appCode</td>
		<td>App Code</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>pageNumber</td>
		<td>Page Number</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>pageSize</td>
		<td>Page Size</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>groupUnits</td>
		<td>Group Units</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>showAdditionalDataElements</td>
		<td>Show Additional Data Elements</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>sortBy</td>
		<td>Sort By</td>
		<td>No</td>
		
	</tr>
	<tr>
		<td>sortOrder</td>
		<td>Sort Order</td>
		<td>No</td>
		
	</tr>
</tbody>
</table>

***Sample Request***
```{
    "op": "GetMobileProperty", 
    "uid": "TWISTUSER010", 
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "searchString": "24 Nundah Street Lane Cove North NSW 2066", 
    "maxResult": "10", 
    "category": "1"
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "summary": {
        "total": 1,
        "onTheMarket": 0,
        "recentlySold": 0,
        "other": 1,
        "isLastPage": true,
        "forRent": 0
      },
      "pages": {
        "totalPages": 1,
        "currentPage": 1
      },
      "buildings": [],
      "properties": [
        {
          "type": "House",
          "id": 3604024,
          "lat": -33.81068809,
          "lon": 151.1710076,
          "unitNumber": "",
          "streetNumber": "24",
          "streetName": "Nundah",
          "streetType": "Street",
          "streetDirection": "",
          "address": "24 Nundah Street",
          "suburb": "Lane Cove North",
          "postcode": "2066",
          "state": "NSW",
          "bathrooms": 2,
          "bedrooms": 4,
          "parking": 2,
          "landSize": 560,
          "salePrice": "1500000",
          "saleDate": "24/03/2010",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "",
          "agentName": "-",
          "recentSales": false,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/10/03/10/17026141/17026141_1.JPG",
          "ucv": 194000,
          "ucvDate": "01/07/1995",
          "realPropertyDescriptor": "LOT 7 DP7817 SEC 8",
          "lgaName": "Lane Cove",
          "lastSaleType": "Unknown",
          "lotPlan": "7/8/DP7817 LANE COVE NORTH NSW",
          "zoning": "",
          "isAgentAdvised": false,
          "landUsePrimary": "Single Res Dwelling",
          "currentRentalPrice": "",
          "forRent": false,
          "forRentDaysOnMarket": 0,
          "forRentAgencyName": "",
          "occupancyType": "",
          "volume": "",
          "folio": "",
          "mapReference": "",
          "block": "",
          "section": ""
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