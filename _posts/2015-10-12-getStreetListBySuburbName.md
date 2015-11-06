---
category: Web Service Calls
path: '/msg/getStreetListBySuburbName'
title: 'getStreetListBySuburbName'
type: 'GET'

layout: nil
---

# getStreetListBySuburbName

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
		<td>getStreetListBySuburbName</td>
	</tr>
	<tr>
		<td>street</td>
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
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?uid=bsguser.rpmob3.bberry&op=getStreetListBySuburbName&sid=2-4eed242594fc464787b8054ddc77de11&street=&suburb=turramurra&state=NSW&pageNumber=1&pageSize=10
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
            "streets": {
                "page": "1",
                "size": "134",
                "total": "134",
                "streetList": [
                    {
                        "displayAddress": "Acacia Close Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Acacia Close"
                    },
                    {
                        "displayAddress": "Adams Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Adams Avenue"
                    },
                    {
                        "displayAddress": "Alice Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Alice Street"
                    },
                    {
                        "displayAddress": "Allan Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Allan Avenue"
                    },
                    {
                        "displayAddress": "Ancona Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Ancona Road"
                    },
                    {
                        "displayAddress": "Apps Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Apps Avenue"
                    },
                    {
                        "displayAddress": "Avalon Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Avalon Street"
                    },
                    {
                        "displayAddress": "Avoca Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Avoca Road"
                    },
                    {
                        "displayAddress": "Bangalla Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Bangalla Street"
                    },
                    {
                        "displayAddress": "Bannockburn Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Bannockburn Road"
                    },
                    {
                        "displayAddress": "Barellan Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Barellan Avenue"
                    },
                    {
                        "displayAddress": "Berrillee Lane Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Berrillee Lane"
                    },
                    {
                        "displayAddress": "Berrillee Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Berrillee Street"
                    },
                    {
                        "displayAddress": "Biara Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Biara Place"
                    },
                    {
                        "displayAddress": "Billabong Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Billabong Avenue"
                    },
                    {
                        "displayAddress": "Bobbin Head Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Bobbin Head Road"
                    },
                    {
                        "displayAddress": "Boomerang Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Boomerang Street"
                    },
                    {
                        "displayAddress": "Boronia Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Boronia Avenue"
                    },
                    {
                        "displayAddress": "Boyd Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Boyd Street"
                    },
                    {
                        "displayAddress": "Brentwood Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Brentwood Avenue"
                    },
                    {
                        "displayAddress": "Buckra Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Buckra Street"
                    },
                    {
                        "displayAddress": "Buller Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Buller Street"
                    },
                    {
                        "displayAddress": "Burns Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Burns Road"
                    },
                    {
                        "displayAddress": "Canberra Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Canberra Avenue"
                    },
                    {
                        "displayAddress": "Carina Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Carina Road"
                    },
                    {
                        "displayAddress": "Catalpa Crescent Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Catalpa Crescent"
                    },
                    {
                        "displayAddress": "Challis Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Challis Avenue"
                    },
                    {
                        "displayAddress": "Charlton Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Charlton Avenue"
                    },
                    {
                        "displayAddress": "Chester Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Chester Road"
                    },
                    {
                        "displayAddress": "Chilton Parade Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Chilton Parade"
                    },
                    {
                        "displayAddress": "Coila Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Coila Street"
                    },
                    {
                        "displayAddress": "Coolabah Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Coolabah Avenue"
                    },
                    {
                        "displayAddress": "Coolabah Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Coolabah Place"
                    },
                    {
                        "displayAddress": "Cornwall Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Cornwall Avenue"
                    },
                    {
                        "displayAddress": "Cudgee Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Cudgee Street"
                    },
                    {
                        "displayAddress": "Dawson Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Dawson Place"
                    },
                    {
                        "displayAddress": "Denman Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Denman Street"
                    },
                    {
                        "displayAddress": "Duff Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Duff Street"
                    },
                    {
                        "displayAddress": "Eastern Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Eastern Road"
                    },
                    {
                        "displayAddress": "Ellalong Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Ellalong Road"
                    },
                    {
                        "displayAddress": "Evelyn Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Evelyn Avenue"
                    },
                    {
                        "displayAddress": "Fairlawn Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Fairlawn Avenue"
                    },
                    {
                        "displayAddress": "Finchley Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Finchley Place"
                    },
                    {
                        "displayAddress": "Finlay Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Finlay Road"
                    },
                    {
                        "displayAddress": "Fitzroy Crescent Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Fitzroy Crescent"
                    },
                    {
                        "displayAddress": "Forwood Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Forwood Avenue"
                    },
                    {
                        "displayAddress": "Georgann Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Georgann Street"
                    },
                    {
                        "displayAddress": "Gilroy Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Gilroy Road"
                    },
                    {
                        "displayAddress": "Gipps Close Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Gipps Close"
                    },
                    {
                        "displayAddress": "Glendale Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Glendale Road"
                    },
                    {
                        "displayAddress": "Godfrey Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Godfrey Avenue"
                    },
                    {
                        "displayAddress": "Handley Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Handley Avenue"
                    },
                    {
                        "displayAddress": "Harrington Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Harrington Avenue"
                    },
                    {
                        "displayAddress": "Hastings Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Hastings Road"
                    },
                    {
                        "displayAddress": "Holmes Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Holmes Street"
                    },
                    {
                        "displayAddress": "Howson Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Howson Avenue"
                    },
                    {
                        "displayAddress": "Jersey Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Jersey Street"
                    },
                    {
                        "displayAddress": "Karloo Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Karloo Street"
                    },
                    {
                        "displayAddress": "Karuah Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Karuah Road"
                    },
                    {
                        "displayAddress": "Kate Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Kate Street"
                    },
                    {
                        "displayAddress": "Katina Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Katina Street"
                    },
                    {
                        "displayAddress": "Kent Lane Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Kent Lane"
                    },
                    {
                        "displayAddress": "Kent Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Kent Road"
                    },
                    {
                        "displayAddress": "King Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "King Street"
                    },
                    {
                        "displayAddress": "Kirawa Close Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Kirawa Close"
                    },
                    {
                        "displayAddress": "Kissing Point Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Kissing Point Road"
                    },
                    {
                        "displayAddress": "Konda Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Konda Place"
                    },
                    {
                        "displayAddress": "Ku-Ring-Gai Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Ku-ring-gai Avenue"
                    },
                    {
                        "displayAddress": "Kuruk Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Kuruk Place"
                    },
                    {
                        "displayAddress": "Lamond Drive Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Lamond Drive"
                    },
                    {
                        "displayAddress": "Laurel Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Laurel Avenue"
                    },
                    {
                        "displayAddress": "Laurence Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Laurence Avenue"
                    },
                    {
                        "displayAddress": "Leeds Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Leeds Place"
                    },
                    {
                        "displayAddress": "May Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "May Street"
                    },
                    {
                        "displayAddress": "McRae Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Mcrae Place"
                    },
                    {
                        "displayAddress": "Merrivale Lane Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Merrivale Lane"
                    },
                    {
                        "displayAddress": "Michele Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Michele Place"
                    },
                    {
                        "displayAddress": "Milford Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Milford Place"
                    },
                    {
                        "displayAddress": "Mimosa Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Mimosa Road"
                    },
                    {
                        "displayAddress": "Monteith Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Monteith Street"
                    },
                    {
                        "displayAddress": "Morna Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Morna Place"
                    },
                    {
                        "displayAddress": "Murdoch Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Murdoch Street"
                    },
                    {
                        "displayAddress": "Musgrave Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Musgrave Street"
                    },
                    {
                        "displayAddress": "Nambucca Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Nambucca Street"
                    },
                    {
                        "displayAddress": "Nimbrin Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Nimbrin Street"
                    },
                    {
                        "displayAddress": "Nulla Nulla Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Nulla Nulla Street"
                    },
                    {
                        "displayAddress": "Pacific Highway Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Pacific Highway"
                    },
                    {
                        "displayAddress": "Pembroke Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Pembroke Avenue"
                    },
                    {
                        "displayAddress": "Pentecost Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Pentecost Avenue"
                    },
                    {
                        "displayAddress": "Princes Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Princes Street"
                    },
                    {
                        "displayAddress": "Raglan Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Raglan Street"
                    },
                    {
                        "displayAddress": "Ravenhill Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Ravenhill Road"
                    },
                    {
                        "displayAddress": "Ray Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Ray Street"
                    },
                    {
                        "displayAddress": "Rohini Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Rohini Street"
                    },
                    {
                        "displayAddress": "Roland Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Roland Avenue"
                    },
                    {
                        "displayAddress": "Rotherwood Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Rotherwood Place"
                    },
                    {
                        "displayAddress": "Rothwell Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Rothwell Road"
                    },
                    {
                        "displayAddress": "Rushall Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Rushall Street"
                    },
                    {
                        "displayAddress": "Sandford Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Sandford Road"
                    },
                    {
                        "displayAddress": "Satterley Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Satterley Avenue"
                    },
                    {
                        "displayAddress": "Shand Crescent Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Shand Crescent"
                    },
                    {
                        "displayAddress": "Solander Close Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Solander Close"
                    },
                    {
                        "displayAddress": "Spurwood Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Spurwood Road"
                    },
                    {
                        "displayAddress": "St James Lane Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "St James Lane"
                    },
                    {
                        "displayAddress": "Stainsby Close Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Stainsby Close"
                    },
                    {
                        "displayAddress": "Surrey Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Surrey Road"
                    },
                    {
                        "displayAddress": "Swindon Close Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Swindon Close"
                    },
                    {
                        "displayAddress": "Tallong Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Tallong Place"
                    },
                    {
                        "displayAddress": "Tamboon Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Tamboon Avenue"
                    },
                    {
                        "displayAddress": "Taylor Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Taylor Avenue"
                    },
                    {
                        "displayAddress": "Tennyson Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Tennyson Avenue"
                    },
                    {
                        "displayAddress": "Terrigal Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Terrigal Avenue"
                    },
                    {
                        "displayAddress": "The Chase Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "The Chase Road"
                    },
                    {
                        "displayAddress": "The Comenarra Parkway Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "The Comenarra Parkway"
                    },
                    {
                        "displayAddress": "The Mall Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "The Mall"
                    },
                    {
                        "displayAddress": "Timaru Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Timaru Street"
                    },
                    {
                        "displayAddress": "Tintagel Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Tintagel Place"
                    },
                    {
                        "displayAddress": "Trentino Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Trentino Road"
                    },
                    {
                        "displayAddress": "Turramurra Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Turramurra Avenue"
                    },
                    {
                        "displayAddress": "Turuga Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Turuga Street"
                    },
                    {
                        "displayAddress": "Wambool Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Wambool Street"
                    },
                    {
                        "displayAddress": "Waratah Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Waratah Road"
                    },
                    {
                        "displayAddress": "Warragal Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Warragal Road"
                    },
                    {
                        "displayAddress": "Warrangi Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Warrangi Street"
                    },
                    {
                        "displayAddress": "Water Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Water Street"
                    },
                    {
                        "displayAddress": "Wattle Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Wattle Place"
                    },
                    {
                        "displayAddress": "William Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "William Street"
                    },
                    {
                        "displayAddress": "Wiltshire Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Wiltshire Place"
                    },
                    {
                        "displayAddress": "Wolsten Avenue Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Wolsten Avenue"
                    },
                    {
                        "displayAddress": "Womerah Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Womerah Street"
                    },
                    {
                        "displayAddress": "Wonga Wonga Road Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Wonga Wonga Road"
                    },
                    {
                        "displayAddress": "Wonga Wonga Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Wonga Wonga Street"
                    },
                    {
                        "displayAddress": "Worcester Place Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Worcester Place"
                    },
                    {
                        "displayAddress": "Yeramba Street Turramurra NSW 2074",
                        "state": "NSW",
                        "suburb": "Turramurra",
                        "streetName": "Yeramba Street"
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