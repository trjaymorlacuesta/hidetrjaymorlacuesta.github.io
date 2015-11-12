---
category: Web Service Calls
path: '/msg/getMobileMarketTrends'
title: 'getMobileMarketTrends'
type: 'GET'

layout: nil
---

# getMobileMarketTrends

##Overview
This call is used to to obtain time series data for one or many metrics, geographies, property types or periods of a given suburb; it uses BSGv3's statistics service.

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
		<td>metricTypeId</td>
		<td>Metric Type Id</td>
        <td>Yes</td>
        
	</tr>
	<tr>
		<td>suburbId</td>
		<td>Suburb Id</td>
        <td>Yes</td>
        
	</tr>
	<tr>
		<td>propertyTypeId</td>
		<td>Property Type Id</td>
        <td>No</td>
        
	</tr>
	<tr>
		<td>fromDate</td>
		<td>From Date</td>
        <td>Yes</td>
        
	</tr>
	<tr>
		<td>toDate</td>
		<td>To Date</td>
        <td>Yes</td>
        
	</tr>
	<tr>
		<td>interval</td>
		<td>Interval</td>
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
		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?op=getMobileMarketTrends&uid=TWISTUSER001&sid=2-4eed242594fc464787b8054ddc77de11&metricTypeId=21&suburbId=28179&propertyTypeId=1&fromDate=2012-02-29&toDate=2013-03-31&interval=1
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
            "marketTrendsLists": [
                {
                    "localityName": "COORPAROO",
                    "locationType": "Locality",
                    "postcodeName": "4151",
                    "councilAreaName": "",
                    "territorialAuthorityName": "",
                    "stateName": "",
                    "countryName": "",
                    "propertyType": "Houses",
                    "metricDisplayType": "Dollar",
                    "metricType": "Median Sale Price (12 months)",
                    "metricTypeShort": "",
                    "metricTypeId": "21",
                    "metricTypeGroupId": "",
                    "metricTypeOrderId": "",
                    "metricTypeGroup": "",
                    "metricTypeDescription": "Statistics are calculated over a rolling 12 month period",
                    "metricTypeGroupDescription": "",
                    "sumStatistic": false,
                    "zMarketTrendsDataLists": [
                        {
                            "dateTime": "29/02/2012",
                            "value": "620000.0"
                        },
                        {
                            "dateTime": "31/03/2012",
                            "value": "625000.0"
                        },
                        {
                            "dateTime": "30/04/2012",
                            "value": "617500.0"
                        },
                        {
                            "dateTime": "31/05/2012",
                            "value": "592500.0"
                        },
                        {
                            "dateTime": "30/06/2012",
                            "value": "587500.0"
                        },
                        {
                            "dateTime": "31/07/2012",
                            "value": "606000.0"
                        },
                        {
                            "dateTime": "31/08/2012",
                            "value": "612000.0"
                        },
                        {
                            "dateTime": "30/09/2012",
                            "value": "609000.0"
                        },
                        {
                            "dateTime": "31/10/2012",
                            "value": "584500.0"
                        },
                        {
                            "dateTime": "30/11/2012",
                            "value": "598250.0"
                        },
                        {
                            "dateTime": "31/12/2012",
                            "value": "616000.0"
                        },
                        {
                            "dateTime": "31/01/2013",
                            "value": "590750.0"
                        },
                        {
                            "dateTime": "28/02/2013",
                            "value": "616000.0"
                        },
                        {
                            "dateTime": "31/03/2013",
                            "value": "603500.0"
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