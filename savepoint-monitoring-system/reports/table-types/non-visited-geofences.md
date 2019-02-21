# Non-visited Geofences

This report gives the list of [geofences](https://docs.wialon.com/en/hosting/user/geo/geo) that were not visited during the indicated time period.

In the parameters of the table, select one or several geofences. In this report, you can use both the geofences from the resource in which the report template is created, as well as the geofences from other resources to which the user has the _View geofences_ [access right](https://docs.wialon.com/en/hosting/cms/rights/resource). The resource is selected in the dropdown list above the list of geofences. It is also possible to select the _All_ option — then the list will contain the geofences from all the resources to which the user has the necessary access right. The geofences in the list are sorted by name. To quickly find one, use the dynamic filter.

Suppose, we have 11 points \(geofences\) that a unit should visit every day. We would like to find out whether there are geofences which were ignored within the work week from June 1 to June 5. To do this, we enable grouping by days \(with detalization\), select necessary geofences and columns for the table.

* **Geofence** — the name of the geofence.
* **Type** — the type of geofence: line, polygon, or circle.
* **Area** — the total area of the geofence \(if the metric system is used, the area is indicated in hectares\).
* **Perimeter** — the perimeter of the geofence.
* **Count** — the number of geofences that were skipped.
* **Description** — the information from the same-name field of the [geofence's properties](https://docs.wialon.com/en/hosting/user/geo/new#ustanovite_svojstva_geozony).
* **Notes** — an empty column for your custom comments.

From this report we see that on June 1 _Point 11_ and _Point 7_ were ignored, on June 4 — _Point 2_, and on June 5 — five geofences. June 2 and 3 are absent, which means that all the predefined geofences were visited on those days. You can click on the names of the geofences to move the map to their first point.

![](https://docs.wialon.com/en/hosting/_media/tables/nonvisited.png)

When the table is applied to a [unit group](https://docs.wialon.com/en/hosting/user/reports/adv/adv), you can find one more parameter in the report template — **Consider group as a whole**. When the box is checked, a group report is structured in the same way as an individual report, and the information is given for each separate unit from the group. When the _Consider group as a whole_ checkbox is marked, the report structure is different — you get the list of geofences that were not visited by any units from the group.

