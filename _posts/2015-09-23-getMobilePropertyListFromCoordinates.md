---
category: Web Service Calls
path: '/msg/getMobilePropertyListFromCoordinates'
title: 'getMobilePropertyListFromCoordinates'
type: 'POST'

layout: nil
---

# getMobilePropertyListFromCoordinates

##Overview
This call is used to fetch all property details within the given radius using BSGv2's Search method. Results can be filtered by the status of the property such as for sale, for rent or sales. 

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
		<td>lon</td>
		<td>Longitude</td>
        <td>Yes</td>
        
	</tr>
	<tr>
		<td>lat</td>
		<td>Latitude</td>
        <td>Yes</td>
        
	</tr>
	<tr>
		<td>radius</td>
		<td>Radius</td>
        <td>Yes</td>
        
	</tr>
	<tr>
		<td>maxResult</td>
		<td>Maximum Result</td>
        <td>Yes</td>
        
	</tr>
	<tr>
		<td>priceMin</td>
		<td>Price Minimum</td>
        <td>No</td>
        
	</tr>
	<tr>
		<td>priceMax</td>
		<td>Price Maximum</td>
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
		<td>floorSize</td>
		<td>Floor Size</td>
        <td>No</td>
        
	</tr>
	<tr>
		<td>capitalValueMax</td>
		<td>Capital Value Maximum</td>
        <td>No</td>
        
	</tr>
	<tr>
		<td>capitalValueMin</td>
		<td>Capital Value Minimum</td>
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
		<td>ignorePastSales</td>
		<td>Ignore Past Sales</td>
        <td>No</td>
        
	</tr>
	<tr>
		<td>recentlySold</td>
		<td>Recently Sold</td>
        <td>No</td>
        
	</tr>
	<tr>
		<td>forSale</td>
		<td>For Sale</td>
        <td>No</td>
        
	</tr>
	<tr>
		<td>other</td>
		<td>Other</td>
        <td>No</td>
        
	</tr>
	<tr>
		<td>forRentOnly</td>
		<td>for Rent Only</td>
        <td>No</td>
        
	</tr>
	<tr>
		<td>displayUnits</td>
		<td>Display Units</td>
        <td>No</td>
        
	</tr>
	<tr>
		<td>street</td>
		<td>Street</td>
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
		<td>isSortedByAddress</td>
		<td>Is Sorted By Address</td>
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
    "op": "getMobilePropertyListFromCoordinates", 
    "uid": "TWISTUSER001", 
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "lat": "-33.89513", 
    "lon": "151.172392", 
    "radius": "0.2", 
    "maxResult": "20"
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "summary": {
        "total": 20,
        "onTheMarket": 3,
        "recentlySold": 7,
        "other": 518,
        "isLastPage": true,
        "forRent": 10
      },
      "pages": {
        "totalPages": 1,
        "currentPage": 1
      },
      "buildings": [
        {
          "streetNumber": "18",
          "streetName": "Gilpin",
          "streetType": "Street",
          "streetDirection": "",
          "address": "18 Gilpin Street",
          "suburb": "Camperdown",
          "postcode": "2050",
          "state": "NSW",
          "id": 16937923,
          "lat": -33.89414741,
          "lon": 151.17317784,
          "onTheMarket": [],
          "recentlySold": [],
          "other": [
            {
              "id": 16937923,
              "unit": "Y",
              "bathrooms": 1,
              "bedrooms": 1,
              "parking": 0,
              "landSize": 0,
              "salePrice": "0",
              "listingPrice": "0",
              "listingDescription": ""
            },
            {
              "id": 17350184,
              "unit": "G",
              "bathrooms": 1,
              "bedrooms": 1,
              "parking": 0,
              "landSize": 0,
              "salePrice": "0",
              "listingPrice": "0",
              "listingDescription": ""
            }
          ]
        },
        {
          "streetNumber": "9",
          "streetName": "Trade",
          "streetType": "Street",
          "streetDirection": "",
          "address": "9 Trade Street",
          "suburb": "Newtown",
          "postcode": "2042",
          "state": "NSW",
          "id": 15539223,
          "lat": -33.89490007,
          "lon": 151.17376122,
          "onTheMarket": [],
          "recentlySold": [
            {
              "id": 4895415,
              "unit": "12",
              "bathrooms": 1,
              "bedrooms": 1,
              "parking": 1,
              "landSize": 696,
              "salePrice": "525000",
              "listingPrice": "0",
              "listingDescription": ""
            }
          ],
          "other": [
            {
              "id": 15539223,
              "unit": "5",
              "bathrooms": 1,
              "bedrooms": 0,
              "parking": 0,
              "landSize": 0,
              "salePrice": "0",
              "listingPrice": "0",
              "listingDescription": ""
            },
            {
              "id": 4895416,
              "unit": "13",
              "bathrooms": 1,
              "bedrooms": 2,
              "parking": 1,
              "landSize": 696,
              "salePrice": "260000",
              "listingPrice": "0",
              "listingDescription": ""
            }
          ]
        },
        {
          "streetNumber": "1",
          "streetName": "Railway",
          "streetType": "Avenue",
          "streetDirection": "",
          "address": "1 Railway Avenue",
          "suburb": "Stanmore",
          "postcode": "2048",
          "state": "NSW",
          "id": 6459180,
          "lat": -33.89494472,
          "lon": 151.17144886,
          "onTheMarket": [],
          "recentlySold": [
            {
              "id": 6459180,
              "unit": "9",
              "bathrooms": 1,
              "bedrooms": 1,
              "parking": 1,
              "landSize": 1492,
              "salePrice": "587500",
              "listingPrice": "0",
              "listingDescription": ""
            },
            {
              "id": 6459218,
              "unit": "27",
              "bathrooms": 2,
              "bedrooms": 2,
              "parking": 1,
              "landSize": 1492,
              "salePrice": "770000",
              "listingPrice": "0",
              "listingDescription": ""
            }
          ],
          "other": [
            {
              "id": 6459211,
              "unit": "24",
              "bathrooms": 0,
              "bedrooms": 2,
              "parking": 0,
              "landSize": 1500,
              "salePrice": "473000",
              "listingPrice": "0",
              "listingDescription": ""
            }
          ]
        },
        {
          "streetNumber": "7",
          "streetName": "Railway",
          "streetType": "Avenue",
          "streetDirection": "",
          "address": "7 Railway Avenue",
          "suburb": "Stanmore",
          "postcode": "2048",
          "state": "NSW",
          "id": 17052385,
          "lat": -33.89498602,
          "lon": 151.17138503,
          "onTheMarket": [],
          "recentlySold": [],
          "other": [
            {
              "id": 17052385,
              "unit": "32",
              "bathrooms": 1,
              "bedrooms": 2,
              "parking": 2,
              "landSize": 0,
              "salePrice": "0",
              "listingPrice": "0",
              "listingDescription": ""
            }
          ]
        }
      ],
      "properties": [
        {
          "type": "House",
          "id": 1701542,
          "lat": -33.8936783,
          "lon": 151.17245475,
          "unitNumber": "",
          "streetNumber": "60",
          "streetName": "Kingston",
          "streetType": "Road",
          "streetDirection": "",
          "address": "60 Kingston Road",
          "suburb": "Camperdown",
          "postcode": "2050",
          "state": "NSW",
          "bathrooms": 2,
          "bedrooms": 3,
          "parking": 1,
          "landSize": 215,
          "salePrice": "620000",
          "saleDate": "18/10/2007",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "rentalListingDate": "23/10/2015",
          "rentalListingPrice": "1100",
          "rentalListingPeriod": "W",
          "REAId": "416577237",
          "agentName": "-",
          "recentSales": false,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/09/02/25980383/25980383_1.JPG",
          "ucv": 116000,
          "ucvDate": "01/07/1997",
          "realPropertyDescriptor": "LOT A DP447292",
          "lgaName": "Marrickville",
          "lastSaleType": "Unknown",
          "distance": 0.2,
          "lotPlan": "A/DP447292 CAMPERDOWN NSW",
          "zoning": "Residential",
          "isAgentAdvised": false,
          "landUsePrimary": "Single Res Dwelling",
          "currentRentalPrice": "",
          "forRent": true,
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
          "id": 1701543,
          "lat": -33.89383496,
          "lon": 151.17185772,
          "unitNumber": "",
          "streetNumber": "61",
          "streetName": "Kingston",
          "streetType": "Road",
          "streetDirection": "",
          "address": "61 Kingston Road",
          "suburb": "Camperdown",
          "postcode": "2050",
          "state": "NSW",
          "bathrooms": 1,
          "bedrooms": 3,
          "parking": 0,
          "landSize": 196,
          "salePrice": "1201000",
          "saleDate": "12/09/2015",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "120505809",
          "agentName": "-",
          "recentSales": true,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/08/18/25915241/25915241_1.JPG",
          "ucv": 88000,
          "ucvDate": "01/07/1997",
          "realPropertyDescriptor": "LOT 9 DP34143",
          "lgaName": "Marrickville",
          "lastSaleType": "Unknown",
          "distance": 0.2,
          "lotPlan": "9/DP34143 CAMPERDOWN NSW",
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
          "type": "House",
          "id": 2254992,
          "lat": -33.89619097,
          "lon": 151.17192371,
          "unitNumber": "",
          "streetNumber": "49",
          "streetName": "Gladstone",
          "streetType": "Street",
          "streetDirection": "",
          "address": "49 Gladstone Street",
          "suburb": "Enmore",
          "postcode": "2042",
          "state": "NSW",
          "bathrooms": 1,
          "bedrooms": 2,
          "parking": 0,
          "landSize": 95,
          "salePrice": "470000",
          "saleDate": "30/10/2006",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "rentalListingDate": "05/11/2015",
          "rentalListingPrice": "670",
          "rentalListingPeriod": "W",
          "REAId": "416883670",
          "agentName": "-",
          "recentSales": false,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/10/15/26174363/26174363_1.JPG",
          "ucv": 68700,
          "ucvDate": "01/07/1997",
          "realPropertyDescriptor": "LOT 1 DP202541",
          "lgaName": "Marrickville",
          "lastSaleType": "Unknown",
          "distance": 0.2,
          "lotPlan": "1/DP202541 ENMORE NSW",
          "zoning": "Residential",
          "isAgentAdvised": false,
          "landUsePrimary": "Single Res Dwelling",
          "currentRentalPrice": "",
          "forRent": true,
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
          "id": 2255541,
          "lat": -33.89662892,
          "lon": 151.17309901,
          "unitNumber": "",
          "streetNumber": "56",
          "streetName": "Phillip",
          "streetType": "Street",
          "streetDirection": "",
          "address": "56 Phillip Street",
          "suburb": "Enmore",
          "postcode": "2042",
          "state": "NSW",
          "bathrooms": 1,
          "bedrooms": 2,
          "parking": 0,
          "landSize": 115,
          "salePrice": "157000",
          "saleDate": "26/03/1996",
          "onTheMarket": true,
          "listingDate": "08/11/2015",
          "listingPrice": "0",
          "listingDescription": "Auction",
          "REAId": "121135718",
          "agentName": "-",
          "recentSales": false,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/10/29/26237168/26237168_1.JPG",
          "ucv": 45000,
          "ucvDate": "01/07/1994",
          "realPropertyDescriptor": "LOT 1 DP212224 :PH PETERSHAM",
          "lgaName": "Marrickville",
          "lastSaleType": "Unknown",
          "distance": 0.2,
          "lotPlan": "1/DP212224 ENMORE NSW",
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
          "id": 2255773,
          "lat": -33.8961071,
          "lon": 151.1723208,
          "unitNumber": "",
          "streetNumber": "35-39",
          "streetName": "Trafalgar",
          "streetType": "Street",
          "streetDirection": "",
          "address": "35-39 Trafalgar Street",
          "suburb": "Enmore",
          "postcode": "2042",
          "state": "NSW",
          "bathrooms": 2,
          "bedrooms": 3,
          "parking": 1,
          "landSize": 917,
          "salePrice": "0",
          "saleDate": "10/07/2015",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "119345987",
          "agentName": "-",
          "recentSales": true,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/03/18/25295356/25295356_1.JPG",
          "ucv": 264000,
          "ucvDate": "01/07/1997",
          "realPropertyDescriptor": "LOTS 16-23 DP1747",
          "lgaName": "Marrickville",
          "lastSaleType": "Unknown",
          "distance": 0.2,
          "lotPlan": "16/DP1747 ENMORE NSW",
          "zoning": "Residential",
          "isAgentAdvised": true,
          "landUsePrimary": "General Industrial",
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
          "id": 17292104,
          "lat": -33.89604302,
          "lon": 151.17198296,
          "unitNumber": "",
          "streetNumber": "39B",
          "streetName": "Trafalgar",
          "streetType": "Street",
          "streetDirection": "",
          "address": "39B Trafalgar Street",
          "suburb": "Enmore",
          "postcode": "2042",
          "state": "NSW",
          "bathrooms": 2,
          "bedrooms": 3,
          "parking": 1,
          "landSize": 0,
          "salePrice": "0",
          "saleDate": "",
          "onTheMarket": false,
          "listingDate": "19/09/2015",
          "listingPrice": "1400000",
          "listingDescription": "Offers over $1,400,000",
          "rentalListingDate": "05/11/2015",
          "rentalListingPrice": "1150",
          "rentalListingPeriod": "W",
          "REAId": "417038070",
          "agentName": "-",
          "recentSales": false,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/11/05/26270973/26270973_1.JPG",
          "ucv": 0,
          "ucvDate": "",
          "realPropertyDescriptor": "-",
          "lgaName": "Marrickville",
          "lastSaleType": "",
          "distance": 0.2,
          "lotPlan": "",
          "zoning": "",
          "isAgentAdvised": false,
          "landUsePrimary": "",
          "currentRentalPrice": "",
          "forRent": true,
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
          "id": 17258581,
          "lat": -33.89604302,
          "lon": 151.17198296,
          "unitNumber": "",
          "streetNumber": "39A",
          "streetName": "Trafalgar",
          "streetType": "Street",
          "streetDirection": "",
          "address": "39A Trafalgar Street",
          "suburb": "Enmore",
          "postcode": "2042",
          "state": "NSW",
          "bathrooms": 2,
          "bedrooms": 3,
          "parking": 1,
          "landSize": 0,
          "salePrice": "1407500",
          "saleDate": "22/07/2015",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "rentalListingDate": "10/11/2015",
          "rentalListingPrice": "900",
          "rentalListingPeriod": "W",
          "REAId": "417002794",
          "agentName": "-",
          "recentSales": true,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/11/02/26248788/26248788_1.JPG",
          "ucv": 0,
          "ucvDate": "",
          "realPropertyDescriptor": "-",
          "lgaName": "Marrickville",
          "lastSaleType": "Unknown",
          "distance": 0.2,
          "lotPlan": "",
          "zoning": "",
          "isAgentAdvised": true,
          "landUsePrimary": "",
          "currentRentalPrice": "",
          "forRent": true,
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
          "listingDate": "08/11/2015",
          "listingPrice": "1365000",
          "listingDescription": "for sale - $1,365,000",
          "REAId": "120922385",
          "agentName": "-",
          "recentSales": false,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/10/07/26128001/26128001_1.JPG",
          "ucv": 79700,
          "ucvDate": "01/07/1997",
          "realPropertyDescriptor": "LOT 6 DP108105",
          "lgaName": "Marrickville",
          "lastSaleType": "Unknown",
          "distance": 0.2,
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
          "bedrooms": 2,
          "parking": 0,
          "landSize": 121,
          "salePrice": "320000",
          "saleDate": "27/05/1999",
          "onTheMarket": true,
          "listingDate": "08/11/2015",
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
          "distance": 0.2,
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
        },
        {
          "type": "House",
          "id": 4894821,
          "lat": -33.89454681,
          "lon": 151.17387623,
          "unitNumber": "",
          "streetNumber": "83",
          "streetName": "St Marys",
          "streetType": "Street",
          "streetDirection": "",
          "address": "83 St Marys Street",
          "suburb": "Newtown",
          "postcode": "2042",
          "state": "NSW",
          "bathrooms": 3,
          "bedrooms": 3,
          "parking": 1,
          "landSize": 234,
          "salePrice": "2170000",
          "saleDate": "21/08/2015",
          "onTheMarket": false,
          "listingDate": "",
          "listingPrice": "0",
          "listingDescription": "",
          "REAId": "120035937",
          "agentName": "-",
          "recentSales": true,
          "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/06/17/25653511/25653511_1.JPG",
          "ucv": 137000,
          "ucvDate": "01/07/1997",
          "realPropertyDescriptor": "LOT 1 DP81374",
          "lgaName": "Marrickville",
          "lastSaleType": "Unknown",
          "distance": 0.2,
          "lotPlan": "1/DP81374 NEWTOWN NSW",
          "zoning": "Residential",
          "isAgentAdvised": true,
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