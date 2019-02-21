# Parameters

In the _Parameters_ section, you can configure the [grouping](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/parameters#gruppirovka) and [sorting](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/parameters#sorting) of the report data.

### Grouping <a id="grouping"></a>

Grouping is the arrangement of information based on the indicated characteristics.

When adding a new grouping, click _Add grouping_, select a time interval in the appeared drop-down list and click _Add_.

![](https://docs.wialon.com/en/hosting/_media/reports/add_grouping.png)

From the available time intervals \(year, season, month, week, day of the month, day, date, shift, duration\), select those based on which you want to group the tabular data. Grouping can be either single- or multi-level. Multi-level grouping implies that there are several groupings for different time intervals. When using it, it is required to assign a hierarchy \(specify nesting\). For example, the grouping can be as follows: tabular data is grouped by year, within each year by months, and within months by days. Nesting is adjusted by dragging the intervals in the _Grouping_ column up or down, with the element above in the list containing the ones that are located below.

If grouping by such intervals as season and duration is selected, at the bottom you can find a special block where it is necessary to set values for the intervals.

* **For seasons** Enter the name of the season, for example, summer, autumn, etc. Afterwards, use the drop-down lists to specify its duration. Note that the duration of the season is a period from the beginning of the first specified month to the end of the last. The minimum duration of the season is one month. Thus, if the _Wintry_ season lasts during February, in both drop-down lists you must select _February_. To activate the season, click the _Add_ button. The maximum number of seasons is 12.
* **For duration** For each interval of duration, you must enter a name \(for example, interval 1\), then specify the duration in seconds, minutes, hours or days \(select from the drop-down list\), and also activate it by clicking the _Add_ button. The maximum number of duration intervals is 5. Using the _Trips_report as an example, let us look at how the use of duration intervals influences the presentation of the report data. The following periods are indicated: _Short trips_ — up to 15 minutes, _Medium-term trips_ — up to 1 hour, _Long trips_ — up to 3 hours. Information in the report will be presented in the following way: short trips — from the minimum trip time indicated in the [trip detector](https://docs.wialon.com/en/hosting/cms/units/trip) up to 15 minutes, medium-term trips — from 15 minutes up to 1 hour, long trips — from 1 up to 3 hours.

Depending on the report type, besides standard groupings \(by time intervals\), additional groupings can be used as well \(for example, by geofence, route, sensor, user, event, action type, violation type, trips, streets\). In this case, the grouping works **by the name** of the element.

### Sorting <a id="sorting"></a>

Sorting is the distribution of information in a table in descending or ascending order based on the selected characteristics.

Sorting allows to distribute the grouped data by any selected column of the report table.

Next to each added grouping interval, in the _Sorting_ column there is a drop-down list where you can specify the column included in the report so that the data will be sorted by the specified characteristic \(column\) within the grouping. The selected sorting criterion is applied to the subsequent \(nested\) grouping level. In addition, to the left of the drop-down list, there is an icon with the help of which you can set the direction of sorting \(from smaller to greater and vice versa\).

Tabular data can be sorted even if the grouping is absent. To do this, in the drop-down list in front of the _Total_ interval select the sorting parameter and also set the direction of grouping.

**Example**

Let us consider the example of grouping and sorting use.

We create a report on trips. In this report, we are interested in the maximum speed, duration, and mileage. Mark these columns. In addition, the information should be grouped by years, months and dates; the dates, in turn, should be sorted by the maximum speed \(from high to low\).

By default, there is no grouping, i.e. without adding grouping or sorting settings, we would get a detailed report where an individual line would correspond to each criterion. These lines would be arranged in chronological order or according to the sorting, indicated next to the _Total_ grouping.

![](https://docs.wialon.com/en/hosting/_media/tables/params1.png)

In order to get the result that corresponds to our task, we need to add the _Year_, _Month_ and _Date_ groupings. If necessary, we can move the grouping criteria to the desired position in the list \(we need the Year –&gt; Month –&gt; Date sequence\).

Next, we determine the sorting criteria and the direction. Since we want to set sorting for the level nested in months \(for dates\), we select the corresponding criterion from the drop-down list of months. Then click the icon of sorting direction to adjust it from a bigger to a smaller value.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) By default, the data is sorted in chronological order.

The report looks as follows:

![](https://docs.wialon.com/en/hosting/_media/tables/params2.png)

Compared to the table for which the grouping and sorting settings are not specified, this table has two additional columns. The first one is a column containing the ‘+’ and ‘-’ buttons, which help show/hide nesting levels. The second is the _Grouping_ column, which shows the levels themselves. The information in the table is grouped by years, and by clicking on the _plus_ the next levels of grouping \(months, dates\) are opened. The dates are sorted by the maximum speed \(from high to low\).

### Time intervals and their use in reports <a id="time_intervals_and_their_use_in_reports"></a>

* **Total** — the highest level of grouping \(cannot be moved\). If it is checked, the report contains a grouping with the resulting data \(the total duration of any state, the total number of registered events, etc.\) in which all the subsequent groupings are nested \(if there are any\).
* **Year** — the grouping of the information in the table by years.
* **Month** — the grouping of the information in the table by months.
* **Week** — the grouping of the information in the table by weeks. The number of the week is displayed \(e.g. week 26, etc.\).
* **Day** — the grouping of the information in the table by days of the week \(e.g. Monday, Tuesday, etc.\).
* **Day of the month** — the grouping of the information in the table by days of the month \(e.g. the 1st, 2nd, etc. day of the month\).
* **Date** — the grouping of the information in the table by dates.
* **Shift** — the grouping of the information in the table by [shifts](https://docs.wialon.com/en/hosting/user/reports/templ/settings/shifts).

When grouping data, the events that **began** in the interval are included in it. To determine the duration of an event, its entire duration is taken into account, even if it has already ended in another interval. That is why in the _Duration_ column there may be values exceeding the size of the interval itself.

When grouping the table data, it makes sense to use the _**Total time**_ column, which, unlike the _Duration_ column, shows not the sum of the intervals \(e.g. the total time of all trips\), but the time from the beginning of the first interval to the end of the last one. This allows, for instance, to calculate the total time of the working day \(convenient for travel sheets\).

#### Retrieve intervals <a id="retrieve_intervals"></a>

This option applies only to the reports with the grouping by [shifts](https://docs.wialon.com/en/hosting/user/reports/templ/settings/shifts). If it is not activated, the whole interval of the trip which intersected with the shift gets in the report. If it is activated, then only the data from the messages received within the specified interval is included in the report.![](https://docs.wialon.com/en/hosting/lib/exe/indexer.php?id=user%3Areports%3Atempl%3Acontents%3Atables%3Aparameters&1550651589)

|  |
| :--- |


