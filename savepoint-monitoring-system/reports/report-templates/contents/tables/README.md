# Tables

 add a table to the report template, click the _New Table_ button on the [_Contents_](https://docs.wialon.com/en/hosting/user/reports/templ/contents/contents) tab of its properties.

In the _New table_ dialog, specify the name and type.

![](https://docs.wialon.com/en/hosting/_media/reports/report_tables.png)

### Columns Selection <a id="columns_selection"></a>

The set of available table types differs depending on the selected type of the report template. The list of tables and their description are presented in the chapters [below](https://docs.wialon.com/en/hosting/user/reports/tables/tables).

Each type of the table has its own set of columns which can be included in it. The list of available ones is shown on the _Columns_ tab after selecting the type of table. To quickly find the required one, you can use [dynamic filter](https://docs.wialon.com/en/hosting/user/gui/masks#dynamic_search). Select the ones you want to see in the report. To select all the columns, press the _Ctrl_ button and click on any unselected column. Removing a selection from all the columns works in the same way. Identical principle is used in the settings of the reports, where geofences, events, etc. should be selected.

![](https://docs.wialon.com/en/hosting/_media/reports/report_tables1.png)

To change the name of the column, click on it with the left button and edit the text. To return the original name of the column, press the _Default_ button ![](https://docs.wialon.com/en/hosting/_media/icons/rename.png)\(the button is inactive if the name has not been changed\).

What is more, the order of the columns can be changed as well. To do this, drag the icon of the double arrow ![](https://docs.wialon.com/en/hosting/_media/icons/drag.png), located to the left of the name of the desired column, up or down.

Some alternative types of reports are available as apps:

* [iDriveSafe](http://apps.wialon.com/?lang=ru/#idrivesafe) — evaluation of the quality of driving;
* [Driving Logbook](http://apps.wialon.com/?lang=ru/#drivinglogbook) — a tax report that defines the actual use of the company car for personal or business purposes \(based on the trips report\);
* [Dashboard](http://apps.wialon.com/?lang=ru/#dashboard) — presentation of key indicators of fleet efficiency in a graphical form.

Any number of tables can be added to the template, and the same table can be added to the report several times with different column configurations, data grouping settings, etc.

### Calculator <a id="calculator"></a>

The calculator is available in all the tables \(except for _Images_, _Video_ and _Statistics_\). It allows to add custom columns to them. To the left of the column names, indices in the C0, C1, C2 … CN format are indicated. Indices **do not change** regardless of the position of the column in the list.![](https://docs.wialon.com/en/hosting/_media/reports/reports_calculator.png)

To add an arbitrary column to the table, press the _Add calculator_ button and enter the calculation formula in the _Formula_ field that appears. To do this, you can use:

* indices of the columns of the table — you can enter them manually or click on the required ones in the list of available columns;
* parameters of the unit: _rcoef_ — consumption by rates, _dehr_ — standard hourly rate, _mcoef_ - mileage coefficient;
* constants \(for example, _const2/5_\);
* mathematical operations +, -, \*, / and \(\) to indicate their priority.

Thus, the formula can, for example, be as follows _\(C1 + C2 + C7\)\*const1.5/rcoef_.

Specify the unit of measurement in the next field \(up to 10 characters\) and click _OK_. The custom column automatically goes to the top of the list, however, if necessary, its position can be changed in the standard way. Such columns differ from the rest by the absence of an index and the background of a blue color.

![](https://docs.wialon.com/en/hosting/_media/reports/reports_calculator1.png)

To edit the name, formula, or units of measurement for the created column, click in the desired field with the left mouse button and make the required changes. Click anywhere in the dialog to confirm the changes.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) The value of an arbitrary column in the [_Total_](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/settings#total) row is calculated in the same way as for other rows, that is, using the specified formula and the column values of the _Total_ row.

### Table Settings <a id="table_settings"></a>

For each table, in addition to selecting columns, there are additional settings, located in the same-name tab.

![](https://docs.wialon.com/en/hosting/_media/reports/report_settings.png)

The tab is divided into three sections:

* [Parameters](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/parameters);
* [Settings](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/settings);
* [Intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration).

