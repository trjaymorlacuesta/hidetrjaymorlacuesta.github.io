---
category: Web Service Calls
path: '/msg/getMobilePropertyListForName'
title: 'getMobilePropertyListForName'
type: 'GET'

layout: nil
---

# getMobilePropertyListForName

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
		<td>getMobilePropertyListForName</td>
	</tr>
	<tr>
		<td>firstName</td>
		<td>-</td>
	</tr>
	<tr>
		<td>lastName</td>
		<td>-</td>
	</tr>
	<tr>
		<td>suburb</td>
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
</tbody>
</table>

<div id="msgtesturl">
<table>
	<tbody>
	<tr>
		<th>Test URL MSG Agent -MSGSIT:</th>
	</tr>
	<tr>
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?uid=bsguser.rpmob3.bberry1&sid=2-4eed242594fc464787b8054ddc77de11&ac=rpm&op=getMobilePropertyListForName&firstName=&lastName=smith&suburb=Turramurra&pageNumber=1&pageSize=10
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
                "total": 28,
                "onTheMarket": 0,
                "recentlySold": 0,
                "other": 10,
                "isLastPage": false
            },
            "pages": {
                "totalPages": 3,
                "currentPage": 1
            },
            "properties": [
                {
                    "type": "House",
                    "id": 6997931,
                    "lat": -33.72047209,
                    "lon": 151.13479898,
                    "unitNumber": "",
                    "streetNumber": "25",
                    "streetName": "Alice",
                    "streetType": "Street",
                    "streetDirection": "",
                    "address": "25 Alice Street",
                    "suburb": "Turramurra",
                    "postcode": "2074",
                    "state": "NSW",
                    "bathrooms": 0,
                    "bedrooms": 0,
                    "parking": 0,
                    "landSize": 987,
                    "salePrice": "530000",
                    "saleDate": "25/10/1994",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "",
                    "agentName": "-",
                    "recentSales": false,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/04/07/19/NSW00925A/286.JPG",
                    "ucv": 0,
                    "ucvDate": "",
                    "realPropertyDescriptor": "LOT 332 DP 543770",
                    "lgaName": "Ku-Ring-Gai",
                    "lastSaleType": "Unknown",
                    "ownerNames": [
                        "SMITH, MICHAEL GRAEME",
                        "SMITH, JULIE ELIZABETH"
                    ],
                    "lotPlan": "332/DP543770 TURRAMURRA NSW",
                    "zoning": "Residential",
                    "isAgentAdvised": false,
                    "landUsePrimary": "",
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
                    "id": 6998575,
                    "lat": -33.73097529,
                    "lon": 151.13880611,
                    "unitNumber": "",
                    "streetNumber": "79",
                    "streetName": "Bobbin Head",
                    "streetType": "Road",
                    "streetDirection": "",
                    "address": "79 Bobbin Head Road",
                    "suburb": "Turramurra",
                    "postcode": "2074",
                    "state": "NSW",
                    "bathrooms": 0,
                    "bedrooms": 0,
                    "parking": 0,
                    "landSize": 1038,
                    "salePrice": "0",
                    "saleDate": "",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "",
                    "agentName": "-",
                    "recentSales": false,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/04/07/19/NSW00925C/133.JPG",
                    "ucv": 0,
                    "ucvDate": "",
                    "realPropertyDescriptor": "LOT 5 DP191370",
                    "lgaName": "Ku-Ring-Gai",
                    "lastSaleType": "",
                    "ownerNames": [
                        "SMITH, N L",
                        "SMITH, D A"
                    ],
                    "lotPlan": "5/DP191370 TURRAMURRA NSW",
                    "zoning": "Residential",
                    "isAgentAdvised": false,
                    "landUsePrimary": "",
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
                    "id": 6998608,
                    "lat": -33.72976227,
                    "lon": 151.13894814,
                    "unitNumber": "",
                    "streetNumber": "93",
                    "streetName": "Bobbin Head",
                    "streetType": "Road",
                    "streetDirection": "",
                    "address": "93 Bobbin Head Road",
                    "suburb": "Turramurra",
                    "postcode": "2074",
                    "state": "NSW",
                    "bathrooms": 3,
                    "bedrooms": 5,
                    "parking": 2,
                    "landSize": 836,
                    "salePrice": "1260000",
                    "saleDate": "10/12/2011",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "108636241",
                    "agentName": "-",
                    "recentSales": false,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/11/11/11/19876320/19876320_1.JPG",
                    "ucv": 0,
                    "ucvDate": "",
                    "realPropertyDescriptor": "LOT B2 DP310410",
                    "lgaName": "Ku-Ring-Gai",
                    "lastSaleType": "Unknown",
                    "ownerNames": [
                        "BOTTOMLEY, -",
                        "SMITH, -"
                    ],
                    "lotPlan": "B2/DP310410 TURRAMURRA NSW",
                    "zoning": "Residential",
                    "isAgentAdvised": false,
                    "landUsePrimary": "",
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
                    "id": 6998764,
                    "lat": -33.72250523,
                    "lon": 151.14078629,
                    "unitNumber": "",
                    "streetNumber": "159",
                    "streetName": "Bobbin Head",
                    "streetType": "Road",
                    "streetDirection": "",
                    "address": "159 Bobbin Head Road",
                    "suburb": "Turramurra",
                    "postcode": "2074",
                    "state": "NSW",
                    "bathrooms": 0,
                    "bedrooms": 0,
                    "parking": 0,
                    "landSize": 906,
                    "salePrice": "8230",
                    "saleDate": "31/05/1957",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "",
                    "agentName": "-",
                    "recentSales": false,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/04/07/19/NSW00925C/248.JPG",
                    "ucv": 0,
                    "ucvDate": "",
                    "realPropertyDescriptor": "LOT 28 DP 36328.",
                    "lgaName": "Ku-Ring-Gai",
                    "lastSaleType": "Unknown",
                    "ownerNames": [
                        "SMITH, KEITH BATHURST",
                        "SMITH, RAE"
                    ],
                    "lotPlan": "28/DP36328 TURRAMURRA NSW",
                    "zoning": "Residential",
                    "isAgentAdvised": false,
                    "landUsePrimary": "",
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
                    "id": 5053567,
                    "lat": 0,
                    "lon": 0,
                    "unitNumber": "62",
                    "streetNumber": "381",
                    "streetName": "Bobbin Head",
                    "streetType": "Road",
                    "streetDirection": "",
                    "address": "62/381 Bobbin Head Road",
                    "suburb": "Turramurra",
                    "postcode": "2074",
                    "state": "NSW",
                    "bathrooms": 0,
                    "bedrooms": 0,
                    "parking": 0,
                    "landSize": 0,
                    "salePrice": "738000",
                    "saleDate": "20/08/2014",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "",
                    "agentName": "-",
                    "recentSales": false,
                    "photo": "",
                    "ucv": 0,
                    "ucvDate": "",
                    "realPropertyDescriptor": "LOT 62 SP54427",
                    "lgaName": "Ku-Ring-Gai",
                    "lastSaleType": "Unknown",
                    "ownerNames": [
                        "SMITH, -"
                    ],
                    "lotPlan": "62/SP54427 TURRAMURRA NSW",
                    "zoning": "Residential",
                    "isAgentAdvised": false,
                    "landUsePrimary": "",
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
                    "id": 6999039,
                    "lat": -33.74111418,
                    "lon": 151.12018405,
                    "unitNumber": "",
                    "streetNumber": "12",
                    "streetName": "Boronia",
                    "streetType": "Avenue",
                    "streetDirection": "",
                    "address": "12 Boronia Avenue",
                    "suburb": "Turramurra",
                    "postcode": "2074",
                    "state": "NSW",
                    "bathrooms": 0,
                    "bedrooms": 0,
                    "parking": 0,
                    "landSize": 886,
                    "salePrice": "0",
                    "saleDate": "",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "",
                    "agentName": "-",
                    "recentSales": false,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/04/07/19/NSW00925F/408.JPG",
                    "ucv": 0,
                    "ucvDate": "",
                    "realPropertyDescriptor": "LOT 19 DP12795 :PH GORDON",
                    "lgaName": "Ku-Ring-Gai",
                    "lastSaleType": "",
                    "ownerNames": [
                        "SMITH, SHIRLEY CLARE"
                    ],
                    "lotPlan": "19/DP12795 TURRAMURRA NSW",
                    "zoning": "Residential",
                    "isAgentAdvised": false,
                    "landUsePrimary": "",
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
                    "id": 6999352,
                    "lat": -33.71932968,
                    "lon": 151.14108086,
                    "unitNumber": "",
                    "streetNumber": "170",
                    "streetName": "Burns",
                    "streetType": "Road",
                    "streetDirection": "",
                    "address": "170 Burns Road",
                    "suburb": "Turramurra",
                    "postcode": "2074",
                    "state": "NSW",
                    "bathrooms": 3,
                    "bedrooms": 4,
                    "parking": 2,
                    "landSize": 1100,
                    "salePrice": "1600000",
                    "saleDate": "22/04/2014",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "116326875",
                    "agentName": "-",
                    "recentSales": false,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/14/03/06/23728257/23728257_1.JPG",
                    "ucv": 0,
                    "ucvDate": "",
                    "realPropertyDescriptor": "LOT 7 DP30833",
                    "lgaName": "Ku-Ring-Gai",
                    "lastSaleType": "Unknown",
                    "ownerNames": [
                        "SMITH, -"
                    ],
                    "lotPlan": "7/DP30833 TURRAMURRA NSW",
                    "zoning": "Residential",
                    "isAgentAdvised": false,
                    "landUsePrimary": "",
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
                    "id": 6999427,
                    "lat": -33.72545017,
                    "lon": 151.14052611,
                    "unitNumber": "",
                    "streetNumber": "6",
                    "streetName": "Canberra",
                    "streetType": "Avenue",
                    "streetDirection": "",
                    "address": "6 Canberra Avenue",
                    "suburb": "Turramurra",
                    "postcode": "2074",
                    "state": "NSW",
                    "bathrooms": 3,
                    "bedrooms": 4,
                    "parking": 2,
                    "landSize": 1619,
                    "salePrice": "1200000",
                    "saleDate": "13/07/2005",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "",
                    "agentName": "-",
                    "recentSales": false,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/05/07/11/9513593/9513593_1.JPG",
                    "ucv": 0,
                    "ucvDate": "",
                    "realPropertyDescriptor": "LOT 61 DP1084866",
                    "lgaName": "Ku-Ring-Gai",
                    "lastSaleType": "Unknown",
                    "ownerNames": [
                        "BERRY, -",
                        "SMITH, -"
                    ],
                    "lotPlan": "61/DP1084866 TURRAMURRA NSW",
                    "zoning": "Residential",
                    "isAgentAdvised": false,
                    "landUsePrimary": "",
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
                    "id": 6999452,
                    "lat": -33.7474904,
                    "lon": 151.11996759,
                    "unitNumber": "",
                    "streetNumber": "5",
                    "streetName": "Carina",
                    "streetType": "Road",
                    "streetDirection": "",
                    "address": "5 Carina Road",
                    "suburb": "Turramurra",
                    "postcode": "2074",
                    "state": "NSW",
                    "bathrooms": 1,
                    "bedrooms": 3,
                    "parking": 1,
                    "landSize": 962,
                    "salePrice": "0",
                    "saleDate": "",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "",
                    "agentName": "-",
                    "recentSales": false,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/04/07/19/NSW00925F/71.JPG",
                    "ucv": 0,
                    "ucvDate": "",
                    "realPropertyDescriptor": "LOT 62 DP28082 :PH GORDON",
                    "lgaName": "Ku-Ring-Gai",
                    "lastSaleType": "",
                    "ownerNames": [
                        "SMITH, GRAEME WILLIAM",
                        "RAPPORT, MARINA FRANCES"
                    ],
                    "lotPlan": "62/DP28082 TURRAMURRA NSW",
                    "zoning": "Residential",
                    "isAgentAdvised": false,
                    "landUsePrimary": "",
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
                    "id": 6999762,
                    "lat": -33.72919674,
                    "lon": 151.14599916,
                    "unitNumber": "",
                    "streetNumber": "6",
                    "streetName": "Charlton",
                    "streetType": "Avenue",
                    "streetDirection": "",
                    "address": "6 Charlton Avenue",
                    "suburb": "Turramurra",
                    "postcode": "2074",
                    "state": "NSW",
                    "bathrooms": 2,
                    "bedrooms": 4,
                    "parking": 2,
                    "landSize": 1069,
                    "salePrice": "1300000",
                    "saleDate": "30/08/2006",
                    "onTheMarket": false,
                    "listingDate": "",
                    "listingPrice": "0",
                    "listingDescription": "",
                    "REAId": "",
                    "agentName": "-",
                    "recentSales": false,
                    "photo": "https://static.rpdata.com/rpdaAU/photo/listsale/120x80/06/08/19/11000231/11000231_1.JPG",
                    "ucv": 0,
                    "ucvDate": "",
                    "realPropertyDescriptor": "LOT 4 DP734952",
                    "lgaName": "Ku-Ring-Gai",
                    "lastSaleType": "Unknown",
                    "ownerNames": [
                        "SMITH, -"
                    ],
                    "lotPlan": "4/DP734952 TURRAMURRA NSW",
                    "zoning": "Residential",
                    "isAgentAdvised": false,
                    "landUsePrimary": "",
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