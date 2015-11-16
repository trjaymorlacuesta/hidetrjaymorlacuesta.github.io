---
category: Web Service Calls
path: '/msg/getMobileComparableSales'
title: 'getMobileComparableSales'
type: 'POST'

layout: nil
---

# getMobileComparableSales

##Overview
This call is used to obtain summary statistics and/or detailed property information for properties considered to be comparable to a target property; it uses BSGv2's comparable service

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
		<td>suburb</td>
		<td>Suburb</td>
    <td>Yes</td>
          
	</tr>
	<tr>
		<td>state</td>
		<td>State</td>
    <td>Yes</td>
          
	</tr>
	<tr>
		<td>postcode</td>
		<td>Postcode</td>
    <td>Yes</td>
          
	</tr>
	<tr>
		<td>maxResult</td>
		<td>MaxResult</td>
    <td>No</td>
          
	</tr>
	<tr>
		<td>type</td>
		<td>Property Type</td>
    <td>Yes</td>
          
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
		<td>showAdditionalDataElements</td>
		<td>Show Additional Data Elements</td>
    <td>No</td>
          
	</tr>
</tbody>
</table>

***Sample Request***
```{
    "op": "getMobileComparableSales", 
    "uid": "TWISTUSER003", 
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "suburb": "Chatswood", 
    "state": "NSW", 
    "postcode": "2067", 
    "bedrooms": "3", 
    "bathrooms": "2", 
    "type": "house"
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "buildings": [],
      "properties": [
        {
          "type": "House",
          "id": 1823762,
          "lat": -33.80623277,
          "lon": 151.1726318,
          "unitNumber": "",
          "streetNumber": "12",
          "streetName": "Beaconsfield",
          "streetType": "Road",
          "streetDirection": "",
          "address": "12 Beaconsfield Road",
          "suburb": "Chatswood",
          "postcode": "2067",
          "state": "NSW",
          "bathrooms": 2,
          "bedrooms": 3,
          "parking": 4,
          "landSize": 966,
          "salePrice": "1880000",
          "saleDate": "04/11/2015",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "120973738",
          "agentName": "-",
          "recentSales": true,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/10/13/26153918/26153918_1.JPG",
          "ucv": 225000,
          "ucvDate": "01/07/1990",
          "realPropertyDescriptor": "LOT A DP339468 :PH WILLOUGHBY",
          "lgaName": "Willoughby",
          "lastSaleType": "Unknown",
          "lotPlan": "A/DP339468 CHATSWOOD NSW",
          "zoning": "Non Urban",
          "isAgentAdvised": true,
          "landUsePrimary": "Single Res Dwelling",
          "forRent": false,
          "volume": "",
          "folio": "",
          "mapReference": "",
          "block": "",
          "section": ""
        },
        {
          "type": "House",
          "id": 1828239,
          "lat": -33.79600731,
          "lon": 151.17700828,
          "unitNumber": "1",
          "streetNumber": "27",
          "streetName": "James",
          "streetType": "Street",
          "streetDirection": "",
          "address": "1/27 James Street",
          "suburb": "Chatswood",
          "postcode": "2067",
          "state": "NSW",
          "bathrooms": 2,
          "bedrooms": 3,
          "parking": 2,
          "landSize": 262,
          "salePrice": "0",
          "saleDate": "03/11/2015",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "121017086",
          "agentName": "-",
          "recentSales": true,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/10/16/26176065/26176065_1.JPG",
          "ucv": 0,
          "ucvDate": "",
          "realPropertyDescriptor": "LOT 100 DP1044003",
          "lgaName": "Willoughby",
          "lastSaleType": "Unknown",
          "lotPlan": "100/DP1044003 CHATSWOOD NSW",
          "zoning": "Residential",
          "isAgentAdvised": true,
          "landUsePrimary": "Single Res Dwelling",
          "forRent": false,
          "volume": "",
          "folio": "",
          "mapReference": "",
          "block": "",
          "section": ""
        },
        {
          "type": "House",
          "id": 1833552,
          "lat": -33.79522822,
          "lon": 151.1775018,
          "unitNumber": "",
          "streetNumber": "5",
          "streetName": "View",
          "streetType": "Street",
          "streetDirection": "",
          "address": "5 View Street",
          "suburb": "Chatswood",
          "postcode": "2067",
          "state": "NSW",
          "bathrooms": 2,
          "bedrooms": 3,
          "parking": 2,
          "landSize": 770,
          "salePrice": "0",
          "saleDate": "18/09/2015",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "120221229",
          "agentName": "-",
          "recentSales": true,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/07/11/25760435/25760435_1.JPG",
          "ucv": 380000,
          "ucvDate": "01/07/1990",
          "realPropertyDescriptor": "LOT 11 DP3435 & LOT 1 DP928773",
          "lgaName": "Willoughby",
          "lastSaleType": "Unknown",
          "lotPlan": "11/DP3435 CHATSWOOD NSW",
          "zoning": "National Parks",
          "isAgentAdvised": true,
          "landUsePrimary": "Park/Garden/Cemetry",
          "forRent": false,
          "volume": "",
          "folio": "",
          "mapReference": "",
          "block": "",
          "section": ""
        },
        {
          "type": "House",
          "id": 17291439,
          "lat": 0,
          "lon": 0,
          "unitNumber": "",
          "streetNumber": "22",
          "streetName": "Wyvern",
          "streetType": "Avenue",
          "streetDirection": "",
          "address": "22 Wyvern Avenue",
          "suburb": "Chatswood",
          "postcode": "2067",
          "state": "NSW",
          "bathrooms": 2,
          "bedrooms": 3,
          "parking": 2,
          "landSize": 574,
          "salePrice": "1815000",
          "saleDate": "16/09/2015",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "120511697",
          "agentName": "-",
          "recentSales": true,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/08/19/25920123/25920123_1.JPG",
          "ucv": 0,
          "ucvDate": "",
          "realPropertyDescriptor": "LOT 1 DP1199483",
          "lgaName": "Willoughby",
          "lastSaleType": "Unknown",
          "lotPlan": "1/DP1199483 CHATSWOOD NSW",
          "zoning": "",
          "isAgentAdvised": false,
          "landUsePrimary": "Single Res Dwelling",
          "forRent": false,
          "volume": "",
          "folio": "",
          "mapReference": "",
          "block": "",
          "section": ""
        },
        {
          "type": "House",
          "id": 1834031,
          "lat": -33.79019467,
          "lon": 151.17780929,
          "unitNumber": "",
          "streetNumber": "22A",
          "streetName": "Wyvern",
          "streetType": "Avenue",
          "streetDirection": "",
          "address": "22A Wyvern Avenue",
          "suburb": "Chatswood",
          "postcode": "2067",
          "state": "NSW",
          "bathrooms": 2,
          "bedrooms": 3,
          "parking": 4,
          "landSize": 983,
          "salePrice": "1525000",
          "saleDate": "16/09/2015",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "416982442",
          "agentName": "-",
          "recentSales": true,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/10/29/26235300/26235300_1.JPG",
          "ucv": 347000,
          "ucvDate": "01/01/1930",
          "realPropertyDescriptor": "LOT 1 DP1064926",
          "lgaName": "Willoughby",
          "lastSaleType": "Unknown",
          "lotPlan": "1/DP1064926 CHATSWOOD NSW",
          "zoning": "Residential",
          "isAgentAdvised": true,
          "landUsePrimary": "Single Res Dwelling",
          "forRent": false,
          "volume": "",
          "folio": "",
          "mapReference": "",
          "block": "",
          "section": ""
        },
        {
          "type": "House",
          "id": 1823226,
          "lat": -33.7925974,
          "lon": 151.17664377,
          "unitNumber": "",
          "streetNumber": "32",
          "streetName": "Anglo",
          "streetType": "Street",
          "streetDirection": "",
          "address": "32 Anglo Street",
          "suburb": "Chatswood",
          "postcode": "2067",
          "state": "NSW",
          "bathrooms": 2,
          "bedrooms": 3,
          "parking": 1,
          "landSize": 930,
          "salePrice": "2400000",
          "saleDate": "09/09/2015",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "120522841",
          "agentName": "-",
          "recentSales": true,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/08/20/25926071/25926071_1.JPG",
          "ucv": 230000,
          "ucvDate": "01/07/1990",
          "realPropertyDescriptor": "LOT A DP355703 :PH WILLOUGHBY",
          "lgaName": "Willoughby",
          "lastSaleType": "Unknown",
          "lotPlan": "A/DP355703 CHATSWOOD NSW",
          "zoning": "Non Urban",
          "isAgentAdvised": true,
          "landUsePrimary": "Single Res Dwelling",
          "forRent": false,
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