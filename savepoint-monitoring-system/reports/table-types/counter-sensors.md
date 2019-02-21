# Counter Sensors

This table shows the operation of the _Counter_ type [sensors](https://docs.wialon.com/en/hosting/cms/units/sensors/sensors). In the template, set the mask \(filter\) for sensors or select _All sensors_. A table can consist of the following columns:

* **Sensor** — the name of the sensor.
* **Activated** — the time of activation.
* **Deactivated** — the time of deactivation.
* **Duration** — operation time.
* **Total time** — the time from the beginning of the first activation to the end of the last.
* **Location** — the location at the moment of sending the data.
* **Mileage** — the distance traveled for the operation period.
* **Mileage \(adjusted\)** — mileage subject to the coefficient set in the unit properties on the _Advanced_ tab.
* **Avg speed** — the average speed at this interval.
* **Max speed** — the maximum speed at this interval.
* **Counter** — the value of the counter meter \(can be shown with an accuracy of hundreds — see [Report Settings –&gt; General](https://docs.wialon.com/en/hosting/user/reports/templ/settings/general)\).
* **Geofences/Units** — the column that includes the names of the geofences or units which were crossed during a given interval. The required geofences and units should be indicated in the [filtration parameters](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration). If at some interval there were several geofences or units like that, in the report there will be the name of the geofence with the smallest area or the name of the unit with the smallest radius of approximation. If the sizes coincide, all the names will be included.
* **Driver** — the name of the driver \(if available\).
* **Trailer** — the name of the trailer \(if it was bound\).
* **Penalties** — the penalties calculated for the adjusted [Eco Driving](https://docs.wialon.com/en/hosting/cms/units/eco) criteria.
* **Rank** — the received penalty points converted into a 6-point rating system.
* **Notes** — an empty column for your custom comments.

![](https://docs.wialon.com/en/hosting/_media/tables/counter.png)

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) The mileage values are displayed in the table as fractional numbers. However, when [exporting](https://docs.wialon.com/en/hosting/user/reports/query/export#excel) to an Excel file the values are rounded.

[Intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) can be applied to this table: by duration, mileage, engine hours, speed range, trips, stops, parkings, sensors, drivers, fuel fillings, fuel thefts, and geofences/units.

The value of the counter sensor can be visualized in the chart that shows the operation intervals of the counter and its value. You can learn more about charts [here](https://docs.wialon.com/en/hosting/user/reports/templ/contents/charts/charts).

![](https://docs.wialon.com/en/hosting/_media/tables/counter1.png)

