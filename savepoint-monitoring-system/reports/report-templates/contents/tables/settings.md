# Settings

The following settings are available in this section:

* [detalization](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/settings#detalization),
* [row numbering](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/settings#row_numbering),
* [total](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/settings#total),
* [time limitation](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/settings#time_limitation),

as well as

* [incomplete interval](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/settings#incomplete_interval),
* [duration format](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/settings#duration_format).

These settings are universal for all the table types. However, individual parameters can be applied to some of them, which is described for each table separately.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Some tables have fields obligatory for submission. For instance, events should be marked in the _Chronology_ table. The _Settings_ tab of such tables and the required fields or blocks in it are marked with a red _asterisk_.

![](https://docs.wialon.com/en/hosting/_media/tables/params.png)

### Detalization <a id="detalization"></a>

Reports with [grouping](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/parameters#grouping) can be extended using the detalization option. Detalization gives an opportunity to move to a final level of nesting \(date and time\). To view the final level of nesting, you can open \(‘+’ at the beginning of the line\) all the previous levels one-by-one, or click on the corresponding level of nesting.

We can add detalization in the report \(check the corresponding box in the table parameters\), suggested [previously](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/settings?&#example) as an example of grouping and sorting use. Since in this example we already have grouping by years, months and dates, the detalization will allow us to expand the level of nesting right before the time of the event \(hours, minutes, seconds\).

![](https://docs.wialon.com/en/hosting/_media/tables/params3.png)

It should be noted that sorting is applied to the nested level. Since the detalization is the final level of nesting, you can also set the [sorting](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/parameters#sorting) for detalization in the list of groupings in a similar way.

The detalization function is applied only to the grouped tables, not the detailed ones. The exception is the reports on groups of units, drivers, trailers, and passengers, as the grouping by units is provided in them by default.

### Row Numbering <a id="row_numbering"></a>

Numbering is an additional \(always the first\) column and can be added to the table of any type.

![](https://docs.wialon.com/en/hosting/_media/tables/params4.png)

If grouping is used in the table, numbering becomes multilevel. The main level is the numbering of the main lines with the help of integers. The nested level is the numbering of hidden lines according to the _number of the main line — point — number of the nested line_ scheme.

![](https://docs.wialon.com/en/hosting/_media/tables/params5.png)

### Total <a id="total"></a>

This option adds the last line which contains the resulting data: the total duration of some state, the total number of registered events, etc.

![](https://docs.wialon.com/en/hosting/_media/tables/params6.png)

In online reports, the final line is always at the bottom of the window, regardless of the number of pages in the table and the position of the scrollbar.

_Total_ does not display the location information, as well as some other data that cannot be summarized.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) For the _Duration_ column of the [_Eco driving_](https://docs.wialon.com/en/hosting/user/reports/tables/drive) table, the duration of the **trips** at the specified time interval and not the duration of violations is indicated in the _Total_ line.

### Time Limitation <a id="time_limitation"></a>

This function allows to indicate which time intervals, days of the week, days, months must be included in the report. For instance, if you check only the working days of the week and working hours or only odd days of the month, etc., only they will be included in the report.

There are two time-limiting algorithms, which depend on the _Cut off intervals_ options:

If the option is not activated, then the state \(for example, the trip\) that started within the specified interval, but ended beyond its limits, _does not terminate_. As a result, its duration is fully included in the report.

If the option is activated, then the state \(for example, the trip\) that started inside the interval, but ended beyond its limits, _terminates_. As a result, the report includes only its duration within the specified interval, and the rest is ‘cut off’.

**Example**

The interval from 9:00 to 18:00 is selected as the time limitation interval. Two trips were registered: the first - from 7:50 to 12:00, the second - from 13:00 to 18:20.

* According to the first algorithm \(the _Cut off intervals_ option is not activated\), only the trip that started within the time limitation interval will be included in the report as a whole. That is, in the report, we get one trip lasting from 13:00 to 18:20.
* According to the second algorithm \(the option the _Cut off intervals_ option is activated\), the report will include two trips that are on the specified interval - from 9:00 to 12:00 and from 13:00 to 18:00.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) To apply a limitation equal to the whole day, you need to set the interval from 00:01 to 23:59.

### Incomplete interval <a id="incomplete_interval"></a>

The _Incomplete interval_ option does not apply to all intervals of the table, but only the last \(trips, sensor operation, etc.\), since its ending does not always coincide with the end of the reporting period. To display this interval, the following options are provided:

* **Show and cut off**  the interval is displayed in the report and in the ending column has the time of the last message for the reporting period;  
* **Do not show in report**  the incomplete interval is not displayed in the report;  
* **Show and mark as incomplete**  the interval is displayed in the report and has the label _Unknown_ in the ending column.

### Duration Format <a id="duration_format"></a>

In tables where the duration is encountered, you can select the format for displaying it. The following options are available:

* **days hours:minutes:seconds**  when displayed in the report, it is displayed as follows: _5 days 12:34:56_.
* **hours:minutes:seconds**  in the report, the duration is displayed as follows: _132:34:56_, that is, the hours are not combined in days \(if there are more than 24\). The option affects not only the cells but also the _Total_ row.
* **hours \(with two decimal places\)**  the duration in the report is displayed as _3.45_ instead of _3:27_.

