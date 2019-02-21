# Geofences

To generate a report on [geofences](https://docs.wialon.com/en/hosting/user/geo/geo), you should select one or several geofences in the parameters of the table. In this report, you can use both the geofences from the resource in which the report template is created and the geofences from other resources to which the user has the _View geofences_ [access right](https://docs.wialon.com/en/hosting/cms/rights/resource). The resource is selected in the dropdown list above the list of geofences. It is also possible to select the _All_ option — the list will contain the geofences from all the resources to which the user has the necessary access right. The geofences in the list are sorted by name. To quickly find one, use the dynamic filter.

The following columns can be selected for this table:

* **Geofence** — the name of the geofence.
* **Type** — polygon, line, circle, unit \(if units are selected instead of geofences in the report template\).
* **Area** — the total area of the geofence \(if the metric system is used, the area will be indicated in hectares\).
* **Perimeter** — the perimeter of the geofence. The perimeter for a line is its length \(line thickness is not taken into account\).
* **Description** — description of the geofence \(taken from the geofence properties\).
* **Time in** — the time when the unit entered the geofence.
* **Time out** — the time when the unit left the geofence.
* **Duration in** — the duration of the visit.
* **Total time** — the time from the beginning of the first visit to the end of the last one.
* **Parkings duration** — the time spent in parkings.
* **Off-time** — the time between the previous visit and the current one \(is defined starting from the second visit of the geofence\).
* **Mileage** — mileage inside the zone.
* **Mileage \(adjusted\)** — mileage subject to the coefficient set in the unit properties \( on the _Advanced_ tab\).
* **Counter** — the value of the counter sensor.
* **Initial counter** — the counter value when entering the geofence.
* **Finale counter** — the counter value when exiting the geofence.
* **Avg engine revs** — the average rate of engine revolutions.
* **Max engine revs** — the maximum rate of engine revolutions.
* **Avg temperature** — the average temperature value registered inside a geofence.
* **Min temperature** — the minimum temperature value registered inside a geofence.
* **Max temperature** — the maximum temperature value registered inside a geofence.
* **Initial temperature** — the temperature value when entering a geofence.
* **Final temperature** — the temperature value when leaving a geofence.
* **Off-mileage** — the mileage traveled from the previous visit.
* **Off-mileage \(adjusted\)** — the mileage traveled from the previous visit subjected to the coefficient.
* **Avg speed** — the average speed with which the unit moved in the geofence.
* **Max speed** — the maximum speed with which the unit moved in the geofence.
* **Driver** — the name of the driver \(if available\).
* **Trailer** — the name of the trailer \(if one was bound\).
* **Visits** — the number of visits \(can be helpful either in grouping table data by years/months/weeks/days/shifts or for the reports on unit groups\).
* **Consumed** — the amount of consumed fuel detected by any sort of fuel sensor. If several sensors are available, their values sum up.
* **Consumed by ImpFCS/AbsFCS/InsFCS/FLS/math/rates** — the volume of consumed fuel detected by a fuel sensor \(such as impulse/absolute/instant fuel consumption sensor, fuel level sensor\) or calculated by math or rates. More details about fuel in reports can be found [here](https://docs.wialon.com/en/hosting/user/reports/dat/dat#fuel_in_reports).
* **Avg consumption** — the average fuel consumption by any sort of fuel sensor. If several sensors are available, their values sum up.
* **Avg consumption by ImpFCS/AbsFCS/InsFCS/FLS/math/rates** — the average fuel consumption by one of the methods mentioned above.
* **Penalties** — the penalties calculated for the adjusted [Eco Driving](https://docs.wialon.com/en/hosting/cms/units/eco) criteria.
* **Rank** — penalty points converted to a 6-point rating system.
* **Notes** — an empty column for your custom comments.

![](https://docs.wialon.com/en/hosting/_media/tables/geofences.png)

Instead of geofences, you can select units in the report's template. Additionally, indicate the radius for these units \(in meters\). In this case, the units are considered as _moving geofences_, and the activity of the selected unit is analyzed with respect to these moving geofences. The _Query reports or messages_access is required to these units.

The [intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) by duration, mileage, engine hours, speed range, trips, stops, parkings, sensors, drivers, trailers, fuel fillings, and thefts can be applied to this table.

Geofences can be displayed on the map. To do this, activate the [_Render geofences_](https://docs.wialon.com/en/hosting/user/reports/templ/settings/map) option in the report template.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Note that the monitoring system provides a possibility to detect a geofence visit at its intersection with the segment of the trip track. This option can be enabled in the [Advanced settings](https://docs.wialon.com/en/hosting/user/reports/templ/settings/map#geofences_on_the_map) of the report template.

See related reports — [Non-visited Geofences](https://docs.wialon.com/en/hosting/user/reports/tables/nonvisited), [Rides](https://docs.wialon.com/en/hosting/user/reports/tables/rides).

