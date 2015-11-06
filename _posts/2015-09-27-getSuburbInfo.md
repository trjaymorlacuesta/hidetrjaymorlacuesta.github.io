---
category: Web Service Calls
path: '/msg/getSuburbInfo'
title: 'getSuburbInfo'
type: 'GET'

layout: nil
---

# getSuburbInfo

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
		<td>getSuburbInfo</td>
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
		<td>yearFrom</td>
		<td>-</td>
	</tr>
	<tr>
		<td>period</td>
		<td>-</td>
	</tr>
	<tr>
		<td>displayChartUrl</td>
		<td>-</td>
	</tr>
	<tr>
		<td>displaySuburbStatistics</td>
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
    		<td>http://msgsit.rpdata.com/ttsvr/msgdebug?uid=TWISTUSER001&op=getSuburbInfo&suburb=Newtown&state=NSW&postcode=2042&yearFrom=2010&period=[1,5,10]&sid=2-4eed242594fc464787b8054ddc77de11
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
            "population": 14158,
            "medianPriceHouses": {
                "medianPrice": 830000,
                "growthValue": [
                    "22.1",
                    "44.38",
                    "133.15"
                ]
            },
            "medianPriceUnits": {
                "medianPrice": 377500,
                "growthValue": [
                    "-7.9",
                    "16.13",
                    "46.45"
                ]
            },
            "predominantStructure": "Childless Couples",
            "hotspots": false,
            "homeBuyerIndex": 5,
            "region": "Inner Sydney",
            "periodHouses": [
                "October",
                "November",
                "December",
                "January",
                "February",
                "March",
                "April",
                "May",
                "June",
                "July",
                "August",
                "September"
            ],
            "medianPriceSuburbHouses": [
                1025000,
                1120000,
                1080000,
                1042500,
                1265000,
                1340000,
                1274000,
                1200000,
                1460000,
                1210000,
                1362500,
                1210000
            ],
            "medianPriceLgaHouses": [
                1207500,
                1180000,
                1230000,
                1376000,
                1300000,
                1437000,
                1420000,
                1380000,
                1390000,
                1450000,
                1400500,
                1405000
            ],
            "periodUnits": [
                "October",
                "November",
                "December",
                "January",
                "February",
                "March",
                "April",
                "May",
                "June",
                "July",
                "August",
                "September"
            ],
            "medianPriceSuburbUnits": [
                568500,
                480000,
                558000,
                361250,
                605000,
                630000,
                475000,
                712500,
                450000,
                687500,
                648500,
                525000
            ],
            "medianPriceLgaUnits": [
                735000,
                725000,
                729000,
                750000,
                738500,
                775000,
                765000,
                800000,
                805500,
                805500,
                830000,
                802500
            ],
            "salesNumberChartHouseUrl": "https://static.rpdata.com/rpdaAU/chart/au/sale-by-number/450x250/2010/10/12087/house.png",
            "salesNumberChartUnitsUrl": "https://static.rpdata.com/rpdaAU/chart/au/sale-by-number/450x250/2010/10/12087/unit.png",
            "salesPriceChartHouseUrl": "https://static.rpdata.com/rpdaAU/chart/au/sale-by-price/450x250/2015/12087/house.png",
            "salesPriceChartUnitsUrl": "https://static.rpdata.com/rpdaAU/chart/au/sale-by-price/450x250/2015/12087/unit.png",
            "monthlyMedianPriceUnitsUrl": "https://static.rpdata.com/rpdaAU/chart/au/median-sale-price-monthly/350x280/2011/12087/2708/unit.png",
            "monthlyMedianPriceHousesUrl": "https://static.rpdata.com/rpdaAU/chart/au/median-sale-price-monthly/350x280/2011/12087/2708/house.png",
            "yearlyMedianPriceUnitsUrl_3": "https://static.rpdata.com/rpdaAU/chart/au/median-sale-price-yearly/350x280/2010/3/12087/2708/unit.png",
            "yearlyMedianPriceHousesUrl_3": "https://static.rpdata.com/rpdaAU/chart/au/median-sale-price-yearly/350x280/2010/3/12087/2708/house.png",
            "yearlyMedianPriceUnitsUrl_10": "https://static.rpdata.com/rpdaAU/chart/au/median-sale-price-yearly/350x280/2010/10/12087/2708/unit.png",
            "yearlyMedianPriceHousesUrl_10": "https://static.rpdata.com/rpdaAU/chart/au/median-sale-price-yearly/350x280/2010/10/12087/2708/house.png",
            "demographicParagraph": "The size of Newtown is approximately 2 square kilometres. It has 6 parks covering nearly 3% of total area.\nThe population of Newtown in 2006 was 13,543 people. By 2011 the population was 14,158 showing a population growth of 4% in the area during that time.\nThe predominant age group in Newtown is 25-34 years.\nHouseholds in Newtown are primarily childless couples and are likely to be repaying between $3000 - $4000 per month on mortgage repayments.\nIn general, people in Newtown work in a Professional occupation.\nIn 2006, 42.1% of the homes in Newtown were owner-occupied compared with 41.2% in 2011.\nCurrently the median sales price of houses in the area is 1,210,000.\n\n",
            "medianAskingRentHouses": 563,
            "medianAskingRentUnits": 380,
            "timeOnMarketDaysHouses": 49,
            "timeOnMarketDaysUnits": 52
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