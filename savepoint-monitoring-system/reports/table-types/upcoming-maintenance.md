# Upcoming Maintenance

The upcoming maintenance table contains the list of service works set for a unit and the status of their execution. A table may include the following columns:

* **Service interval** — the name of the scheduled maintenance work indicated on the _Service Intervals_ tab of the unit properties dialog in the _Service name_ field. The work should be repeated throughout a particular interval indicated in the _Service Intervals_ tab.
* **State** — the overall state of the execution of the service work. In other words, it is the remaining or expired interval of mileage, engine hours, and days.
* **State by mileage** — the remaining or expired mileage interval.
* **State by engine hours** — the interval of the remaining or expired engine hours.
* **State by days** — the interval of the remaining or expired days.
* **Description** — the information taken from the corresponding field on the _Service Intervals_ tab.
* **Frequency** — the interval \(mileage, engine hours, or days\) that shows how often a vehicle maintenance should be performed.
* **Notes** — an empty column for your custom comments.

![](https://docs.wialon.com/en/hosting/_media/tables/req_maint.png)

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Note that there is no need to indicate the time interval for the _Upcoming maintenance_ report generation because this table provides you with the information on all the indicated service works regardless of the time period.

Moreover, an individual parameters of [grouping](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/parameters#grouping) \(without any connection to the time intervals\) are used in the _Upcoming maintenance_ table. The data can be grouped on the basis of the state \(planned/expired maintenance\), service interval, or unit \(for reports on unit groups\).

