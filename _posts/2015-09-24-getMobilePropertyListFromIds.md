---
category: Web Service Calls
path: '/msg/getMobilePropertyListFromIds'
title: 'getMobilePropertyListFromIds'
type: 'POST'

layout: nil
---

# getMobilePropertyListFromIds

##Overview
This call is used to fetch all property details of the given property ids, it uses BSGv2's Search method. Results can be filtered by the status of the property such as for sale, for rent or sales. 

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
		<td>ids</td>
		<td>Property IDs</td>
          <td>Yes</td>
          
	</tr>
	<tr>
		<td>showAdditionalDataElements</td>
		<td>Show Additional DataElements</td>
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
    "op": "getMobilePropertyListFromIds", 
    "uid": "TWISTUSER001", 
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "ids": "[7007111,7007124,7007137,7007145,7007153,7007157,7007165,7007173,7007180,7007188,7007196]"
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "summary": {
        "total": 11,
        "onTheMarket": 0,
        "recentlySold": 0,
        "other": 11,
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
          "type": "Unit",
          "id": 7007124,
          "lat": -33.73263023,
          "lon": 151.1312403,
          "unitNumber": "4",
          "streetNumber": "1",
          "streetName": "Turramurra",
          "streetType": "Avenue",
          "streetDirection": "",
          "address": "4/1 Turramurra Avenue",
          "suburb": "Turramurra",
          "postcode": "2074",
          "state": "NSW",
          "bathrooms": 2,
          "bedrooms": 4,
          "parking": 2,
          "landSize": 1464,
          "salePrice": "950000",
          "saleDate": "10/11/2006",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "",
          "agentName": "-",
          "recentSales": false,
          "ucv": 0,
          "ucvDate": "",
          "realPropertyDescriptor": "LOT 4 SP75729",
          "lgaName": "Ku-Ring-Gai",
          "lastSaleType": "Unknown",
          "lotPlan": "4/SP75729 TURRAMURRA NSW",
          "zoning": "Residential",
          "isAgentAdvised": false,
          "landUsePrimary": "Residential Strata Units",
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
          "type": "Unit",
          "id": 7007111,
          "lat": -33.73262757,
          "lon": 151.13124165,
          "unitNumber": "",
          "streetNumber": "1",
          "streetName": "Turramurra",
          "streetType": "Avenue",
          "streetDirection": "",
          "address": "1 Turramurra Avenue",
          "suburb": "Turramurra",
          "postcode": "2074",
          "state": "NSW",
          "bathrooms": 2,
          "bedrooms": 3,
          "parking": 2,
          "landSize": 0,
          "salePrice": "1600000",
          "saleDate": "20/09/2002",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "",
          "agentName": "-",
          "recentSales": false,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/06/10/31/mapnsw/586/595/0058595586",
          "ucv": 0,
          "ucvDate": "",
          "realPropertyDescriptor": "SP75729",
          "lgaName": "Ku-Ring-Gai",
          "lastSaleType": "Unknown",
          "lotPlan": "",
          "zoning": "Residential",
          "isAgentAdvised": false,
          "landUsePrimary": "Residential Strata Units",
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
          "id": 7007137,
          "lat": -33.73187852,
          "lon": 151.13142776,
          "unitNumber": "",
          "streetNumber": "7-11",
          "streetName": "Turramurra",
          "streetType": "Avenue",
          "streetDirection": "",
          "address": "7-11 Turramurra Avenue",
          "suburb": "Turramurra",
          "postcode": "2074",
          "state": "NSW",
          "bathrooms": 1,
          "bedrooms": 3,
          "parking": 0,
          "landSize": 906,
          "salePrice": "1733333",
          "saleDate": "19/01/2009",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "106843873",
          "agentName": "-",
          "recentSales": false,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/13/03/05/22082791/22082791_1.JPG",
          "ucv": 0,
          "ucvDate": "",
          "realPropertyDescriptor": "LOT 456 DP1149960",
          "lgaName": "Ku-Ring-Gai",
          "lastSaleType": "Unknown",
          "lotPlan": "456/DP1149960 TURRAMURRA NSW",
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
          "id": 7007145,
          "lat": -33.73169368,
          "lon": 151.1314327,
          "unitNumber": "",
          "streetNumber": "11",
          "streetName": "Turramurra",
          "streetType": "Avenue",
          "streetDirection": "",
          "address": "11 Turramurra Avenue",
          "suburb": "Turramurra",
          "postcode": "2074",
          "state": "NSW",
          "bathrooms": 1,
          "bedrooms": 3,
          "parking": 1,
          "landSize": 911,
          "salePrice": "1733333",
          "saleDate": "19/01/2009",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "106843843",
          "agentName": "-",
          "recentSales": false,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/10/09/19/17901208/17901208_1.JPG",
          "ucv": 0,
          "ucvDate": "",
          "realPropertyDescriptor": "LOT 4 DP6353",
          "lgaName": "Ku-Ring-Gai",
          "lastSaleType": "Unknown",
          "lotPlan": "4/DP6353 TURRAMURRA NSW",
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
          "type": "Land",
          "id": 7007153,
          "lat": -33.73092505,
          "lon": 151.13158757,
          "unitNumber": "",
          "streetNumber": "15",
          "streetName": "Turramurra",
          "streetType": "Avenue",
          "streetDirection": "",
          "address": "15 Turramurra Avenue",
          "suburb": "Turramurra",
          "postcode": "2074",
          "state": "NSW",
          "bathrooms": 0,
          "bedrooms": 0,
          "parking": 0,
          "landSize": 1515,
          "salePrice": "0",
          "saleDate": "",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "",
          "agentName": "-",
          "recentSales": false,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/13/08/30/22878515/22878515_1.JPG",
          "ucv": 0,
          "ucvDate": "",
          "realPropertyDescriptor": "LOT 1 DP587965 :PH GORDON",
          "lgaName": "Ku-Ring-Gai",
          "lastSaleType": "",
          "lotPlan": "1/DP587965 TURRAMURRA NSW",
          "zoning": "Undetermined Or Village",
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
          "id": 7007157,
          "lat": -33.73070364,
          "lon": 151.13173598,
          "unitNumber": "",
          "streetNumber": "17",
          "streetName": "Turramurra",
          "streetType": "Avenue",
          "streetDirection": "",
          "address": "17 Turramurra Avenue",
          "suburb": "Turramurra",
          "postcode": "2074",
          "state": "NSW",
          "bathrooms": 2,
          "bedrooms": 3,
          "parking": 2,
          "landSize": 1454,
          "salePrice": "3500000",
          "saleDate": "04/09/2014",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "118598611",
          "agentName": "-",
          "recentSales": false,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/14/11/27/24876484/24876484_1.JPG",
          "ucv": 0,
          "ucvDate": "",
          "realPropertyDescriptor": "LOT 8 DP21174",
          "lgaName": "Ku-Ring-Gai",
          "lastSaleType": "Unknown",
          "lotPlan": "8/DP21174 TURRAMURRA NSW",
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
        },
        {
          "type": "Unit",
          "id": 7007165,
          "lat": -33.73088686,
          "lon": 151.1308125,
          "unitNumber": "5",
          "streetNumber": "20",
          "streetName": "Turramurra",
          "streetType": "Avenue",
          "streetDirection": "",
          "address": "5/20 Turramurra Avenue",
          "suburb": "Turramurra",
          "postcode": "2074",
          "state": "NSW",
          "bathrooms": 2,
          "bedrooms": 3,
          "parking": 4,
          "landSize": 822,
          "salePrice": "1849945",
          "saleDate": "23/11/2007",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "106557853",
          "agentName": "-",
          "recentSales": false,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/10/05/22/17379897/17379897_1.JPG",
          "ucv": 0,
          "ucvDate": "",
          "realPropertyDescriptor": "LOT 5 DP510186",
          "lgaName": "Ku-Ring-Gai",
          "lastSaleType": "Unknown",
          "lotPlan": "5/DP510186 TURRAMURRA NSW",
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
          "id": 7007173,
          "lat": -33.72983721,
          "lon": 151.13160436,
          "unitNumber": "",
          "streetNumber": "23",
          "streetName": "Turramurra",
          "streetType": "Avenue",
          "streetDirection": "",
          "address": "23 Turramurra Avenue",
          "suburb": "Turramurra",
          "postcode": "2074",
          "state": "NSW",
          "bathrooms": 3,
          "bedrooms": 5,
          "parking": 2,
          "landSize": 1100,
          "salePrice": "860000",
          "saleDate": "12/04/2001",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "409794959",
          "agentName": "-",
          "recentSales": false,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/13/02/14/22000448/22000448_1.JPG",
          "ucv": 0,
          "ucvDate": "",
          "realPropertyDescriptor": "LOT A DP398976 :PH GORDON",
          "lgaName": "Ku-Ring-Gai",
          "lastSaleType": "Unknown",
          "lotPlan": "A/DP398976 TURRAMURRA NSW",
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
          "type": "Unit",
          "id": 7007180,
          "lat": -33.73013163,
          "lon": 151.1310427,
          "unitNumber": "4",
          "streetNumber": "28",
          "streetName": "Turramurra",
          "streetType": "Avenue",
          "streetDirection": "",
          "address": "4/28 Turramurra Avenue",
          "suburb": "Turramurra",
          "postcode": "2074",
          "state": "NSW",
          "bathrooms": 3,
          "bedrooms": 3,
          "parking": 2,
          "landSize": 753,
          "salePrice": "1693035",
          "saleDate": "23/11/2007",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "106120194",
          "agentName": "-",
          "recentSales": false,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/09/11/06/16554835/16554835_1.JPG",
          "ucv": 0,
          "ucvDate": "",
          "realPropertyDescriptor": "LOT 4 DP11993",
          "lgaName": "Ku-Ring-Gai",
          "lastSaleType": "Unknown",
          "lotPlan": "4/DP11993 TURRAMURRA NSW",
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
          "id": 7007188,
          "lat": -33.72956972,
          "lon": 151.13186535,
          "unitNumber": "",
          "streetNumber": "33",
          "streetName": "Turramurra",
          "streetType": "Avenue",
          "streetDirection": "",
          "address": "33 Turramurra Avenue",
          "suburb": "Turramurra",
          "postcode": "2074",
          "state": "NSW",
          "bathrooms": 2,
          "bedrooms": 3,
          "parking": 1,
          "landSize": 1102,
          "salePrice": "0",
          "saleDate": "",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "",
          "agentName": "-",
          "recentSales": false,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/07/04/30/11996308/11996308_1.JPG",
          "ucv": 0,
          "ucvDate": "",
          "realPropertyDescriptor": "LOT 4 DP18870 :PH GORDON",
          "lgaName": "Ku-Ring-Gai",
          "lastSaleType": "",
          "lotPlan": "4/DP18870 TURRAMURRA NSW",
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
          "id": 7007196,
          "lat": -33.72939619,
          "lon": 151.13109549,
          "unitNumber": "",
          "streetNumber": "36",
          "streetName": "Turramurra",
          "streetType": "Avenue",
          "streetDirection": "",
          "address": "36 Turramurra Avenue",
          "suburb": "Turramurra",
          "postcode": "2074",
          "state": "NSW",
          "bathrooms": 0,
          "bedrooms": 0,
          "parking": 0,
          "landSize": 960,
          "salePrice": "390000",
          "saleDate": "01/12/1994",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "",
          "agentName": "-",
          "recentSales": false,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/04/07/19/NSW00925A/491.JPG",
          "ucv": 0,
          "ucvDate": "",
          "realPropertyDescriptor": "LOT B DP 348843 SUBJECT TO DRAINAGE EASEMENT",
          "lgaName": "Ku-Ring-Gai",
          "lastSaleType": "Unknown",
          "lotPlan": "B/DP348843 TURRAMURRA NSW",
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