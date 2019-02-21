# Rides

Wialon can track rides between geofences if one of them \(or several\) is set as the starting point, and the other \(or several\) as the final one. Two factors are important to generate such report: when a unit leaves the starting geofence and when it enters the final one. In such case, a ride between geofences is considered complete. In addition, all rides between geofences are determined taking into account the trip detector.

This report is useful, for instance, to control the transportation of a cargo from one place to another in several trips.

### Preparing Geofences <a id="preparing_geofences"></a>

To get a report on rides between geofences, you must first create [geofences](https://docs.wialon.com/en/hosting/user/geo/geo) that determine the beginning and end of the ride. The beginning and the end can be the same geofence if the ride starts and ends in one place, for example, if you need to transport cargo from point A to point B and this will take more than one trip. Create two geofences and then specify them as the starting and ending points in the report template.

![](https://docs.wialon.com/en/hosting/_media/tables/rides1.png)

### Ride Parameters <a id="ride_parameters"></a>

When you create a report template for rides, you can set additional parameters for it.

**Allow circle ride**  
Check this option if the beginning and end of the ride must be in the same geofence. At the same time, in order for the report to work, it is necessary that a geofence \(or a unit\) have both boxes checked — beginning and end of the ride.

**Show the rides finished with a stop**  
This can be used as an additional filter. If this option is selected, only visiting the geofences with a stop at the final point are considered the end of the ride. Note that a stop is considered to be a unit state in which its speed is less than the minimum moving speed indicated in the [trip detector](https://docs.wialon.com/en/hosting/cms/units/trip). A ride begins when a unit leaves the starting point. If a unit enters the final destination \(after the beginning of the ride has been detected\), but does not make a stop there, the ride continues.

**Starting and terminal points**  
In this section, you choose which geofences and units will be analyzed in the report. You can not only use the geofences from the resource in which the report template is created but also the geofences from other resources to which the user has the [access right](https://docs.wialon.com/en/hosting/cms/rights/resource) _View geofences_. The resource is chosen in the dropdown list above the geofences' names. It is also possible to choose the _All_ option — then the list will contain the geofences from all the resources to which the user has the necessary access right. The geofences in the list are sorted by name. To quickly find one, use the dynamic filter.

Besides, you can choose units as so-called 'moving geofences'. For them, set the radius to outline unit's area. Geofences and units on the lists are sorted by name. If the list is large, it is convenient to use name mask to quickly find necessary items. You can even set ride beginning at unit's area and ride end at an ordinary geofence.

![](https://docs.wialon.com/en/hosting/_media/tables/rides2.png)

If the _Counter_ column is selected for the table, you can indicate its mask in the _Sensors masks_ field on the _Settings_ tab. Besides, [intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) can be applied to this table: by duration, mileage, engine hours, speed range, trips, stops, parkings, sensor state, driver, trailer, fuel thefts, fillings, and geofences/units.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Note that the monitoring system provides a possibility of detecting geofence visit in case a trip intersects a geofence by any segment of its track. This option can be enabled in the [advanced settings](https://docs.wialon.com/en/hosting/user/reports/templ/settings/general) of a report template.

### Report on Rides <a id="report_on_rides"></a>

The report on rides gives the list of all performed rides. The table can contain the following information:

* **Ride** — this column specifies the start and end point of movement \(names of geofences or units are hyphenated\).
* **Ride from** — the departure geofence.
* **Ride to** — the destination geofence.
* **Beginning** — the date and time when the ride began.
* **End** — the date and time when the ride ended.
* **Mileage** — the distance traveled during the ride.
* **Mileage \(adjusted\)** — mileage subject to the coefficient set in unit properties \(_Advanced_ tab\).
* **Ride duration** — the amount of time spent to perform the ride.
* **Total time** — the time from the beginning of the first ride to the end of the last one.
* **Parkings duration** — the total amount of time spent on parkings during the trip.
* **Avg speed** — the average speed calculated for the ride.
* **Max speed** — the maximum speed registered during the ride.
* **Driver** — driver's name \(if identified\).
* **Trailer** — trailer's name \(if bound\).
* **Counter** — the counter sensor value \(can be helpful either in grouping table data by years/months/weeks/days/shifts or for the reports on unit groups\).
* **Initial counter** — the counter value at the beginning of the trip.
* **Finale counter** — the counter value at the end.
* **Avg temperature** — the average temperature value registered during a ride.
* **Min temperature** — the minimum temperature value registered during a ride.
* **Max temperature** — the maximum temperature value registered during a ride.
* **Initial temperature** — the temperature value at the beginning of a ride.
* **Final temperature** — temperature value at the end of a ride.
* **Count** — the number of rides.
* **Status** — the unit status registered during the current ride \(if there are several, the first one is displayed\).
* **Cargo weight** — the weight of a cargo transported within a trip between geofences.
* **Consumed** — the volume of consumed fuel detected by any sort of fuel sensor. If several such sensors are available, their values sum up.
* **Consumed by ImpFCS/AbsFCS/InsFCS/FLS/math** — the volume of consumed fuel detected by a fuel sensor \(such as impulse/absolute/instant fuel consumption sensor, fuel level sensor\) or calculated by math.
* **Avg consumption** — the average fuel consumption by any sort of fuel sensor. If several such sensors are available, their values sum up.
* **Avg consumption by ImpFCS/AbsFCS/InsFCS/FLS/math** — the average fuel consumption during the ride detected by one of the methods mentioned above.
* **Initial fuel level** — the fuel level at the beginning of the ride.
* **Final fuel level** — the fuel level at the end of the ride.
* **Max fuel level** — the maximum fuel level.
* **Min fuel level** — the minimum fuel level.
* **Penalties** — the penalties calculated for adjusted [_Eco Driving_](https://docs.wialon.com/en/hosting/cms/units/eco) criteria.
* **Rank** — the received penalty points converted into a grade using a 6-point scoring system.
* **Notes** — an empty column for your custom comments.

![](https://docs.wialon.com/en/hosting/_media/tables/rides.png)

More information on unfinished rides can be found [here](https://docs.wialon.com/en/hosting/user/reports/tables/unfinished).

