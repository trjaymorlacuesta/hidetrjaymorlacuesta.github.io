---
category: Web Service Calls
path: '/msg/getMobilePropertyListForSuburb'
title: 'getMobilePropertyListForSuburb'
type: 'GET'

layout: nil
---

# getMobilePropertyListForSuburb

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
		<td>Yes</td>
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
		<td>getMobilePropertyListForSuburb</td>
	</tr>
	<tr>
		<td>postcode</td>
		<td>-</td>
	</tr>
	<tr>
		<td>suburb</td>
		<td>-</td>
	</tr>
	<tr>
		<td>state</td>
		<td>-</td>
	</tr>
	<tr>
		<td>maxResult</td>
		<td>-</td>
	</tr>
	<tr>
		<td>priceMin</td>
		<td>-</td>
	</tr>
	<tr>
		<td>priceMax</td>
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
		<td>floorSize</td>
		<td>-</td>
	</tr>
	<tr>
		<td>capitalValueMin</td>
		<td>-</td>
	</tr>
	<tr>
		<td>capitalValueMax</td>
		<td>-</td>
	</tr>
	<tr>
		<td>start</td>
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
		<td>land</td>
		<td>-</td>
	</tr>
	<tr>
		<td>commercial</td>
		<td>-</td>
	</tr>
	<tr>
		<td>others</td>
		<td>-</td>
	</tr>
	<tr>
		<td>recentlySold</td>
		<td>-</td>
	</tr>
	<tr>
		<td>forSale</td>
		<td>-</td>
	</tr>
	<tr>
		<td>other</td>
		<td>-</td>
	</tr>
	<tr>
		<td>forRentOnly</td>
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
		<td>pageNumber</td>
		<td>-</td>
	</tr>
	<tr>
		<td>pageSize</td>
		<td>-</td>
	</tr>
	<tr>
		<td>isSortedByAddress</td>
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
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?uid=TWISTUSER001&op=getMobilePropertyListForSuburb&state=NSW&suburb=NEWTOWN&postcode=2042&maxResult=5&start=1&house=true&unit=true&recentlySold=true&forSale=true&other=true&landSize=0&bedrooms=0&bathrooms=0&sid=2-4eed242594fc464787b8054ddc77de11
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
                "total": 7662,
                "onTheMarket": 30,
                "recentlySold": 161,
                "other": 7320,
                "isLastPage": false,
                "forRent": 151
            },
            "pages": {
                "totalPages": 1533,
                "currentPage": 1
            },
            "buildings": [ ],
            "properties": [
                {
                    "type": "House",
                    "id": 4879567,
                    "lat": -33.8960781,
                    "lon": 151.17397436,
                    "unitNumber": "",
                    "streetNumber": "101",
                    "streetName": "Albermarle",
                    "streetType": "Street",
                    "streetDirection": "",
                    "address": "101 Albermarle Street",
                    "suburb": "Newtown",
                    "postcode": "2042",
                    "state": "NSW",
                    "bathrooms": 1,
                    "bedrooms": 3,
                    "parking": 1,
                    "landSize": 108,
                    "salePrice": "800000",
                    "saleDate": "20/10/2009",
                    "onTheMarket": true,
                    "listingDate": "02/11/2015",
                    "listingPrice": "0",
                    "listingDescription": "for sale - price on request",
                    "REAId": "120922385",
                    "agentName": "-",
                    "recentSales": false,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/10/07/26128001/26128001_1.JPG",
                    "ucv": 79700,
                    "ucvDate": "01/07/1997",
                    "realPropertyDescriptor": "LOT 6 DP108105",
                    "lgaName": "Marrickville",
                    "lastSaleType": "Unknown",
                    "lotPlan": "6/DP108105 NEWTOWN NSW",
                    "zoning": "Residential",
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
                },
                {
                    "type": "House",
                    "id": 4879807,
                    "lat": -33.9031052,
                    "lon": 151.17795527,
                    "unitNumber": "",
                    "streetNumber": "33",
                    "streetName": "Alice",
                    "streetType": "Street",
                    "streetDirection": "",
                    "address": "33 Alice Street",
                    "suburb": "Newtown",
                    "postcode": "2042",
                    "state": "NSW",
                    "bathrooms": 1,
                    "bedrooms": 3,
                    "parking": 0,
                    "landSize": 188,
                    "salePrice": "63000",
                    "saleDate": "07/05/1986",
                    "onTheMarket": true,
                    "listingDate": "01/11/2015",
                    "listingPrice": "0",
                    "listingDescription": "auction",
                    "REAId": "120979698",
                    "agentName": "-",
                    "recentSales": false,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/10/13/26154571/26154571_1.JPG",
                    "ucv": 82500,
                    "ucvDate": "01/07/1997",
                    "realPropertyDescriptor": "LOT 5 DP 200090",
                    "lgaName": "Marrickville",
                    "lastSaleType": "Unknown",
                    "lotPlan": "5/DP200090 NEWTOWN NSW",
                    "zoning": "Residential",
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
                },
                {
                    "type": "House",
                    "id": 4880325,
                    "lat": -33.90459885,
                    "lon": 151.17384184,
                    "unitNumber": "",
                    "streetNumber": "181",
                    "streetName": "Alice",
                    "streetType": "Street",
                    "streetDirection": "",
                    "address": "181 Alice Street",
                    "suburb": "Newtown",
                    "postcode": "2042",
                    "state": "NSW",
                    "bathrooms": 2,
                    "bedrooms": 4,
                    "parking": 2,
                    "landSize": 143,
                    "salePrice": "453000",
                    "saleDate": "16/08/2000",
                    "onTheMarket": true,
                    "listingDate": "30/10/2015",
                    "listingPrice": "0",
                    "listingDescription": "Expressions Of Interest",
                    "REAId": "",
                    "agentName": "-",
                    "recentSales": false,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/10/04/26116905/26116905_1.JPG",
                    "ucv": 79700,
                    "ucvDate": "01/07/1997",
                    "realPropertyDescriptor": "LOT B DP 107528",
                    "lgaName": "Marrickville",
                    "lastSaleType": "Unknown",
                    "lotPlan": "B/DP107528 NEWTOWN NSW",
                    "zoning": "Residential",
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
                },
                {
                    "type": "House",
                    "id": 4880475,
                    "lat": -33.90170103,
                    "lon": 151.18013781,
                    "unitNumber": "",
                    "streetNumber": "88",
                    "streetName": "Angel",
                    "streetType": "Street",
                    "streetDirection": "",
                    "address": "88 Angel Street",
                    "suburb": "Newtown",
                    "postcode": "2042",
                    "state": "NSW",
                    "bathrooms": 2,
                    "bedrooms": 3,
                    "parking": 1,
                    "landSize": 500,
                    "salePrice": "1025000",
                    "saleDate": "09/02/2005",
                    "onTheMarket": true,
                    "listingDate": "23/10/2015",
                    "listingPrice": "0",
                    "listingDescription": "POA",
                    "REAId": "118534859",
                    "agentName": "-",
                    "recentSales": false,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/14/11/20/24848096/24848096_1.JPG",
                    "ucv": 195000,
                    "ucvDate": "01/01/1930",
                    "realPropertyDescriptor": "LOT 1 DP1147071",
                    "lgaName": "Sydney",
                    "lastSaleType": "Unknown",
                    "lotPlan": "2/DP456893 NEWTOWN NSW",
                    "zoning": "Residential",
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
                },
                {
                    "type": "House",
                    "id": 4880927,
                    "lat": -33.89538037,
                    "lon": 151.17421721,
                    "unitNumber": "",
                    "streetNumber": "41",
                    "streetName": "Baltic",
                    "streetType": "Street",
                    "streetDirection": "",
                    "address": "41 Baltic Street",
                    "suburb": "Newtown",
                    "postcode": "2042",
                    "state": "NSW",
                    "bathrooms": 1,
                    "bedrooms": 3,
                    "parking": 0,
                    "landSize": 121,
                    "salePrice": "320000",
                    "saleDate": "27/05/1999",
                    "onTheMarket": true,
                    "listingDate": "01/11/2015",
                    "listingPrice": "0",
                    "listingDescription": "Auction",
                    "REAId": "121113930",
                    "agentName": "-",
                    "recentSales": false,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/10/27/26223392/26223392_1.JPG",
                    "ucv": 82500,
                    "ucvDate": "01/07/1997",
                    "realPropertyDescriptor": "LOT 2 DP 110260",
                    "lgaName": "Marrickville",
                    "lastSaleType": "Unknown",
                    "lotPlan": "2/DP110260 NEWTOWN NSW",
                    "zoning": "Residential",
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