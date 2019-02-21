# Speeding

This kind of report shows speed limitation violations. The speed limit depends on the method for determining the speeding selecred in the properties of the unit on the [Advanced](https://docs.wialon.com/en/hosting/cms/units/adv) tab. The following information can be presented in this kind of report:

* **Beginning** — the date and time when the speed limit was exceeded.
* **Location** — the location of the device at the moment of speeding.
* **Duration** — the time interval during which the unit was moving with an excessive speed. If the speeding was determined by one message, in the line _00:00_ is written. In order the speeding to be determined also by one message, it is necessary to indicate _0_ as the minimum speeding time in the [advanced properties](https://docs.wialon.com/en/hosting/cms/units/adv#speeding) of the unit.
* **Total time** — the time from the beginning of the first speeding to the end of the last speeding.
* **Max speed** — the maximum speed within the period of speeding.
* **Speed limit** — the maximum allowed speed on a particular road section or in the unit properties.
* **Mileage** — the distance traveled with the exceeded speed.
* **Mileage \(adjusted\)** — the mileage subject to the coefficient set in unit properties \(the _Advanced_ tab\).
* **Initial mileage** — the mileage sensor value at the moment of the beginning of speeding. If no saving of mileage parameter was made through the reported period, the mileage is counted from 0.
* **Final mileage** — mileage sensor value at the end of the speeding interval.
* **Avg speed** — the average speed within the interval.
* **Driver** — the name of the driver \(if identified\).
* **Trailer** — the name of the trailer \(if bound\).
* **Count** — the number of speed violations.
* **Notes** — an empty column for your custom comments.

![](https://docs.wialon.com/en/hosting/_media/tables/speedings.png)

[Intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) \(by speeding duration, mileage, driver, geofences/units\) can be applied to this table.

You can use special [markers](https://docs.wialon.com/en/hosting/user/reports/templ/settings/map#markers) for this report:

![](https://docs.wialon.com/en/hosting/_media/tables/markers-speedings.png)

Other means to control speed are described in [Notifications](https://docs.wialon.com/en/hosting/user/notify/trigger).

