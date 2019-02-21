# Summary

The tabular report _Summary_ allows you to display a variety of generalizing data related to the reporting interval and, at the same time, not tied to any conditions \(such as trips, sensor operation, geofence visits, etc.\). In other words, the summary report processes all the messages for the indicated period, regardless of how long the unit worked and was in motion.

The following columns can be included:

* **Mileage in trips** — the mileage on the interval taking the trip detector into account.
* **Mileage in all messages** — the mileage for the reporting interval by the mileage counter.
* **Mileage \(adjusted\)** — the mileage on the interval by the mileage counter multiplied by the [mileage coefficient](https://docs.wialon.com/en/hosting/cms/units/adv#mileage_coefficient) \(a setting in the unit properties\). More information about the mileage in reports can be found [here](https://docs.wialon.com/en/hosting/user/reports/dat/dat#mileage).
* **Avg speed** — the average speed on the interval.
* **Max speed** — the maximum speed on the interval. More information about the speed in reports can be found [here](https://docs.wialon.com/en/hosting/user/reports/dat/dat#mileage).
* **Move time** — the time in trips.
* **Engine hours** — the time of engine hours operation.
* **Engine efficiency duration** — the duration of operation of the attached implements \(if there is an engine efficiency sensor\).
* **Parkings** — the total time of parkings on the interval.
* **Counter** — the counter sensor value.
* **Initial counter** — the counter value at the beginning of the interval.
* **Final counter** — the counter value at the end of the interval.
* **Custom sensor initial value** — the custom sensor value at the beginning of the interval. If there are more than one custom sensors, a separate column is built for each of them and the name is written in brackets. The name masks of custom sensors can be indicated on the right-hand side of the template dialog.
* **Custom sensor final value** — the value of the custom sensor at the end of the interval.
* **Difference** — the difference between the initial and final values of the custom sensor.
* **Utilization** — the percentage ratio of the duration of engine hours to the engine hours rate \(engine hours divided by daily engine hours rate indicated in the unit properties\).
* **Useful utilization** — the percentage ratio of the duration of engine efficiency to the engine hours rate.
* **Productivity** — the percentage ratio of the duration of engine efficiency to the engine hours duration.
* **Consumed** — the volume of consumed fuel detected by any sort of fuel sensor. If several such sensors are available, their values sum up.
* **Consumed by…** — the volume of consumed fuel detected by a fuel sensor \(such as impulse/absolute/instant fuel consumption sensor, fuel level sensor\) or calculated by math or rates. Besides, in the report template \(on the right\) you can specify additional parameters to calculate fuel: throughout the reporting period, in trips or in engine hours.
* **Avg consumption** — the average fuel consumption by any sort of fuel sensor. If several such sensors are available, their values sum up.
* **Avg consumption by…** — the average fuel consumption on the interval. More details about the fuel in reports can be found [here](https://docs.wialon.com/en/hosting/user/reports/dat/dat#fuel_in_reports).
* **Avg mileage per unit of fuel by …** — the average mileage per unit of fuel based on the indications of a particular sensor.
* **Initial fuel level** — the counter value at the beginning of the interval.
* **Final fuel level** — the counter value at the end of the interval.
* **Total fillings** — the number of the detected fuel fillings.
* **Total thefts** — the number of the detected fuel thefts.
* **Filled** — the volume of filled fuel \(only fuel fillings detected by a sensor\).
* **Stolen** — the volume of stolen fuel.
* **Penalties** — the penalties calculated for the adjusted [Eco Driving](https://docs.wialon.com/en/hosting/cms/units/eco) criteria.
* **Rank** — the received penalty points converted into a grade using a 6-point scoring system.

Fuel can be calculated for the whole interval, in trips or in engine hours, which is selected in the additional parameters of the table. This option affects such columns as _Consumed…_ and _Avg consumption…_.

As additional settings, you can specify masks for sensors \(fuel, counters\), including the engine hours sensor.

The [_Retrieve Intervals_](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/parameters#retrieve_intervals) option is available for this table if grouping by shifts is configured for it or if a value in the field _Summary by:_ is selected.

The _Summary_ table is presented by one row — the summarized data for a selected period of time. However, the report template parameters for this table contain an individual option — _Summary by_. This option allows to select a time interval \(shifts/days/weeks/months\) according to which the table data is arranged. This option can be used either in the reports for units or in [reports for units groups](https://docs.wialon.com/en/hosting/user/reports/adv/group).

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Note._  
Often a value received from the analog sensor may differ from the corresponding value in the _Total_ row. It is stipulated by the analog data leaping, and application of grouping by days/weeks/months towards the values received as a result of processing such data. In other words, the analog data values \(with or without leaps\) are divided into intervals and then summarized. That is why the value of the summarized intervals can be sufficiently different from the value not divided into intervals. And since the values in the _Total_ row are not divided into intervals, you can receive the difference compared to the values from the analog sensors. For example, calculating fuel, a value in the _Consumed by FLS_ column may differ from the corresponding value in the _Total_ row.

