# Engine Hours

The _Engine hours_ report shows how long the unit worked, how much time was in motion, how much fuel was spent for this period. Also, the duration and efficiency of the work of the attachable equipment can be shown.

To generate this report, the unit is supposed to have such [sensors](https://docs.wialon.com/en/hosting/cms/units/sensors/sensors) as ignition or absolute/relative engine hours sensor. The method of calculating engine hours is set in [Unit Properties –&gt; General](https://docs.wialon.com/en/hosting/cms/units/counters). In [Unit Properties –&gt; Advanced](https://docs.wialon.com/en/hosting/cms/units/adv) you can also set _Daily engine hours rate_ to calculate utilization and productivity.

There are two properties which can be used in engine hours report. They are [timeout](https://docs.wialon.com/en/hosting/cms/units/sensors/props#additional_properties) \(indicated for a sensor\) and [maximum interval between messages](https://docs.wialon.com/en/hosting/cms/units/adv#parameters_used_in_reports) \(set for a unit\). Both properties are used to cut off invalid intervals when the amount of engine hours is defined. If values for both timeout and maximum interval between messages are indicated, the system will use the property with the minimum value indicated.

Additionally, you can specify the daily engine hours. For this, enter the name mask of the engine hours sensor in a special filter in the report's template. It allows to create a separate table for each engine if there are several.

The table can contain the following columns:

![](https://docs.wialon.com/en/hosting/_media/tables/eh.png)

* **Beginning** — the time when the engine hours interval begins.
* **Initial location** — the location at that moment.
* **End** — the time when the engine hours interval ends.
* **Final location** — the location at that moment.
* **Engine hours** — the value of engine hours on the interval. For an accurate engine hours calculation, the equipment should send a valid parameter value of the engine sensor. In case of receiving an invalid value, it is necessary to [replace the sensor with validator](https://docs.wialon.com/en/hosting/cms/units/sensors/validation) using the correct value \(for example, 0\).
* **Initial engine hours** — the value of engine hours at the beginning of the interval.
* **Final engine hours** — the value of engine hours at the end of the interval.
* **Total time** — duration of the interval. If grouping by days is enabled, it shows the time from the beginning of the first engine hours interval to the end of the last interval.
* **Off-time** — the period of time passed from the end of the previous interval to the beginning of the current one \(determined starting from the second interval\).
* **In movement** — the interval of time during which the unit moved.
* **Idling** — the time when the unit was standing with the engine on. Note that idling cannot be detected if the equipment does not send messages containing speed value.
* **Mileage** — the distance traveled during the operating hours.
* **Mileage \(adjusted\)** — mileage subject to the coefficient set in the unit properties \(the _Advanced_ tab\).
* **Initial mileage** — the value of the mileage sensor at the moment of the beginning of the reporting period.
* **Final mileage** — the value of the mileage sensor at the end of the reporting period.
* **Avg speed** — average speed during the interval of engine operation.
* **Max speed** — the maximum speed during the interval of engine operation.
* **Counter** — the counter sensor value.
* **Initial counter** — the counter value at the beginning of the interval.
* **Finale counter** — the counter value at the end of the interval.
* **Avg engine revs** — the average rate of engine revolutions.
* **Max engine revs** — the maximum rate of engine revolutions.
* **Avg temperature** — the average temperature value registered for the interval of engine operation.
* **Min temperature** — the minimum temperature value registered for the interval of engine operation.
* **Max temperature** — the maximum temperature value registered for the interval of engine operation.
* **Initial temperature** — the temperature value at the beginning of engine hours operation.
* **Final temperature** — the temperature value the end of engine hours operation.
* **Status** — the status of the unit registered during engine hours operation \(if there are several, the first one is displayed\).
* **Cargo weight** — the weight of the transported cargo.
* **Driver** — the name of the driver \(if identified\).
* **Trailer** — the name of the trailer \(if it was bound\).
* **Movement productivity** — percentage ratio of engine hours in the movement to the duration of engine hours.
* **Engine efficiency duration** — the duration of the operation of attached equipment \(if there is the engine efficiency sensor\).
* **Engine efficiency idling** — the engine operation time after deduction of efficiency time \(total engine hours subtract engine efficiency duration\).
* **Utilization** — the percentage ratio of the duration of engine hours to engine hours rate \(engine hours divided by daily engine hours rate indicated in the unit properties\).
* **Useful utilization** — the percentage ratio of the duration of engine efficiency to the engine hours rate.
* **Productivity** — the percentage ratio of the duration of engine efficiency to the duration of engine hours.
* **Consumed** — the volume of consumed fuel detected by any sort of fuel sensor. If several sensors are available, their values sum up.
* **Consumed by ImpFCS/AbsFCS/InsFCS/FLS/math/rates** — the fuel volume used in engine hours. It can be detected by a fuel sensor \(such as impulse/absolute/instant fuel consumption sensor, fuel level sensor\) or calculated by math or rates. [Here](https://docs.wialon.com/en/hosting/user/reports/dat/dat#fuel_in_reports) you can find more details about fuel in reports.
* **Avg consumption** — the average fuel consumption by any sort of fuel sensor. If several sensors are available, their values sum up.
* **Avg consumption by …** — the average consumption in engine hours.
* **Consumed in motion by …** — the fuel volume used in engine hours while moving.
* **Avg consumption in motion by …** — the average consumption in engine hours while moving.
* **Consumed in idle run by …** — the fuel volume used in engine hours during idle running.
* **Avg consumption in idle run by …** — the average fuel consumption in idling.
* **Avg consumption by … in trips** — the average fuel consumption in trips.
* **Initial fuel level** — the fuel level at the beginning of the interval.
* **Final fuel level** — the fuel level at the end of the interval.
* **Max fuel level** — the maximum fuel level.
* **Min fuel level** — the minimum fuel level.
* **Penalties** — the penalties calculated for the adjusted [Eco Driving](https://docs.wialon.com/en/hosting/cms/units/eco) criteria.
* **Rank** — the received penalty points converted into a grade using 6 point scoring system.
* **Notes** — an empty column for your custom comments.

For the engine hours report, you can apply [intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) by duration, mileage, engine hours, speed range, trips, stops, parkings, sensors, driver, trailer, fuel fillings, fuel thefts, and geofences/units. If the engine hours are counted according to the engine hours sensor, it is possible to filter the intervals not only by the duration of their operation \(i.e., the duration of their on-state\), but also by the value of the engine hours sent by the sensor itself.

