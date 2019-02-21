# Fuel Traffic

This report is designed to display the data about fuel fillings and thefts, as well as the intervals of operation of the counter sensor of the unit in one table.

For each type of activity \(fuel filling, theft, counter operation\) you can customize its [intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) in the parameters of the table. If in the filtration parameters there are other selected units and at the moment of activity they were close to the unit for which the report is executed, the algorithm of fuel fillings analysis is run. Thus, when executing, for example, a report on a tanker, one can see not only its fuel activity, but also the amount of fuel received by the units near it \(at least one message from such units should be received during the activity interval from a distance less than the radius specified in the filtration parameters\).

Read about setting the parameters used in the report in the [_Fuel Consumption_](https://docs.wialon.com/en/hosting/cms/units/fuel) and [_Sensor Properties_](https://docs.wialon.com/en/hosting/cms/units/sensors/props) sections.

The _Fuel Traffic_ report may include the following columns:

* **Beginning** — depending on the type \(see below\) — the [activation time](https://docs.wialon.com/en/hosting/user/reports/tables/counter) of the sensor, the [time of the fuel filling](https://docs.wialon.com/en/hosting/user/reports/tables/fillings) or [theft](https://docs.wialon.com/en/hosting/user/reports/tables/thefts).
* **End** — depending on the type — the deactivation time of the sensor, the time of the fuel filling or theft.
* **Duration** — the time from the beginning to the end \(0 for fuel fillings and thefts\).
* **Location** — the position of the unit while sending the data \(is associated with the _End_ field\).
* **Type** — the kind of the current activity determined by the system \(filling, theft, counter operation\).
* **Volume** — depending on the type — the quantity calculated by the counter sensor or the data from the _Filled_ or _Stolen_ columns taken from the columns of the same name in the corresponding tables.
* **Sensor name** — the name of the sensor by which the type was determined.
* **Geofences/Units** — the column that includes the names of the geofences or units with which an intersection was recorded during a given interval. Necessary geofences and units are indicated in the [filtration parameters](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration). If there are several geofences or units that have been triggered, the report displays the name of the geofence with the smallest surface or the name of the unit with the smallest radius of approximation. If the sizes coincide, all the names are included.
* **Filled** — the sum of the fuel fillings \(if any\) of the units shown in the _Geofences/Units_ column. Only the fillings registered automatically and the time of which is within the interval from _Beginning_ to _End_ are taken into account.
* **Deviation** — the difference between the values of the _Volume_ and _Filled_ columns.
* **Driver** — the name of the driver assigned to the unit on the current interval.
* **Notes** — an empty column where you can introduce your custom comments after you have printed or exported the report.

![](https://docs.wialon.com/en/hosting/_media/tables/fuel_traffic.png)

