---
category: Web Service Calls
path: '/msg/getMobileComparableSales'
title: 'getMobileComparableSales'
type: 'GET'

layout: nil
---

# getMobileComparableSales

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
		<td>getMobileComparableSales</td>
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
		<td>postcode</td>
		<td>-</td>
	</tr>
	<tr>
		<td>maxResult</td>
		<td>-</td>
	</tr>
	<tr>
		<td>type</td>
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
		<td>showAdditionalDataElements</td>
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
     		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?uid=TWISTUSER003&op=getMobileComparableSales&suburb=Chatswood&state=NSW&postcode=2067&bedrooms=3&bathrooms=2&type=house&sid=2-4eed242594fc464787b8054ddc77de11
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
            "buildings": [ ],
            "properties": [
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
                    "lat": -33.78989511,
                    "lon": 151.17795859,
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
                    "landSize": 0,
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
                    "realPropertyDescriptor": "-",
                    "lgaName": "Willoughby",
                    "lastSaleType": "Unknown",
                    "lotPlan": "",
                    "zoning": "",
                    "isAgentAdvised": true,
                    "landUsePrimary": "",
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
                },
                {
                    "type": "House",
                    "id": 1825300,
                    "lat": -33.7917744,
                    "lon": 151.19214115,
                    "unitNumber": "",
                    "streetNumber": "20",
                    "streetName": "Crick",
                    "streetType": "Street",
                    "streetDirection": "",
                    "address": "20 Crick Street",
                    "suburb": "Chatswood",
                    "postcode": "2067",
                    "state": "NSW",
                    "bathrooms": 2,
                    "bedrooms": 3,
                    "parking": 1,
                    "landSize": 346,
                    "salePrice": "1695000",
                    "saleDate": "29/08/2015",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "120418489",
                    "agentName": "-",
                    "recentSales": true,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/08/06/25870211/25870211_1.JPG",
                    "ucv": 234000,
                    "ucvDate": "01/01/1930",
                    "realPropertyDescriptor": "LOT 1 DP576713",
                    "lgaName": "Willoughby",
                    "lastSaleType": "Unknown",
                    "lotPlan": "1/DP576713 CHATSWOOD NSW",
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
                    "id": 1828224,
                    "lat": -33.79714565,
                    "lon": 151.17676453,
                    "unitNumber": "",
                    "streetNumber": "14",
                    "streetName": "James",
                    "streetType": "Street",
                    "streetDirection": "",
                    "address": "14 James Street",
                    "suburb": "Chatswood",
                    "postcode": "2067",
                    "state": "NSW",
                    "bathrooms": 2,
                    "bedrooms": 3,
                    "parking": 2,
                    "landSize": 512,
                    "salePrice": "0",
                    "saleDate": "14/08/2015",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "120405129",
                    "agentName": "-",
                    "recentSales": true,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/08/05/25861863/25861863_1.JPG",
                    "ucv": 175000,
                    "ucvDate": "01/07/1990",
                    "realPropertyDescriptor": "LOT 2 DP115611 :PH WILLOUGHBY",
                    "lgaName": "Willoughby",
                    "lastSaleType": "Unknown",
                    "lotPlan": "2/DP115611 CHATSWOOD NSW",
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