# Rounds \(for unit\)

If any [routes](https://docs.wialon.com/en/hosting/user/routes/routes) were assigned to a unit and events about routes were stored in the unit history, a report based on these events can be generated:

* **Route** — the name of the route given during its creation.
* **Schedule** — the name of the schedule on the basis of which the route was created.
* **Round** — the name of the round.
* **Beginning** — the start time of the round \(activation time or entrance in the first checkpoint\).
* **Initial location** — the unit location at the beginning of the route.
* **End** — the end time of the round \(entrance to the last point\).
* **Final location** — the unit location at the end of the route.
* **Result** — _Finished_ \(the route was activated successfully, and later on the entrance to the last point was detected\), _Not finished_ \(the last point was not visited\) or _Aborted_ \(the round has been removed from the table manually or its expiration time has been reached\).
* **Skipped points** — the number of skipped checkpoints \(a detailed report can be generated — [Check Points](https://docs.wialon.com/en/hosting/user/reports/tables/points)\).
* **Duration** — the time taken to perform the route.
* **Total time** — the time from the beginning of the first route to the end of the last route.
* **Mileage** — the distance traveled while performing the route.
* **Avg speed** — the average speed on the route.
* **Max speed** — the maximum speed on the route.
* **Count** — the number of routes.
* **Driver** — the name of the driver \(if available\).
* **Trailer** — the name of the trailer \(if bound\).
* **Notes** — an empty column for your custom comments.

![](https://docs.wialon.com/en/hosting/_media/tables/rounds.png)

More information on how different route statuses are defined \(route beginning, route end, point skipped, point visit, etc.\) can be found [here](https://docs.wialon.com/en/hosting/user/routes/control#route_statuses).

In addition, in [report template](https://docs.wialon.com/en/hosting/user/reports/templ/templ), you can indicate **masks for geofences and routes**. That is, not all routes completed by the unit for the specified period can be displayed in the report, but only those that correspond to the specified route name mask or use a certain geofence\(-s\). Both filters can be used separately or simultaneously.

[Intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) can be applied to this table: by duration, mileage, engine hours, speed range, trips, stops, parkings, sensors, driver, trailer, fuel thefts, fillings, and geofences/units.

