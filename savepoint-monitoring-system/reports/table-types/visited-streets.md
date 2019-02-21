# Visited Streets

This report shows what streets were visited and when. Highways, roads, and other places with available addresses are also considered as streets in this report.

The following columns can be presented in this kind of report:

* **Street** — the name of the street, road, highway, etc.
* **Initial location** — the place where the first message from this street was received. It can be the same as the previous cell or more detailed \(for example, it can additionally contain a house number\).
* **Beginning** — the time when the unit started moving along the street.
* **End** — the time when the unit left the street.
* **Duration** — the total time the unit was on the street.
* **Mileage** — the distance that was traveled by the unit while moving along the street.
* **Mileage \(adjusted\)** — the mileage subject to the coefficient set in advanced unit properties. More information about mileage in the report can be found [here](https://docs.wialon.com/en/hosting/user/reports/dat/dat#mileage).
* **Avg speed** — the average speed while moving along the street.
* **Max speed** — the maximum speed detected while moving along the street. More information about speed in reports can be found [here](https://docs.wialon.com/en/hosting/user/reports/dat/dat#mileage).
* **Streets count** — the number of performed visits \(can be helpful if there is [grouping](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/parameters#grouping) by years/months/weeks/days/shifts\).
* **Notes** — an empty column for your custom comments.

![](https://docs.wialon.com/en/hosting/_media/tables/streets.png)

When clicking on a green cell in the table, the map is moved so that to display a point where the unit entered or left the indicated street, or reached the maximum speed.

Sometimes there can be gaps in cells. This means that only one message was received on this street, and therefore it is difficult to determine the length of time it was on the street, the mileage, and the average and maximum speed.

[Intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) by duration, mileage, engine hours, speed range, trips, stops, parkings, sensors, fuel fillings, and thefts can be applied to this table. For example, you can display only the streets where a particular sensor was turned on or the streets where the sensor was turned off. To specify the sensor, you can set a mask for it. This function is convenient, for example, for snow removal equipment — it allows you to know that the car did not just pass along the street, but had the brushes on.

