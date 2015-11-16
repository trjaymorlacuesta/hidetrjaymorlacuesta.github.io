---
category: Web Service Calls
path: '/msg/getMobileComparableProperties'
title: 'getMobileComparableProperties'
type: 'POST'

layout: nil
---

# getMobileComparableProperties

##Overview
This call is used to obtain summary statistics and/or detailed property information for properties considered to be comparable to a target property; it uses BSGv3's comparable service

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
        <td>Optional</td>
        
	</tr>
	<tr>
		<td>latitude</td>
		<td>Latitude</td>
        <td>Yes if propertyId is Null</td>
        
	</tr>
	<tr>
		<td>longitude</td>
		<td>Longitude</td>
        <td>Yes if propertyId is Null</td>
        
	</tr>
	<tr>
		<td>targetPropertyBedrooms</td>
		<td>Target Property Bedrooms</td>
        <td>Yes if propertyId is Null</td>
        
	</tr>
	<tr>
		<td>targetPropertyBathrooms</td>
		<td>Target Property Bathrooms</td>
        <td>Yes if propertyId is Null</td>
        
	</tr>
	<tr>
		<td>targetPropertyLandArea</td>
		<td>Target Property Land Area</td>
        <td>Yes if propertyId is Null</td>
        
	</tr>
	<tr>
		<td>targetPropertyPropertyType</td>
		<td>Property Type of the Target Property</td>
        <td>Yes if propertyId is Null</td>
        
	</tr>
	<tr>
		<td>targetPropertyCarSpaces</td>
		<td>Target Property CarS paces</td>
        <td>Yes if propertyId is Null</td>
        
	</tr>
	<tr>
		<td>limit</td>
		<td>Limit of List to Display</td>
        <td>No</td>
        
	</tr>
	<tr>
		<td>comparableRuleId</td>
		<td>Comparable Rule Id</td>
        <td>Yes</td>
        
	</tr>
	<tr>
		<td>returnStatisticsForComparableCategoryId</td>
		<td>Return Statistics For Comparable Category Id</td>
        <td>No</td>
        
	</tr>
	<tr>
		<td>returnDetailForComparableCategoryId</td>
		<td>Return Detail For Comparable Category Id</td>
        <td>No</td>
        
	</tr>
	<tr>
		<td>returnFields</td>
		<td>Return Fields</td>
        <td>No</td>
        
	</tr>
</tbody>
</table>

***Sample Request***
```{
    "op": "getMobileComparableProperties",
    "uid": "TWISTUSER001",
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "limit": 1, 
    "comparableRuleId": 3, 
    "propertyId": "3971426"
}```

### Response

Success:
```{
  "response": {
    "status": "success",
    "result": {
      "comparableSummaryLists": [
        {
          "averageForRentListingPrice": "468",
          "maximumForRentCampaignDate": "09/11/2015",
          "maximumForRentListingPrice": "480",
          "medianForRentListingPrice": "465",
          "minimumForRentCampaignDate": "02/11/2015",
          "minimumForRentListingPrice": "460",
          "comparableCategoryId": "2",
          "comparableCategory": "GOOD",
          "totalProperties": "3",
          "propertyComparableList": [
            {
              "propertyDetail": {
                "distanceFromTarget": "0.9747291985776219",
                "address": {
                  "buildingComplexName": "",
                  "councilArea": "Moreton Bay Regional - Pine Rivers",
                  "singleLine": "7 Marigold Street Margate QLD 4019",
                  "unitNumber": "",
                  "unitAlpha": "",
                  "derivedUnit": false,
                  "startNumber": "7",
                  "startAlpha": "",
                  "endNumber": "",
                  "endAlpha": "",
                  "street": {
                    "id": "2564374",
                    "singleLine": "Marigold Street Margate QLD 4019",
                    "name": "MARIGOLD",
                    "extension": "STREET",
                    "direction": "",
                    "locality": {
                      "id": "29491",
                      "singleLine": "Margate QLD 4019",
                      "name": "MARGATE",
                      "postcode": {
                        "id": "1306698",
                        "singleLine": "4019 QLD",
                        "name": "4019",
                        "state": "QLD"
                      }
                    }
                  }
                },
                "coordinate": {
                  "latitude": "-27.24133455",
                  "longitude": "153.09870556"
                },
                "currentOwnershipList": [
                  {
                    "mailingAddress": {
                      "careOf": "",
                      "line1": "14 BRENNAN RD",
                      "line2": "SCARBOROUGH QLD",
                      "suburb": "",
                      "state": "",
                      "postcode": "4020",
                      "country": "",
                      "doNotMail": false
                    },
                    "person": {
                      "firstName": "FRANCA",
                      "middleNames": "",
                      "initials": "",
                      "lastName": "DEL ROSSO"
                    },
                    "company": {
                      "companyName": "",
                      "abn": "",
                      "acn": ""
                    }
                  },
                  {
                    "mailingAddress": {
                      "careOf": "",
                      "line1": "14 BRENNAN RD",
                      "line2": "SCARBOROUGH QLD",
                      "suburb": "",
                      "state": "",
                      "postcode": "4020",
                      "country": "",
                      "doNotMail": false
                    },
                    "person": {
                      "firstName": "SAMUELE",
                      "middleNames": "",
                      "initials": "",
                      "lastName": "DEL ROSSO"
                    },
                    "company": {
                      "companyName": "",
                      "abn": "",
                      "acn": ""
                    }
                  }
                ],
                "featureList": [
                  {
                    "abbreviation": "WATER",
                    "id": "261743",
                    "name": "Water",
                    "type": "Boolean",
                    "value": "yes"
                  },
                  {
                    "abbreviation": "SEWAGE",
                    "id": "261745",
                    "name": "Sewage",
                    "type": "Boolean",
                    "value": "yes"
                  },
                  {
                    "abbreviation": "LUG",
                    "id": "261521",
                    "name": "Lockup Garages",
                    "type": "Integer",
                    "value": "4"
                  },
                  {
                    "abbreviation": "WC",
                    "id": "261590",
                    "name": "Toilets",
                    "type": "Integer",
                    "value": "2"
                  },
                  {
                    "abbreviation": "O/RMS",
                    "id": "261622",
                    "name": "Other Rooms",
                    "type": "Integer",
                    "value": "5"
                  },
                  {
                    "abbreviation": "RUMP",
                    "id": "261570",
                    "name": "Family / Rumpus Rooms",
                    "type": "Integer",
                    "value": "1"
                  },
                  {
                    "abbreviation": "PLSH FL",
                    "id": "261568",
                    "name": "Polished Floors",
                    "type": "Boolean",
                    "value": "TRUE"
                  },
                  {
                    "abbreviation": "TENNIS",
                    "id": "261586",
                    "name": "No of Tennis Courts",
                    "type": "Integer",
                    "value": "2"
                  },
                  {
                    "abbreviation": "",
                    "id": "261841",
                    "name": "Other Special Features",
                    "type": "String",
                    "value": "0"
                  }
                ],
                "attributes": {
                  "bedrooms": 4,
                  "bathrooms": 2,
                  "carSpaces": 4,
                  "landArea": 741,
                  "calculatedLandArea": false,
                  "lockUpGarages": 4,
                  "wallMaterial": "",
                  "roofMaterial": "",
                  "yearBuilt": ""
                },
                "parcelList": {
                  "surveyPlan": "",
                  "landAuthority": "Moreton Bay Regional - Pine Rivers",
                  "hundred": "",
                  "referenceSection": " ",
                  "location": "",
                  "plan": "131612",
                  "lot": "31",
                  "lotAlpha": "",
                  "lotPart": "",
                  "section": "",
                  "block": "",
                  "planType": "RP",
                  "area": "741 m?",
                  "primaryPlan": true
                },
                "site": {
                  "landUsePrimary": "Single Unit Dwelling",
                  "landUseSecondary": "None",
                  "zoneCodeLocal": "950",
                  "zoneDescriptionLocal": "Low Density Residential(R)",
                  "zoneCodeGeneral": "G01",
                  "zoneDescriptionGeneral": "Urban",
                  "siteValue": [
                    {
                      "type": "SV",
                      "date": "30/06/2014",
                      "value": "242500",
                      "valuationNumber": "00085591000000"
                    },
                    {
                      "type": "SV",
                      "date": "30/06/2013",
                      "value": "230000",
                      "valuationNumber": "00085591000000"
                    },
                    {
                      "type": "SV",
                      "date": "30/06/2012",
                      "value": "230000",
                      "valuationNumber": "00085591000000"
                    },
                    {
                      "type": "SV",
                      "date": "30/06/2011",
                      "value": "270000",
                      "valuationNumber": "00085591000000"
                    },
                    {
                      "type": "UCV",
                      "date": "30/06/2010",
                      "value": "225000",
                      "valuationNumber": "00085591000000"
                    },
                    {
                      "type": "UCV",
                      "date": "30/06/2005",
                      "value": "160000",
                      "valuationNumber": "00085591000000"
                    }
                  ]
                },
                "id": "5803515",
                "occupancyType": "Rented",
                "propertySubType": "House",
                "propertyType": "HOUSE",
                "forRent": {
                  "advertisementId": "107373850",
                  "agency": {
                    "id": "",
                    "company": {
                      "companyName": "Realway Property Consultants - Redcliffe",
                      "abn": "",
                      "acn": ""
                    },
                    "phone": {
                      "phoneNumber": "(07) 3883 9999",
                      "doNotCall": false
                    },
                    "derivedAgency": false
                  },
                  "agent": {
                    "id": "",
                    "agent": "Candice Wilson",
                    "phone": {
                      "phoneNumber": "",
                      "doNotCall": false
                    },
                    "derivedAgent": false
                  },
                  "daysOnMarket": "52",
                  "fromDate": "23/09/2015",
                  "activeCampaign": true,
                  "period": "W",
                  "price": "480",
                  "priceDescription": "$480",
                  "toDate": "02/11/2015"
                }
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