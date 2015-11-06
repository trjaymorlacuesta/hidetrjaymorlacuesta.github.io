---
category: Web Service Calls
path: '/msg/getMobileRecentSales'
title: 'getMobileRecentSales'
type: 'GET'

layout: nil
---

# getMobileRecentSales

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
		<td>getMobileRecentSales</td>
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
     		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?uid=TWISTUSER001&op=getMobileRecentSales&suburb=Newtown&state=NSW&postcode=2042&type=house&sid=2-4eed242594fc464787b8054ddc77de11
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
                    "id": 4883563,
                    "lat": -33.90587184,
                    "lon": 151.1770669,
                    "unitNumber": "",
                    "streetNumber": "48",
                    "streetName": "Commodore",
                    "streetType": "Street",
                    "streetDirection": "",
                    "address": "48 Commodore Street",
                    "suburb": "Newtown",
                    "postcode": "2042",
                    "state": "NSW",
                    "bathrooms": 1,
                    "bedrooms": 3,
                    "parking": 2,
                    "landSize": 247,
                    "salePrice": "1361000",
                    "saleDate": "31/10/2015",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "120861161",
                    "agentName": "-",
                    "recentSales": true,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/09/30/26099643/26099643_1.JPG",
                    "ucv": 137000,
                    "ucvDate": "01/07/1997",
                    "realPropertyDescriptor": "PT LOT 38 DP 67532 :PH PETERSHAM",
                    "lgaName": "Marrickville",
                    "lastSaleType": "Unknown",
                    "lotPlan": "38/DP67532 NEWTOWN NSW",
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
                    "id": 4886089,
                    "lat": -33.9009798,
                    "lon": 151.17559964,
                    "unitNumber": "",
                    "streetNumber": "9",
                    "streetName": "Fulham",
                    "streetType": "Street",
                    "streetDirection": "",
                    "address": "9 Fulham Street",
                    "suburb": "Newtown",
                    "postcode": "2042",
                    "state": "NSW",
                    "bathrooms": 1,
                    "bedrooms": 2,
                    "parking": 0,
                    "landSize": 114,
                    "salePrice": "1070000",
                    "saleDate": "31/10/2015",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "120911561",
                    "agentName": "-",
                    "recentSales": true,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/10/06/26123258/26123258_1.JPG",
                    "ucv": 75600,
                    "ucvDate": "01/07/1997",
                    "realPropertyDescriptor": "LOT 1 DP220221",
                    "lgaName": "Marrickville",
                    "lastSaleType": "Unknown",
                    "lotPlan": "1/DP220221 NEWTOWN NSW",
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
                    "id": 17351350,
                    "lat": -33.905426,
                    "lon": 151.17514796,
                    "unitNumber": "",
                    "streetNumber": "29",
                    "streetName": "Laura",
                    "streetType": "Street",
                    "streetDirection": "",
                    "address": "29 Laura Street",
                    "suburb": "Newtown",
                    "postcode": "2042",
                    "state": "NSW",
                    "bathrooms": 1,
                    "bedrooms": 3,
                    "parking": 0,
                    "landSize": 0,
                    "salePrice": "0",
                    "saleDate": "31/10/2015",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "120936865",
                    "agentName": "-",
                    "recentSales": true,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/10/08/26134849/26134849_1.JPG",
                    "ucv": 0,
                    "ucvDate": "",
                    "realPropertyDescriptor": "-",
                    "lgaName": "Marrickville",
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
                    "id": 4896134,
                    "lat": -33.90553247,
                    "lon": 151.17898118,
                    "unitNumber": "",
                    "streetNumber": "49",
                    "streetName": "Wells",
                    "streetType": "Street",
                    "streetDirection": "",
                    "address": "49 Wells Street",
                    "suburb": "Newtown",
                    "postcode": "2042",
                    "state": "NSW",
                    "bathrooms": 1,
                    "bedrooms": 2,
                    "parking": 1,
                    "landSize": 101,
                    "salePrice": "960000",
                    "saleDate": "29/10/2015",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "120902357",
                    "agentName": "-",
                    "recentSales": true,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/10/06/26124505/26124505_1.JPG",
                    "ucv": 14500,
                    "ucvDate": "01/07/1983",
                    "realPropertyDescriptor": "LOT D DP105503",
                    "lgaName": "Marrickville",
                    "lastSaleType": "Unknown",
                    "lotPlan": "D/DP105503 NEWTOWN NSW",
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
                    "id": 4891113,
                    "lat": -33.90472096,
                    "lon": 151.1765293,
                    "unitNumber": "",
                    "streetNumber": "3",
                    "streetName": "Little Commodore",
                    "streetType": "Street",
                    "streetDirection": "",
                    "address": "3 Little Commodore Street",
                    "suburb": "Newtown",
                    "postcode": "2042",
                    "state": "NSW",
                    "bathrooms": 1,
                    "bedrooms": 2,
                    "parking": 0,
                    "landSize": 107,
                    "salePrice": "1000000",
                    "saleDate": "28/10/2015",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "120883757",
                    "agentName": "-",
                    "recentSales": true,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/10/02/26108393/26108393_1.JPG",
                    "ucv": 68700,
                    "ucvDate": "01/07/1997",
                    "realPropertyDescriptor": "LOT 4 DP 232510",
                    "lgaName": "Marrickville",
                    "lastSaleType": "Unknown",
                    "lotPlan": "4/DP232510 NEWTOWN NSW",
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
                    "id": 4896326,
                    "lat": -33.90678689,
                    "lon": 151.17630863,
                    "unitNumber": "",
                    "streetNumber": "112",
                    "streetName": "Wells",
                    "streetType": "Street",
                    "streetDirection": "",
                    "address": "112 Wells Street",
                    "suburb": "Newtown",
                    "postcode": "2042",
                    "state": "NSW",
                    "bathrooms": 2,
                    "bedrooms": 4,
                    "parking": 1,
                    "landSize": 373,
                    "salePrice": "2150000",
                    "saleDate": "24/10/2015",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "120869377",
                    "agentName": "-",
                    "recentSales": true,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/15/09/30/26101437/26101437_1.JPG",
                    "ucv": 151000,
                    "ucvDate": "01/07/1997",
                    "realPropertyDescriptor": "LOT 44 DP111247 S3 :PH PETERSHAM",
                    "lgaName": "Marrickville",
                    "lastSaleType": "Unknown",
                    "lotPlan": "44/3/DP111247 NEWTOWN NSW",
                    "zoning": "Residential",
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