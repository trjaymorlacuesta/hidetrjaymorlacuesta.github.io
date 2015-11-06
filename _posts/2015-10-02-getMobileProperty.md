---
category: Web Service Calls
path: '/msg/getMobileProperty'
title: 'getMobileProperty'
type: 'GET'

layout: nil
---

# getMobileProperty

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
		<td>getMobileProperty</td>
	</tr>
	<tr>
		<td>searchString</td>
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
	<tr>
		<td>house</td>
		<td>-</td>
	</tr>
	<tr>
		<td>unit</td>
		<td>-</td>
	</tr>
	<tr>
		<td>commercial</td>
		<td>-</td>
	</tr>
	<tr>
		<td>land</td>
		<td>-</td>
	</tr>
	<tr>
		<td>others</td>
		<td>-</td>
	</tr>
	<tr>
		<td>listedDays</td>
		<td>-</td>
	</tr>
	<tr>
		<td>soldDays</td>
		<td>-</td>
	</tr>
	<tr>
		<td>bedrooms</td>
		<td>-</td>
	</tr>
	<tr>
		<td>bathrooms</td>
		<td>-</td>
	</tr>
	<tr>
		<td>parking</td>
		<td>-</td>
	</tr>
	<tr>
		<td>landSize</td>
		<td>-</td>
	</tr>
	<tr>
		<td>forSale</td>
		<td>-</td>
	</tr>
	<tr>
		<td>recentlySold</td>
		<td>-</td>
	</tr>
	<tr>
		<td>forRentOnly</td>
		<td>-</td>
	</tr>
	<tr>
		<td>other</td>
		<td>-</td>
	</tr>
	<tr>
		<td>appCode</td>
		<td>-</td>
	</tr>
	<tr>
		<td>pageNumber</td>
		<td>-</td>
	</tr>
	<tr>
		<td>pageSize</td>
		<td>-</td>
	</tr>
	<tr>
		<td>groupUnits</td>
		<td>-</td>
	</tr>
	<tr>
		<td>showAdditionalDataElements</td>
		<td>-</td>
	</tr>
	<tr>
		<td>sortBy</td>
		<td>-</td>
	</tr>
	<tr>
		<td>sortOrder</td>
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
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?uid=TWISTUSER010&op=GetMobileProperty&searchString=24%20Nundah%20Street%20Lane%20Cove%20North%20NSW%202066&maxResult=10&category=1&sid=2-4eed242594fc464787b8054ddc77de11
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
            "buildings": [ ],
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