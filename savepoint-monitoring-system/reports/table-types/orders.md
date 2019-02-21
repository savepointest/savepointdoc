# Orders

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Attention!_  
To generate a report, activate the _Orders_ [service](https://docs.wialon.com/en/hosting/cms/accounts/services) first.

This kind of report displays detailed information about orders that were used while creating the route in the [Logistics](http://apps.wialon.com/?lang=en#logistics) app. The table can contain the following columns:

* **Name** — the name of the order.
* **Time from** — the time from which the order should be delivered \(the beginning of the delivery interval\).
* **Time to** — the time until which the order should be delivered \(the end of the delivery interval\).
* **Estimated arrival time** — the approximate time of arriving at the destination point \(system calculation\).
* **Actual arrival time** — the actual time of arriving at the destination point.
* **Deviation** — the difference between the actual and estimated arrival time.
* **Estimated mileage** — the approximate distance to the destination point \(system calculation\).
* **Actual mileage** — the actual distance to the destination point.
* **Estimated time to point** — the approximate time for covering the distance between the previous and current destination points \(system calculation\).
* **Actual time to point** — the actual time spent on covering the distance between the previous and current destination points.
* **Fuel consumed** — the amount of fuel spent on delivery.
* **Avg temperature** — the average temperature over the delivery period.
* **Min temperature** — the minimum temperature value registered for the interval of delivery.
* **Max temperature** — the maximum temperature value registered for the interval of delivery.
* **Initial temperature** — the temperature value at the beginning of delivery.
* **Final temperature** — the temperature value at the end of delivery.
* **Status** — the status of the order delivery \(confirmed/rejected/not set\).
* **Comment** — a comment entered when the status was submitted.
* **Address** — the address of the delivery point.
* **Weight** — total weight of goods in the order.
* **Volume** — the quantitative value \(for example, items\) of the order indicated at its creation.
* **Cost** — the total cost of goods in the order.
* **Client name** — the name of the client.
* **Driver** — the name of the driver.
* **Files** — the number of files attached to the order.

![](https://docs.wialon.com/en/hosting/_media/tables/orders.png)

Additional parameters can be selected for this kind of report. In other words, the report on orders can be generated on the basis of orders of the selected type:

* **All orders** — all orders for the indicated time period.
* **Visited** — the arrival of a courier to the address is fixed, or the status is set.
* **Visited late** — orders are visited and fixed with a delay, or the status is set with a delay.
* **Fulfilled** —the arrival of a courier to the address is detected and fixed, the _Confirm_ status is set.
* **Rejected** — the orders for which the _Reject_ status is set.
* **Visited without status** — the arrival of a courier to the address is detected, the status is not set.
* **Non-visited** — the arrival of courier to the address is not detected.

