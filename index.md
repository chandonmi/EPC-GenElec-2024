# 2024 General Election Results for El Paso County, Colorado

This interactive map was made with QGIS and the qgis2web plugin. It comprehensively details the 2024 General Election results for El Paso County for 4 ballot measures: Amendment J, Proposition KK, Question 300, and Amendment 79.

## Map Background & Details

This interactive map is the result of a months-long project to visually represent last year's election results for El Paso County at the precinct level. The purpose of this map is to strategically support the <a href="https://www.jointinitiatives.org/family-friendly-initiative/">Family Friendly Initiative</a>, a collaborative initiative to expand affordable childcare for families across the Pikes Peak Region. This data can be used to develop an optimal strategy for a ballot measure that would address the childcare gap in El Paso County.

Data on all state-wide propositions and amendments, the presidential race, and all national and state representative/senate candidates was initially collected across all 329 precincts in El Paso County. This data was then corresponded to each precinct's shapefile, which was obtained through a public dataset found <a href="https://opendata-elpasoco.hub.arcgis.com/datasets/6a9d04124af34a218dfebdbfc2c16864_0/about">here</a>. I uploaded the shapefile layers into QGIS and joined election results data for the 4 ballot measures in each table.

Using rule-based and graduated symbology in each layer, precincts were color-coded to indicate Yes/For, No/Against, and Tie results. The heat maps shade each precinct according to their percentage of yes votes - darker precincts indicate a higher percentage of yes votes, and lighter precincts indicate a lower percentage. In addition, I also created a layer of "swing precincts" for each ballot measure to show precincts that had a roughly even split of votes. The ratio of % yes/no votes for these precincts ranges from 52/48 to 48/52. Once the initial map layers were complete, I used the qgis2web plugin to make the map accessible and interactive on a webpage.

When you get to the map, use the Leaflet dropdown menu in the upper-right corner to display which ballot measure results and their associated heat maps/swing precincts you want to see. You can click on individual precincts to show the precinct number, contest, total precinct votes, Yes/For and No/Against votes, and percentages of Yes/For and No/Against votes. Note that Question 300 was a local ballot measure for Colorado Springs, so only precincts for Colorado Springs will display for that layer. Precinct 747 did not receive any votes for any of the 4 ballot measures, which is why it was omitted - hence the "hole" in the map.

## Ballot Measure Details

**Amendment J:** Proposed removing language from the Colorado Constitution prohibiting same-sex couples from marrying. Amendment J succeeded in El Paso County, with 55.8% of voters voting Yes/For, and succeeded state-wide with 64.3% of all voters in Colorado voting Yes/For.

**Proposition KK:** Proposed levying a 6.5% excise tax on the sale and manufacturing of firearms and ammunition. This tax would be imposed on firearms dealers, manufacturers, and ammunition vendors. The revenue from this tax would be used to fund crime victim services programs, mental health programs for children and veterans, and school security and safety programs. Proposition KK succeeded state-wide, with 54.4% of all voters voting Yes/For, but failed in El Paso County with 54.4% of voters voting No/Against.

**Question 300:** Proposed authorizing medical marijuana licensees to become recreational marijuana retail licensees. Question 300 succeeded in Colorado Springs, with 54.7% of voters voting Yes/For.

**Amendment 79**: Proposed creating a right to abortion in the state of Colorado and allowing the use of public funds for abortion. Amendment 79 succeeded state-wide, with 62% of voters voting Yes/For, and succeeded in El Paso County with 52% of voters voting Yes/For.

<iframe src="qgis2web_2025_08_25-15_03_14_455580/map.html" height="700" width="700"></iframe>
