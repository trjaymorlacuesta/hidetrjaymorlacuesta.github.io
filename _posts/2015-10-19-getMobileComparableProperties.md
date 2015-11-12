---
category: Web Service Calls
path: '/msg/getMobileComparableProperties'
title: 'getMobileComparableProperties'
type: 'GET'

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

* The headers must include a **valid authentication token**.

<table>
	<tbody>
	<tr>
		<th>Parameter</th>
        <th>Description</th>
        <th>Required</th>
        
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
		<td>op</td>
        <td>Operation</td>
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

<div id="msgtesturl">
<table>
	<tbody>
	<tr>
		<th>Test URL MSG Agent -MSGSIT:</th>
	</tr>
	<tr>
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?op=getMobileComparableProperties&uid=TWISTUSER001&limit=1&comparableRuleId=3&sid=2-4eed242594fc464787b8054ddc77de11&propertyId=3971426
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
            "comparableSummaryLists": [
                {
                    "averageForRentListingPrice": "438",
                    "maximumForRentCampaignDate": "26/10/2015",
                    "maximumForRentListingPrice": "460",
                    "medianForRentListingPrice": "435",
                    "minimumForRentCampaignDate": "20/10/2015",
                    "minimumForRentListingPrice": "420",
                    "comparableCategoryId": "2",
                    "comparableCategory": "GOOD",
                    "totalProperties": "3",
                    "propertyComparableList": [
                        {
                            "propertyDetail": {
                                "distanceFromTarget": "1.0139446868242528",
                                "address": {
                                    "buildingComplexName": "",
                                    "councilArea": "Moreton Bay Regional - Pine Rivers",
                                    "singleLine": "24 Wendy Crescent Clontarf QLD 4019",
                                    "unitNumber": "",
                                    "unitAlpha": "",
                                    "derivedUnit": false,
                                    "startNumber": "24",
                                    "startAlpha": "",
                                    "endNumber": "",
                                    "endAlpha": "",
                                    "street": {
                                        "id": "2604467",
                                        "singleLine": "Wendy Crescent Clontarf QLD 4019",
                                        "name": "WENDY",
                                        "extension": "CRESCENT",
                                        "direction": "",
                                        "locality": {
                                            "id": "28085",
                                            "singleLine": "Clontarf QLD 4019",
                                            "name": "CLONTARF",
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
                                    "latitude": "-27.25356665",
                                    "longitude": "153.08406791"
                                },
                                "currentOwnershipList": [
                                    {
                                        "mailingAddress": {
                                            "careOf": "",
                                            "line1": "9/61-65 WARIALDA ST",
                                            "line2": "KOGARAH NSW",
                                            "suburb": "",
                                            "state": "",
                                            "postcode": "2217",
                                            "country": "",
                                            "doNotMail": false
                                        },
                                        "person": {
                                            "firstName": "DIANA",
                                            "middleNames": "",
                                            "initials": "",
                                            "lastName": "WOLSELY"
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
                                            "line1": "9/61-65 WARIALDA ST",
                                            "line2": "KOGARAH NSW",
                                            "suburb": "",
                                            "state": "",
                                            "postcode": "2217",
                                            "country": "",
                                            "doNotMail": false
                                        },
                                        "person": {
                                            "firstName": "MENA RAMSES RIAD",
                                            "middleNames": "",
                                            "initials": "",
                                            "lastName": "WOLSELY"
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
                                        "value": "1"
                                    },
                                    {
                                        "abbreviation": "M2F",
                                        "id": "261589",
                                        "name": "M2 Total In Floor Area",
                                        "type": "Float",
                                        "value": "112.00"
                                    },
                                    {
                                        "abbreviation": "T/FLR",
                                        "id": "261593",
                                        "name": "Total Floors In Building",
                                        "type": "Integer",
                                        "value": "1"
                                    },
                                    {
                                        "abbreviation": "YR BUILT",
                                        "id": "261587",
                                        "name": "Year Built",
                                        "type": "Integer",
                                        "value": "1980"
                                    },
                                    {
                                        "abbreviation": "ENS",
                                        "id": "259992",
                                        "name": "Ensuites",
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
                                        "abbreviation": "OPENPLAN",
                                        "id": "261513",
                                        "name": "Open Plan",
                                        "type": "Boolean",
                                        "value": "TRUE"
                                    },
                                    {
                                        "abbreviation": "RENOVATED",
                                        "id": "261580",
                                        "name": "Renovated",
                                        "type": "Boolean",
                                        "value": "TRUE"
                                    },
                                    {
                                        "abbreviation": "",
                                        "id": "261812",
                                        "name": "Building Area",
                                        "type": "Float",
                                        "value": "23"
                                    },
                                    {
                                        "abbreviation": "WALLEXT",
                                        "id": "261829",
                                        "name": "Materials in External Walls",
                                        "type": "String",
                                        "value": "Rendered brick"
                                    },
                                    {
                                        "abbreviation": "ROOF",
                                        "id": "261832",
                                        "name": "Materials in Roof",
                                        "type": "String",
                                        "value": "0"
                                    }
                                ],
                                "attributes": {
                                    "bedrooms": 4,
                                    "bathrooms": 2,
                                    "carSpaces": 2,
                                    "landArea": 607,
                                    "calculatedLandArea": false,
                                    "lockUpGarages": 1,
                                    "wallMaterial": "Rendered brick",
                                    "roofMaterial": "0",
                                    "yearBuilt": "1980"
                                },
                                "parcelList": {
                                    "surveyPlan": "",
                                    "landAuthority": "Moreton Bay Regional - Pine Rivers",
                                    "hundred": "",
                                    "referenceSection": " ",
                                    "location": "",
                                    "plan": "102525",
                                    "lot": "17",
                                    "lotAlpha": "",
                                    "lotPart": "",
                                    "section": "",
                                    "block": "",
                                    "planType": "RP",
                                    "area": "607 m?",
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
                                            "value": "237500",
                                            "valuationNumber": "00101850000000"
                                        },
                                        {
                                            "type": "SV",
                                            "date": "30/06/2013",
                                            "value": "225000",
                                            "valuationNumber": "00101850000000"
                                        },
                                        {
                                            "type": "SV",
                                            "date": "30/06/2012",
                                            "value": "225000",
                                            "valuationNumber": "00101850000000"
                                        },
                                        {
                                            "type": "SV",
                                            "date": "30/06/2011",
                                            "value": "265000",
                                            "valuationNumber": "00101850000000"
                                        },
                                        {
                                            "type": "UCV",
                                            "date": "30/06/2010",
                                            "value": "265000",
                                            "valuationNumber": "00101850000000"
                                        },
                                        {
                                            "type": "UCV",
                                            "date": "30/06/2005",
                                            "value": "202500",
                                            "valuationNumber": "00101850000000"
                                        }
                                    ]
                                },
                                "id": "3980954",
                                "occupancyType": "Rented",
                                "propertySubType": "House",
                                "propertyType": "HOUSE",
                                "forRent": {
                                    "advertisementId": "106618315",
                                    "agency": {
                                        "id": "",
                                        "company": {
                                            "companyName": "Abode Properties - Woody Point",
                                            "abn": "",
                                            "acn": ""
                                        },
                                        "phone": {
                                            "phoneNumber": "(07) 3284 1999",
                                            "doNotCall": false
                                        },
                                        "derivedAgency": false
                                    },
                                    "agent": {
                                        "id": "",
                                        "agent": "Lyn Batten",
                                        "phone": {
                                            "phoneNumber": "0477 117 899",
                                            "doNotCall": false
                                        },
                                        "derivedAgent": false
                                    },
                                    "daysOnMarket": "61",
                                    "fromDate": "04/09/2015",
                                    "activeCampaign": true,
                                    "period": "W",
                                    "price": "460",
                                    "priceDescription": "$460 per week",
                                    "toDate": "21/10/2015"
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