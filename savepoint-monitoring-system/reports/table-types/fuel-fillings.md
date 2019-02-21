# Fuel Fillings

This report shows where and when a vehicle was filled up. The parameters for the report are set in [Unit Properties –&gt; Fuel Consumption](https://docs.wialon.com/en/hosting/cms/units/fuel). This report is generated on the basis of fillings [registered manually](https://docs.wialon.com/en/hosting/user/monitor/reg#fuel_filling) or detected by sensors. The table cannot be generated if no fuel fillings are found for the indicated time interval.

This report may include the following columns:

* **Time** — the moment of the most significant change in the fuel level.
* **Location** — the location of the unit at the time of filling \(if a filling is registered manually, the location of the unit is detected on the basis of the messages received at the time of filling registration\).
* **Initial fuel level** — the fuel level before the filling.
* **Final fuel level** — the fuel level after the filling.
* **Filled** — the volume of filled fuel \(the name of the sensor can be indicated in parenthesis\).
* **Registered** — the volume of registered fuel.
* **Difference** — the difference between the detected and registered filling volume.
* **Description** — a brief description indicated during the manual registration of fuel filling.
* **Sensor** — the sensor which detected the filling.
* **Driver** — the name of the driver \(if identified\).
* **Trailer** — the name of the trailer \(if one was bound\).
* **Count** — the number of fillings.
* **Counter** — the indications of the counter sensor.
* **Mileage** — the mileage sensor value at the moment of filling. If the mileage parameter was not saved throughout the reported period, the mileage is counted from 0.
* **Notes** — an empty column for your custom comments.

![](https://docs.wialon.com/en/hosting/_media/tables/fillings.png)

The [intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) by geofences/units, drivers, trailers, filling volume, and sensor masks can be additionally applied to this table. Note that in the case of sensor masks, intervals filtration is only applied to the fuel filling detected by sensors.

You can use special [markers](https://docs.wialon.com/en/hosting/user/reports/templ/settings/map#markers) for this report to mark places of fillings on the map.

Information on **fuel thefts** can be found [here](https://docs.wialon.com/en/hosting/user/reports/tables/thefts).  


![](https://docs.wialon.com/en/hosting/_media/tables/markers-fillings.png)

