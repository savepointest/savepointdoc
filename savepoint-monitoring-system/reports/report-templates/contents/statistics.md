# Statistics

Statistics is a table consisting of two columns where the first one contains the parameters you have chosen, and the second one shows their values.

![](https://docs.wialon.com/en/hosting/_media/reports/statistics.png)

The statistics table gives information on the report as a whole, for example, on the beginning and end of the report interval, the number of messages, the name of the unit, the time zone, the time of report execution, and other statistics, depending on the selected [type of template](https://docs.wialon.com/en/hosting/user/reports/templ/templ#creating_a_report_template).

To add a statistics table to a report template, click the _Statistics_ button on the [_Contents_](https://docs.wialon.com/en/hosting/user/reports/templ/contents/contents) tab of its properties.

In the dialog window of the _Statistics_ table properties, mark the points you want to include in the table. To find the required ones, use the [dynamic search](https://docs.wialon.com/en/hosting/user/gui/masks#dynamic_search), located in the upper right corner. Search is carried out both by the name of the line \(the left column\) and by the subgroup to which it belongs to \(right\).

![](https://docs.wialon.com/en/hosting/_media/reports/statistics1.png)

To change the name of a table item, click on it with the left mouse button and make the changes. To cancel changes, click on the _Default_ button ![](https://docs.wialon.com/en/hosting/_media/icons/rename.png) \(the button is inactive if the name has not been changed\).

You can also change the order of the rows. To do this, drag up or down the _double arrow_ button to the left of the name of the desired line.

The statistics table is added to the list of contents of the report template. It always goes first and cannot be moved.

The following items are available for display in the statistics table for the reports of the _Units_ type.

**Statistics**

* **Report** — the name of the report template.
* **Unit** — the name of the unit.
* **Report execution time** — the time of report generation when a user executed the report online or it was generated automatically as a job or notification.
* **Interval beginning** — the beginning of the reporting interval.
* **Interval end** — the end of the reporting interval.
* **Time zone** — the time zone as it is set in user settings.
* **Messages** — the messages analyzed within the reporting period.
* **Mileage in all messages** — the mileage in all messages according to the selected mileage counter \(without filtration by the trip detector\).
* **Consumed** — the volume of consumed fuel detected by any sort of fuel sensor. If several such sensors are available, their values sum up.
* **Consumed by ImpFCS/AbsFCS/InsFCS/FLS/math/rates** — the volume of consumed fuel detected by a fuel sensor \(such as impulse/absolute/​instant fuel consumption sensor, fuel level sensor\) or calculated by math or rates.
* **Avg consumption** — the average fuel consumption by any sort of fuel sensor. If several such sensors are available, their values sum up.
* **Avg consumption by ImpFCS/​AbsFCS/​InsFCS/​FLS/​math/rates** — the average fuel consumption in trips detected by one of the methods mentioned above. It can be presented either as liters per 100 kilometers or miles per one gallon. The whole mileage of the reported interval is normally taken for these calculations. However, average consumption by FLS can take either all mileage or mileage by the trip detector. ​
* **Initial fuel level** — the fuel level at the beginning of the interval.
* **Final fuel level** — the fuel level at the end of the interval.
* **Max fuel level** — the maximum fuel level.
* **Min fuel level** — the minimum fuel level. More information about the fuel in reports can be found [here](https://docs.wialon.com/en/hosting/user/reports/dat/dat#fuel_in_reports).

**Engine hours**

* **Engine hours** — the duration of the [engine hours](https://docs.wialon.com/en/hosting/user/reports/tables/eh). It can be calculated by the engine hours sensor or by the ignition sensor depending on the unit properties.
* **Initial engine hours** — the value of the engine hours at the beginning of the interval.
* **Final engine hours** — the value of engine hours at the end of the interval.
* **In movement** — the time interval during which the unit was in motion.
* **Idling** — a total time interval during which the unit did not move with the engine running \(idling\).
* **Mileage in engine hours** — the distance traveled during the engine hours operation.
* **Initial mileage in engine hours** — the value of the mileage sensor at the moment of the beginning of the reporting period.
* **Final mileage in engine hours** — the value of the mileage sensor at the end of the reporting period.
* **Avg engine revs** — the average rate of engine revolutions.
* **Max engine revs** — the maximum rate of engine revolutions.
* **Avg temperature in e/h** — the average temperature during the engine hours.
* **Engine efficiency duration** — the duration of the attached implements operation \(if there is an engine efficiency sensor\).
* **Engine efficiency idling** — the engine hours minus the engine efficiency time.
* **Utilization** — the duration of the engine hours work divided by the engine hours rate, indicated on the _Advanced_ tab of the device properties.
* **Useful utilization** — the duration of the engine efficiency divided by the engine hours rate.
* **Productivity** — the duration of the engine efficiency divided by the engine hours duration.
* **Consumed in e/h** — the volume of the consumed fuel detected by any sort of fuel sensor. If several such sensors are available, their values sum up.
* **Consumed by ImpFCS/AbsFCS/InsFCS/FLS/math/rates in e/h** — the fuel volume used in engine hours. It can be detected by a fuel sensor \(such as impulse/absolute/instant fuel consumption sensor, fuel level sensor\) or calculated by math or rates. More information about the fuel in reports can be found [here](https://docs.wialon.com/en/hosting/user/reports/dat/dat#fuel_in_reports).
* **Avg consumption in e/h** — the average fuel consumption by any sort of fuel sensor. If several such sensors are available, their values sum up.
* **Avg consumption by ImpFCS/AbsFCS/InsFCS/FLS/math/rates in e/h** — the average fuel consumption in the engine hours determined in accordance with a fuel sensor readings or calculated by math or rates.
* **Consumed by ImpFCS/AbsFCS/InsFCS/FLS/math/rates in motion** — the average fuel consumption in motion.
* **Avg consumption by ImpFCS/AbsFCS/InsFCS/FLS/math/rates in motion** — the amount of fuel consumed at idle determined in accordance with a fuel sensor readings or calculated by math or rates.
* **Consumed by ImpFCS/AbsFCS/InsFCS/FLS/math/rates in idle run** — the fuel volume used in the engine hours during idle running determined in accordance with a fuel sensor readings or calculated by math or rates.
* **Avg consumption by ImpFCS/AbsFCS/InsFCS/FLS/math/rates in e/h in trips** — the average fuel consumption during the work of engine hours in trips determined in accordance with a fuel sensor readings or calculated by math or rates.

**Events**

* **Events count** — the number of the registered [events](https://docs.wialon.com/en/hosting/user/reports/tables/events).

**Fuel fillings**

* **Total filled** — the volume of fuel filled during the reporting interval.
* **Total registered** — the registered fuel volume regardless of binding to sensors and calculation methods.
* **Difference** — the difference between the registered and detected fillings.
* **Total fillings** — the number of fuel fillings detected within the reporting period.

**Fuel thefts**

* **Total fuel stolen** — the total volume of stolen fuel.
* **Total thefts** — the number of thefts detected within the reporting period.

**SMS messages**

* **SMS messages** — the number of SMS messages received from a unit.

**Speedings**

* **Initial mileage** — the mileage sensor reading at the time of the start of the first speeding at the reporting interval. If there is no mileage sensor, the mileage is counted from 0.
* **Final mileage** — the mileage sensor reading at the end of the speeding interval.

**Parkings**

* **Parking time** — the total duration of [parkings](https://docs.wialon.com/en/hosting/user/reports/tables/parkings) for the reporting period. Parking is determined by the trip detector. If it is disabled, the number of parkings is counted as zero.
* **Parkings count** — the number of parkings for the reporting period.

**Trips**

* **Move time** — the total duration of all trips.
* **Engine hours** — the engine hours of attachable equipment.
* **Mileage in trips** — the total distance traveled in all trips.
* **Mileage \(adjusted\)** — the total mileage of the movement intervals determined by the trip detector, multiplied by [mileage coefficient](https://docs.wialon.com/en/hosting/cms/units/adv) \(the setting in the additional properties of the unit\).
* **Urban mileage in trips** — the distance traveled at a speed that is defined as the speed in the city.
* **Suburban mileage in trips** — the distance traveled at a speed that is defined as the speed outside the city. [Urban speed limit](https://docs.wialon.com/en/hosting/cms/units/adv) is configured in the additional settings of the unit.
* **Initial mileage** — the mileage sensor value at the beginning of the reporting interval \(it makes sense if there is an absolute odometer\).
* **Final mileage** — the mileage sensor value at the end of the reporting interval.
* **Toll roads mileage** — the distance that a unit traveled during the trip on the roads on which the _Platon_ system is used.
* **Toll roads cost** — a sum of money \(in RUB\) for the toll roads mileage calculated on the basis of the covered distance and the _Platon_tariff.
* **Average speed in trips** — the average speed in trips \(total mileage divided by the time of travel\).
* **Maximum speed in trips** — the maximum speed registered during the trips.
* **Trips count** — the number of trips.
* **Consumed in trips** — the volume of consumed fuel detected by any sort of fuel sensor. If several sensors are available, their values sum up.
* **Consumed by ImpFCS/AbsFCS/InsFCS/FLS/math/rates in trips** — the fuel consumed in trips. It can be detected by a fuel sensor \(such as impulse/absolute/instant fuel consumption sensor, fuel level sensor\) or calculated by math or rates. More information about fuel in reports can be found [here](https://docs.wialon.com/en/hosting/user/reports/dat/dat#fuel_in_reports).
* **Rates deviation by ImpFCS/AbsFCS/InsFCS/FLS in trips** — the difference between the fuel consumption detected by a sensor and the fuel consumption rates.
* **Avg consumption in trips** — the average fuel consumption by any sort of fuel sensor. If several such sensors are available, their values sum up.
* **Avg consumption by ImpFCS/AbsFCS/InsFCS/FLS/math/rates in trips** — the average fuel consumption in trips determined in accordance with a fuel sensor readings or calculated by math or rates.
* **Avg mileage per unit of fuel by ImpFCS/AbsFCS/InsFCS/FLS/math/rates in trips** — the average fuel consumption presented as _kilometers per liter_ or as _miles per gallon_.

**Violations**

* **Violations count** — the number of [violations](https://docs.wialon.com/en/hosting/user/reports/tables/violations) registered within the reporting period.

**Executed commands**

* **Executed commands** — the number of [commands](https://docs.wialon.com/en/hosting/user/monitor/cmd) sent to a unit.

**Unit latest data**

All the items in this section do not depend on the reporting interval. The latest information is taken at the moment of the report execution.

* **Mileage counter** — the mileage counter value.
* **Engine hours counter** — the engine hours counter value.
* **GPRS traffic counter** — the consumed traffic.
* **Unit last location** — the latest unit location detected \(address or coordinates\).
* **Last message time** — the time when the latest message from the unit was received.

**Visited streets**

* **Streets count** — the number of visits of [streets](https://docs.wialon.com/en/hosting/user/reports/tables/streets).

**Maintenance**

* **Total maintenance duration** — duration of all registered services.
* **Total maintenance cost** — total cost of all maintenance works.
* **Services count** — the number of services performed.

Typically, for all of the points mentioned above, you can make more detailed reports, presented in the form of tables or charts, described above.

**Utilization cost**

* **Total utilization cost** — the total cost of all registered service works and fuel fillings.
* **Count of services and fillings** — the total number of all registered service works and fuel fillings.

**Counter sensors**

* **Total counter** — the sum of values of all sensors of the _counter_ type.

**Images**

* **Images** — the number of [images](https://docs.wialon.com/en/hosting/user/monitor/pics) received from unit. And if there are any, the resulting report contains a section with all the received images for the reporting period. Supported format is JPEG.

**Eco driving**

* **Penalties** — the overall penalty for various [Eco Driving](https://docs.wialon.com/en/hosting/cms/units/eco) criteria for the reporting period.
* **Rank** — the received penalty points converted into a grade using a 6-point scoring system.

**Video**

The list of video files received from a unit.

**Orders**

* **Total orders** — the total amount of [orders](https://docs.wialon.com/en/hosting/user/reports/tables/orders) within the indicated time period.
* **Orders visited** — orders in which the arrival of a courier to an address is detected or any status is set.
* **Orders visited in time** — orders in which the arrival of a courier to an address is detected on time \(in advance\) or any status is set.
* **Orders visited late** — orders in which the arrival of a courier to an address is detected late or any status is set late.
* **Non-visited orders** — orders in which the arrival of a courier to an address is not detected.
* **Orders fulfilled** — orders in which the arrival of a courier to an address is detected, the _Confirm_ status is set.
* **Orders fulfilled in time** — orders which are fulfilled on time \(in advance\), the _Confirm_ status is set.
* **Orders fulfilled late** — orders which are fulfilled late, the _Confirm_ status is set.
* **Orders visited without status** — orders in which the arrival of a courier to an address is detected, a status is not set.
* **Orders rejected** — orders for which the _Reject_ status is set.
* **Order's avg time \(estimated\)** — the ratio of the time calculated by the system for the delivery of all orders to the total number of orders.
* **Order's avg time \(actual\)** — the ratio of time spent delivering orders to a total amount of orders.
* **Avg time deviation in orders** — the difference between the actual and estimated average time for delivery of an order.
* **Order's avg mileage \(actual\)** — the ratio of a distance covered by a courier to a total amount of orders.
* **Order's avg weight** — the ratio of the total weight of orders to their total number.
* **Order's avg volume** — the ratio of the total volume of orders to a total amount of orders.
* **Order's avg cost** — the ratio of total cost of orders to a total amount of orders.
* **Avg fuel consumption for an order** — the ratio of a total amount of fuel consumed to a total amount of orders.
* **Orders' estimated mileage** — the total distance calculated by the system for the delivery of orders.
* **Orders' actual mileage** — the total distance covered by a courier delivering orders.
* **Fuel consumed in orders** — the total amount of fuel consumed while delivering orders.
* **Orders' total weight** — the overall weight of all created orders.
* **Orders' total volume** — the overall volume of all created orders.
* **Orders' total cost** — the overall cost of all created orders.

Moreover, the following data may be included in the statistics for orders:

* **Percentage of orders visited in time**;
* **Percentage of orders visited late**;
* **Percentage of non-visited orders**;
* **Percentage of orders fulfilled in time**;
* **Percentage of orders fulfilled late**;
* **Percentage of orders visited without status**;
* **Percentage of orders rejected**.

If the report is executed not for the unit, then, depending on the type of the report template, the statistics includes the data listed below.  


| **Report template type** | **Statistics data** |
| :--- | :--- |
| **Unit group** | _Статистика_: Report; Group; Interval beginning; Interval end; Report execution time. |
| **User** | _Статистика_: Report; User; Interval beginning; Interval end; Report execution time; _Logins_: Time spent on site; Logins count. |
| **Driver** | _Bindings_: In movement; Idling; _Statistics_: Report; Driver; Interval beginning; Interval end; Report execution time; _Orders_: Total orders; Orders visited; Orders visited in time; Orders visited late; Non-visited orders; Orders fulfilled; Orders fulfilled in time; Orders fulfilled late; Orders visited without status; Orders rejected; Percentage of orders visited in time; Percentage of orders visited late; Percentage of non-visited orders; Percentage of orders fulfilled in time; Percentage of orders fulfilled late; Percentage of orders visited without status; Percentage of orders rejected; Order's avg time \(estimated\); Order's avg time \(actual\); Avg time deviation in orders; Order's avg mileage \(actual\); Order;s avg weight; Order's avg volume; Order's avg cost; Avg fuel consumption for an order. |
| **Trailer** | _Statistics_: Report; Trailer; Interval beginning; Interval end; Report execution time. |
| **Resource** | _Statistics_: Report; Resource; Interval beginning; Interval end; Report execution time; SMS sent; SMS available.  ![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) The number of text messages that are displayed in these fields does not depend on the interval of report execution. The information is displayed for the period corresponding to the _Reset_ option on the [_Services_](https://docs.wialon.com/en/hosting/cms/billing/features) tab of the tariff billing properties. |
| **Retranslator** | _Statistics_: Report; Retranslator; Interval beginning; Interval end; Report execution time. |
| **Route** | _Statistics_: Report; Route; Interval beginning; Interval end; Report execution time. |
| **Group of drivers** | _Bindings_: In movement; Idling; _Statistics_: Report; Group of drivers; Interval beginning; Interval end; Report execution time. |
| **Group of trailers** | _Statistics_: Report; Group of trailers; Interval beginning; Interval end; Report execution time. |
| **Passengers** | _Statistics_: Report; Passenger; Interval beginning; Interval end; Report execution time. |
| **Group of passengers** | _Статистика_: Report; Group of passengers; Interval beginning; Interval end; Report execution time. |

As a rule, for all of the above points, you can make more detailed reports in the form of tables or charts, described above.

