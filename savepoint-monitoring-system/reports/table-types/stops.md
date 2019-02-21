# Stops

A stop is one or more consecutive messages with a zero speed. Stops can be registered at lights, intersections, in traffic jams, etc.

Stops should be distinguished from [parkings](https://docs.wialon.com/en/hosting/user/reports/tables/parkings). Parameters to detect trips, parkings, and stops are adjusted in the [trip detector](https://docs.wialon.com/en/hosting/cms/units/trip). If there are several messages in succession, they are united in one stop. If total time of such a stop reaches _Minimum parking time_, it is registered as a parking \(not a stop\).

The following information is presented in this kind of report:

* **Beginning** — the time when the stop started.
* **End** — the time when the stop ended.
* **Duration** — the total time of the stop.
* **Total time** — the time from the beginning of the first stop to the end of the last stop.
* **Off-time** — the time from the end of the previous stop to the beginning of the current one \(to be defined beginning from the second stop\).
* **Location** — the address where the unit stopped.
* **Coordinates** — the coordinates of the unit at the moment of a stop \(in decimal degrees\).
* **Driver** — the name of the driver \(if available\).
* **Trailer** — the name of the trailer \(if bound\).
* **Count** — the number of stops.
* **Counter** — the counter sensor values \(can be helpful either in grouping table data by years/months/weeks/days/shifts or for the reports on unit groups\).
* **Notes** — an empty column for your custom comments.
* **Avg weight** — the average weight value registered for the stop interval.
* **Min weight** — the minimum weight value registered for the stop interval.
* **Max weight** — the maximum weight value registered for the stop interval.
* **Initial weight** — the weight value at the beginning of the stop interval.
* **Final weight** — the weight value at the end of the stop interval.

![](https://docs.wialon.com/en/hosting/_media/tables/stops.png)

See [Data in Reports](https://docs.wialon.com/en/hosting/user/reports/dat/dat#time_in_reports) to learn how time \(duration\) can be formatted.

[Intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) \(by stop duration, sensor state, driver, trailer, fuel fillings and thefts\) can be applied to this table.

This kind of report can be supplemented with the corresponding [markers](https://docs.wialon.com/en/hosting/user/reports/templ/settings/map#markers) on the map.

![](https://docs.wialon.com/en/hosting/_media/tables/markers-stops.png)

