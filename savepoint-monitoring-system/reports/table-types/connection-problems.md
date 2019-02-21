# Connection Problems

This kind of report lists the time periods when the system did not receive data from the unit. The parameters for this report are adjusted in [Unit Properties =&gt; Advanced](https://docs.wialon.com/en/hosting/cms/units/adv#parameters_used_in_reports) where you set _Maximum interval between messages_.

The following information can be presented in this kind of report:

* **Beginning** — the date and time when connection loss happened.
* **End** — the date and time when the connection was recovered. ![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Note that if the time passed between receiving the last message for the reporting interval and the end of a report interval exceeds a value of a maximum interval between messages, then a connection loss interval will be added to the report. The beginning of this interval corresponds to the time of receiving the last message, and the end corresponds to the end of a reporting interval.
* **Duration** — the time interval of connection loss.
* **Location** — the address where the unit was right before the loss of connection.
* **Count** — the number of connection gaps detected in a certain time interval \(it is advisable when grouping rows by days/weeks/months or for reports about groups of units\).
* **Driver** — the name of the driver \(if available\).
* **Trailer** — the name of the trailer \(if it was bound\).
* **Notes** — an empty column for your custom comments.

![](https://docs.wialon.com/en/hosting/_media/tables/connection.png)

Additional [filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) by driver, trailer and geofences/units can be applied to this report.

