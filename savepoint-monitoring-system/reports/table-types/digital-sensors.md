# Digital Sensors

Usually, digital sensors have two states: on/off, activated/deactivated, etc. For example, it can be an ignition or cargo load sensor. All sensors are configured in [Unit Properties –&gt; Sensors](https://docs.wialon.com/en/hosting/cms/units/sensors/sensors).

To receive the information about a specific sensor, specify its name or part of the name using wildcard symbols — an asterisk \* \(replaces several characters\) or question mark **?** \(replaces one symbol\). The sensor name cannot contain commas. If the sensor mask is not specified, the information in the table is displayed for all sensors of the unit.

The table can contain the following columns:

* **Sensor** — the name of the controlled sensor.
* **Activated** — the time from the first message that contains information about the activation of the sensor.
* **Deactivated** — the time when the sensor was deactivated.
* **Duration** — the interval when the sensor was on.
* **Total time** — the time from the beginning of the first activation to the end of the last one.
* **Location** — the location of the unit at the moment of activation.
* **Mileage** — the distance traveled while the sensor was on.
* **Mileage \(adjusted\)** — mileage subject to the coefficient set in the unit properties \(the _Advanced_ tab\).
* **Initial mileage** — the mileage sensor value at the moment of a sensor activation. If the mileage parameter was not saved at the reporting interval, the mileage is counted from zero.
* **Final mileage** — the mileage sensor value at the time the sensor is turned off.
* **Avg speed** — the average speed of movement with the sensor on.
* **Max speed** — the maximum speed with which the unit moved with the sensor turned on.
* **Activations count** — the number of activations \(can be helpful either in grouping table data by years/months/weeks/days/shifts or for the reports on unit groups\).
* **Driver** the name of the driver \(if available\).
* **Trailer** — the name of the trailer \(if it was bound\).
* **Penalties** — penalties calculated for the adjusted [Eco Driving](https://docs.wialon.com/en/hosting/cms/units/eco) criteria.
* **Rank** — penalty points, converted to the 6-point rating system.
* **Notes** — an empty column for your custom comments.
* **Custom sensor initial value** — the custom sensor value at the moment of activation of the digital sensor.
* **Custom sensor final value** — the custom sensor value at the moment of deactivation of the digital sensor.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) If there are several custom sensors, separate columns with initial and final values are displayed for each of them. The name of each custom sensor and units of measurement \(if they were specified when creating the sensor\) are indicated next to the name of each of these columns in parenthesis. In case there are no suitable sensors, the columns are not displayed.

![](https://docs.wialon.com/en/hosting/_media/tables/digital.png)

[Intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) can be applied to this table: by duration, mileage, engine hours, speed range, trips, stops, parkings, driver, trailer, fuel fillings, fuel thefts and geofences/units.

