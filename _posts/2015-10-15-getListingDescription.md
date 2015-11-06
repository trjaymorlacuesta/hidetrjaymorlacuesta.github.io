---
category: Web Service Calls
path: '/msg/getListingDescription'
title: 'getListingDescription'
type: 'GET'

layout: nil
---

# getListingDescription

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
		<td>Yes</td>
		<td>No</td>
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
		<td>getListingDescription</td>
	</tr>
	<tr>
		<td>propertyId</td>
		<td>-</td>
	</tr>
	<tr>
		<td>advertisementType</td>
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
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?op=getListingDescription&uid=TWISTUSER001&sid=2-4eed242594fc464787b8054ddc77de11&propertyId=7267327
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
            "advertisementList": {
                "description": "AFFORDABLE FAMILY HOME<BR>THIS TIDY 3 BEDROOM HOME OFFERS AFFORDABLE LIVING IDEAL FOR A SMALL FAMILY. POLISHED FLOORBOARDS THROUGHOUT LIVING AND DINING AREA. UPDATED KITCHEN. OUTDOOR DECK AND COURTYARD FOR ENTERTAINING. SMALL TERRACED REAR YARD. GARAGE AND ADDITIONAL STUDIO ROOM UNDERNEATH. QUIET STREET, CLOSE TO PRE-SCHOOL, SHORT DISTANCE TO LAKE, PUBLIC JETTY AND LOCAL CLUB. PET/S: SORRY THIS PROPERTY IS NOT SUITABLE FOR PETS ARRANGING TO VIEW A PROPERTY WE PRIDE OURSELVES ON OFFERING A QUALITY SERVICE AND ASSISTING YOU TO FIND THE RIGHT RENTAL PROPERTY. YOU WON'T BE SUBJECT TO INCONVENIENT & IMPERSONAL OPEN HOUSE INSPECTIONS. OUR AUTOMATED BOOKING SYSTEM WILL ASSIST YOU WITH A HASSLE FREE APPROACH TO VIEWING PROPERTIES + KEEP YOU INFORMED DURING THE PROCESS OF APPLYING FOR TENANCY. IF YOU REQUIRE ANY FURTHER INFORMATION OR ASSISTANCE, PLEASE EMAIL OUR OFFICE OR PHONE.. WE WILL BE HAPPY TO ASSIST YOU. PH. 02 4950 4900",
                "id": "1244920",
                "type": "FORRENT",
                "date": "10/11/2014",
                "method": "Rental",
                "period": "W",
                "price": "340",
                "priceDescription": "$340 PER WEEK",
                "advertiserList": [
                    {
                        "companyName": "",
                        "agencyPhoneNumber": "",
                        "agent": "Melanie Bieler",
                        "agentPhoneNumber": ""
                    },
                    {
                        "companyName": "Keys Real Estate",
                        "agencyPhoneNumber": "(02) 4950 4900",
                        "agent": "Mel Bieler",
                        "agentPhoneNumber": "(02) 4950 4900"
                    }
                ]
            }
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