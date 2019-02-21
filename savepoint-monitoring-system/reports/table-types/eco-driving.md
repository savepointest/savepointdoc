# Eco Driving

The report provides you with the information on how a driver handles the entrusted vehicle. Analysis of the driving behavior can help you extend the life of the vehicle, reduce fuel costs, ensure cargo safety and also understand the reason of any case of emergency.

Before generating the _Eco Driving_ report it is necessary to indicate settings on the [corresponding tab](https://docs.wialon.com/en/hosting/cms/units/eco) of the unit properties dialog. Eco driving analysis is based on the data received during the trip.

A table may contain the following information:

* **Violation** — the type of violation. When you use grouping, violations with the same name will be merged into one group.
* **Beginning** — the time when violation began.
* **Initial location** — an address of the unit location at the moment of violation beginning.
* **End** — the end time of the violation.
* **Final location** — the address where the unit was located at the moment of the end of the violation interval.
* **Value** — the parameter value during the violation.
* **Avg speed** — the average speed during the violation.
* **Max speed** — the maximum speed during the violation.
* **Penalty** — the penalty value indicated on the [_Eco Driving_](https://docs.wialon.com/en/hosting/cms/units/eco) tab of the unit properties.
* **Rank** — the penalty points converted to a 6-point rating system \(can be useful if grouping by years, months, weeks, days, shifts, or trips has been applied\).
* **Rating by violations** — an individual index number of a unit/driver calculated on the basis of the committed violations. The lower the rating, the fewer violations are committed. ![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) This column can be used in the report on unit groups and driver groups only.
* **Mileage** — mileage for the interval of violation or [grouping](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/parameters#grouping).
* **Mileage \(adjusted\)** — mileage taking into account the coefficient set in unit properties \(the _Advanced_ tab\).
* **Initial mileage** — the mileage counter value at the moment of the beginning of the violation. If the mileage parameter was not saved at the reporting interval, the mileage is counted from zero.
* **Final mileage** — the mileage counter value at the end of the violation interval.
* **Duration** — the duration of the violation or grouping interval. If the speeding is detected by one message, in the line «00:00» is written.
* **Count** — the number of violations of this type.
* **Driver** — the name of the driver on this vehicle.

Special attention should be paid to the _Rating by violations_ column. It can be used in the report on unit groups and driver groups only. If the column is included in the table, then units/drivers can be placed in the table according to the violations committed \(from the lower rating to the highest one\). To do this, select the total grouping by rating in the parameters of the report template. The violations rating is calculated by the system on the basis of the eco driving ranks. In case the ranks are similar, the system takes the covered mileage into account. The higher the mileage value with the same rating, the lower the rating by violations is. Note that the system supports the visual marking of the rating fields according to the eco driving rank. To do this, select the colors and the values matching them in the corresponding block of the report template parameters.

![](https://docs.wialon.com/en/hosting/_media/tables/eco-dr.png)

Note that it is easier to analyze the received report if the grouping option was applied to the report template. The information received in the report can be grouped on the basis of different criteria, such as time \(year, month, week, day, shift\), type of violation and trips.

Moreover, in addition to grouping an option of [detalization](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/settings#detalization) can be applied. This option allows to view the final level of nesting \(date and time\) inside of grouping. However, take into consideration that a penalty and rank can be given for a violation that occurred at a certain time interval \(not immediately\). That is why on the final level of nesting \(date and time\) a dash is given in the _Rank_ column, and the _Penalty_ column receives the value indicated on the _Eco Driving_ tab of the unit properties.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) If grouping is used in the _Eco driving_ table or the [_Total_](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/settings#total) line is added to it, the _Duration_ column indicates the duration of the **trips** at the specified time interval and not the duration of the violations.

### Penalty Scoring System <a id="penalty_scoring_system"></a>

The value of penalty points for a particular criterion is indicated on the [_Eco driving_](https://docs.wialon.com/en/hosting/cms/units/eco) tab of the unit properties dialog. Afterwards the indicated points are used in the report for driving quality evaluation. The calculation of penalty points is made using the special algorithm. The main peculiarities are presented below.

**Without grouping**

* If no averaging has been used, the penalty value \(earlier indicated on the _Eco Driving_ tab\) is displayed next to every criterion in the corresponding column. The _Total_ line \(if available\) contains the value which corresponds to the sum of points scored for violations.
* If averaging \(by mileage/by time\) has been used, the main difference is that the _Total_ value corresponds to the value received as a result of dividing the total number of scored penalty points by the number of minute intervals \(averaging by time\), or by the number of kilometer intervals \(averaging by mileage\) in a trip.

**With grouping**

* If no averaging has been used, the total number of penalty points for the violations of a particular group is displayed next to every group in the corresponding column. The _Total_ line \(if available\) contains a sum of penalty scores received for all the violations.
* If averaging \(by mileage/by time\) has been used, this averaging is applied to every group of parameters in the report table. Besides, if the _Total_line is available, the averaging will be applied to the total number of the scored penalty points. The algorithm of averaging is described above. You can also get acquainted with it on the _Eco Driving_ tab of the unit properties dialog.

### Penalty–Rank Conversion <a id="penalty_rank_conversion"></a>

The system allows to recalculate the received penalties into a six-point evaluation system.

The following algorithm is used:

| Penalty | Rank |
| :--- | :--- |
| 0 | 6.0 |
| Less than 20 | 5.9 |
| 20-50 | 5.0 |
| 50-100 | 4.0 |
| 100-200 | 3.0 |
| 200-500 | 2.0 |
| More than 500 | 1.0 |

![](https://docs.wialon.com/en/hosting/lib/exe/indexer.php?id=user%3Areports%3Atables%3Adrive&1550652801)

