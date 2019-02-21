# Unfinished Rides

See the [Rides](https://docs.wialon.com/en/hosting/user/reports/tables/rides) topic to learn how to prepare rides for this report.

A ride is considered to be unfinished when the unit leaves the starting point, and then, not having visited any of the final points, again appears in the point marked as the beginning. It can be the same zone from where the unit left \(if circle rides are not allowed\) or some other geofence with a starting point mark.

The following columns are available for the report:

* **Ride** — the departure and destination point.
* **Ride from** — the departure point.
* **Ride to** — the destination point.
* **Beginning** — the date and time when the ride began.
* **End** — the date and time when the ride ended.
* **Mileage** — the distance traveled during the ride.
* **Mileage \(adjusted\)** — the mileage subject to the coefficient set in the unit properties on the _Advanced_ tab.
* **Ride duration** — the amount of time it took to perform the ride.
* **Total time** — the time from the beginning of the first ride to the end of the last ride.
* **Parkings duration** — the time spent on parkings.
* **Avg speed** — the average speed calculated for the ride.
* **Max speed** — the maximum speed registered during the ride.
* **Driver** — driver's name \(if identified\).
* **Trailer** — trailer's name \(if bound\).
* **Counter** — the counter sensor value.
* **Initial counter** — the value of a counter at the moment of leaving a departure geofence.
* **Final counter** — the value of the counter at the moment of entering a destination end.
* **Count** — the number of rides \(can be helpful either when grouping the table data by years/months/weeks/days/shifts or for the reports on unit groups\).
* **Status** — the unit status registered during the current ride \(if there are several, the first one is displayed\).
* **Consumed** — the volume of consumed fuel detected by any sort of fuel sensor. If several such sensors are available, their values sum up.
* **Consumed by ImpFCS/AbsFCS/InsFCS/FLS/math/rates** — the volume of consumed fuel detected by a fuel sensor \(such as impulse/absolute/instant fuel consumption sensor, fuel level sensor\) or calculated by math or rates. More information on fuel in reports can be found [here](https://docs.wialon.com/en/hosting/user/reports/dat/dat#fuel_in_reports).
* **Avg consumption** — the average fuel consumption by any sort of fuel sensor. If several such sensors are available, their values sum up.
* **Avg consumption by ImpFCS/AbsFCS/InsFCS/FLS/math/rates** — the average fuel consumption during the ride detected by one of the methods mentioned above.
* **Initial fuel level** — the fuel level at the beginning of the ride.
* **Final fuel level** — the fuel level at the end of the ride.
* **Max fuel level** — the maximum fuel level.
* **Min fuel level** — the minimum fuel level.
* **Penalties** — the penalties calculated for the adjusted [_Eco Driving_](https://docs.wialon.com/en/hosting/cms/units/eco) criteria.
* **Rank** — the received penalty points converted into a grade using a 6-point scoring system.
* **Notes** — an empty column for your custom comments.

![](https://docs.wialon.com/en/hosting/_media/tables/unfinished.png)

See the [Rides](https://docs.wialon.com/en/hosting/user/reports/tables/rides) section to find out more information about the additional parameters for _Unfinished rides_.

