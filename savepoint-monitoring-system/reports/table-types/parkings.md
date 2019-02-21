# Parkings

Parkings are estimated according to the parameters set in the [Trip Detection](https://docs.wialon.com/en/hosting/cms/units/trip) when configuring a unit. To get the information as accurate as possible, it is advised that you configure each parameter individually for every piece of equipment.

A parking is an interval of time when the following conditions are met:

1. **Insignificant speed**. The speed detected must fall in the range from 0 to the _Minimum moving speed_. When this speed is reached, the behavior of the unit is regarded as a movement \(=trip\), if by the time and distance traveled it corresponds to the trip definition \(the _Minimum trip time_ and _Minimum trip distance_ parameters\). The parking, respectively, ends. However, if the time or distance traveled does not fit the scope of the trip, the parking is prolonged.  
2. **Sufficient time interval**. This speed must continue for a period of time \(and not less than _Minimum parking time_\). If this time is not reached, the behavior of the unit is not regarded as parking, but as a stop.  
3. **Insignificant location change**. As it has been noted above, parking is also considered an insignificant movement in space, that is, a movement that does not exceed the _Minimum trip distance_ parameter, if it is equal to or greater than the _Minimum parking time_ parameter.

The following information is presented in this kind of report:

* **Beginning** — the time when the parking started.
* **End** — the time when the parking ended.
* **Duration** — the time interval of a parking.
* **Total time** — the time from the beginning of the first parking to the end of the last parking.
* **Off-time** — the time interval from the end of the previous parking to the beginning of the current parking \(defined starting from the second parking\).
* **Location** — the address where the unit was stationary. If there was an insignificant movement detected, the initial address is used.
* **Coordinates** — the coordinates of the unit during the parking \(in decimal degrees\).
* **Driver** — the name of the driver \(if available\).
* **Trailer** — the name of the trailer \(if one was bound\).
* **Counter** — the values of the counter sensor.
* **Initial counter** — the counter value at the beginning of the parking.
* **Finale counter** — the counter value at the end of the parking.
* **Avg temperature** — the average temperature value registered for the parking interval.
* **Min temperature** — the minimum temperature value registered for the parking interval.
* **Max temperature** — the maximum temperature value registered for the parking interval.
* **Initial temperature** — the temperature value at the beginning of the parking interval.
* **Final temperature** — the temperature value at the end of the parking interval.
* **Avg weight** — the average weight value registered for the parking interval.
* **Min weight** — the minimum weight value registered for the parking interval.
* **Max weight** — the maximum weight value registered for the parking interval.
* **Initial weight** — the weight value at the beginning of the parking interval.
* **Final weight** — the weight value at the end of the parking interval.
* **Status** — the status of the unit registered during the current parking interval \(if there are several, the first one is displayed\).
* **Count** — the number of parkings \(useful when grouping rows by years/months/weeks/days/shifts or for the reports on unit groups\).
* **Notes** — an empty column for your custom comments.

![](https://docs.wialon.com/en/hosting/_media/tables/parkings.png)

See [Data in Reports](https://docs.wialon.com/en/hosting/user/reports/dat/dat#time_in_reports) to learn how time \(duration\) can be formatted.

The [intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) \(by parking duration, sensor state, driver, trailer, fuel fillings/thefts, and geofences/units\) can be applied to this table.

The parkings can be displayed on the map. To make use of this feature, select [Parking markers](https://docs.wialon.com/en/hosting/user/reports/templ/settings/map#markers) in the report template.

![](https://docs.wialon.com/en/hosting/_media/tables/markers-parkings.png)

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Attention!_  
Parkings should be distinguished from [stops](https://docs.wialon.com/en/hosting/user/reports/tables/stops).

