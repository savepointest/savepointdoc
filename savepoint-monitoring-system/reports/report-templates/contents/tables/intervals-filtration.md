# Intervals Filtration

Most table reports in the Wialon system involve retrieving time intervals which meet certain criteria from the unit's history. These are reports on trips, parkings, stops, engine hours, rounds, geofences and visited streets, reports on the operation of sensors and speeding, and others. For such reports, additional filtering options are provided, which specify the conditions for displaying information in the table.

![](https://docs.wialon.com/en/hosting/_media/tables/intervals_filtration.png)

Available parameters of filtration vary depending on the type of report and allow you to limit the range of intervals that fall within it. For instance, the report does not include trips, stops or speeding intervals, if their duration is less than the minimum duration specified in the intervals filtration. It is also possible to display only visited geofences in which parking has been detected or during which the sensor was turned on. All possible filters are described below.

Filters can be used both separately and in combination with each other. Each filer is applied directly to the time interval under consideration, and the report displays the value that combines the results of all the filters used.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) All filters except the mileage filter work only with integer values.

**Additional parameters**  
The filter is available for the [_Eco driving_](https://docs.wialon.com/en/hosting/user/reports/tables/drive) table. When the _Show all trips_ option is activated, all trips, not just trips with violations, are included in the report for units with customized eco-driving parameters.

**Counter sensor value range**  
This filter can only be used for the _Counter Sensors_ and _Fuel Traffic_ tables. It allows to display in the report the intervals at which the messages with values that are within the specified limits are received.

**Custom fields masks**  
The filter is available for the [_Custom fields_](https://docs.wialon.com/en/hosting/user/reports/tables/fields) table. Here you can indicate the masks that must be applied to the names of the custom fields and their values.

**Custom sensors masks**  
In the filter you can indicate the masks of custom sensors, which must be taken into account when generating a report on [digital sensors](https://docs.wialon.com/en/hosting/user/reports/tables/digital).

**Driver**  
The filter allows to display the intervals at which the unit did not have a driver or there was a certain driver or group of drivers. If you want the report to include only the intervals at which a particular driver controlled the unit, select the _With driver_ option and specify the mask of the driver's name in the field below. In this case, all intervals with the driver are displayed, regardless of whether the driver was present at the beginning, end, middle or along the whole interval. If the _Driver group_ option is selected, only the intervals at which the vehicle was driven by any driver in the group \(the mask of the name can also be specified\) are analyzed when generating the report. In addition, you can activate the _Retrieve intervals_ option to remove only the segments with the specified driver or group.

If the _Without driver_ option is selected, the table displays only the intervals at which there are segments without drivers. These segments can also be retrieved.

**Duration**  
In the filter, you can specify the minimum and/or maximum duration of the interval.

**Engine hours**  
The minimum and/or maximum duration of engine hours. In addition, the engine hours sensor mask can be specified in the _Engine hours sensor_ filter.

**Engine hours sensor**  
In this filter, you can specify a mask for the name of the engine hours sensor. It affects the calculation of engine hours in the tables which have the corresponding columns, as well as the engine hours filter if it is turned on.

**Event filter**  
This filter is only available for the _Events_ table. If it contains an event mask, only the events that satisfy it are included in the report. When the option _Custom events only_ is activated in the filter, only [custom events](https://docs.wialon.com/en/hosting/user/monitor/reg#custom_event) fall into the report. If the option is not activated, in addition to custom events, the fields with [online notifications](https://docs.wialon.com/en/hosting/user/notify/online) are also displayed in the report.

**Fuel fillings**  
The filter allows to display intervals _with_ or _without fuel fillings_ in the report. In the first case, you can additionally specify the minimum and maximum volume of fillings, and also activate the _Sum up fillings_ option. Summing up assumes that only those intervals fall into the report, the amount of fillings on which falls within the specified limits.

**Fuel thefts**  
The filter allows you to display in the report intervals with fuel thefts or without them. In the first case, you can additionally specify the minimum and maximum amount of theft, and also activate the _Sum up thefts_ option. Summing up assumes that only those intervals where the amount of thefts falls within the specified limits get into the report.

**Geofences/Units**  
This filter is divided into two parts. In the first one, you can specify the geofences by which the intervals should be filtered. In order to consider the position of the unit in any geofence or outside of it, set the radio button to the left of its name in the list from the _None_ position to the 'Inside' or 'Outside', respectively. In addition to individual geofences, you can also specify their [groups](https://docs.wialon.com/en/hosting/user/geo/groups). It is the same as specifying each geofence which belongs to the group. ![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) The number of geofences in a group is dynamic, that is, it changes when you change the list of geofences which belong to it. These changes are taken into account when building the report.

In the second part of the filter, units are selected in the same way. Thus, it is possible to get the intervals of the unit's location inside or outside the zone of another unit. The size of the zone is defined by the _Radius_ parameter. Only those units to which you have the _Query messages or reports_ access right are displayed.

To quickly search for geofences and units in the list, the [dynamic filter](https://docs.wialon.com/en/hosting/user/gui/masks#dynamic_search) is available. To select all units in a column, hold the _Ctrl_ key.

When determining the time of intersection of a unit with geofences or zones of other units, the [_Maximum interval between messages_](https://docs.wialon.com/en/hosting/cms/units/adv#parameters_used_in_reports) option is taken into account from the _Advanced_ tab of the unit's properties.

The _Retrieve Intervals_ option is available in the filter. It allows you to remove the segments inside/outside of the specified geofences or units from the intervals.

In the filters by geofences/units in the _Sensors_ section for the [_Fuel Traffic_](https://docs.wialon.com/en/hosting/user/reports/tables/fuel_traffic) table, the _Include only units with tank fuelling box_ option is available. It allows you to display in the report results only those units that were near the unit on the specified interval and had registered fillings.

**Merge intervals condition**  
In this filter, which is available for the _Counter Sensors_ and _Fuel Traffic_ tables, you must specify a timeout. If you generate a timeout between some intervals less than the indicated one, the intervals are merged. In this case, firstly the merger is carried out, and then the filtration on the basis of remaining parameters is executed.

**Mileage**  
In the filter, you can specify the minimum and/or maximum mileage within the interval. It can use both integer and fractional values. Use a period as the separator for fractional values.

**Parkings**  
The filter allows you to display only those intervals within which there were parkings, or only those within which there were none. Select the _With parkings_ or _Without parkings_ option from the drop-down list. In the filter, you can also specify the minimum length of parking. As a result of using this option, the report on geofences, for example, displays only such visited geofences in which a parking period of at least the specified duration was detected. The _Sum up intervals_option allows you to summarize the time of parking, that is, show in the report, for example, only those geofences, the **total** number of parkings in which was not less than the specified time.

**Sensors**  
The filter allows to display intervals in the report table with the sensor turned on or off, and, additionally, specify the minimum and/or maximum duration of such intervals. In order for each interval to be shown in a separate row of the table, check the _Retrieve intervals_ option. Intervals can also be summed if the maximum and/or minimum duration of the sensor on/off state is specified. To specify a certain sensor, whose turning on/off should be taken into account, specify its mask in the _Sensors mask_ filter. If several masks are specified, only those intervals at which all these sensors were simultaneously turned on/off are selected. If the sensor masks are not specified, the report takes into account all sensors of the unit.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) The intervals filtration of the _With sensor on_ type works only for the digital sensors.

**Sensors masks**  
Here you can enter the sensor [masks](https://docs.wialon.com/en/hosting/user/gui/masks) which will be considered when generating the report. Sensors masks affect the _Sensors_ filter, _Counter_ column, and information on fuel \(if any of these options is selected in the report template\). Note that the engine hours mask is indicated individually in the corresponding field.

**Speed**  
In the filter, you can set the minimum and/or maximum speed within the interval. As a result, the report shows the intervals at which the speed that falls within the given limits is met at least once. If you want only those segments within which the speed does not leave the specified limits to get in the report, activate the _Retrieve intervals_ option in the filter.

**Stops**  
This filter allows you to display only those intervals at which there were stops or only those at which there were no stops. To do this, select either the _With stops_or _Without stops_ option from the drop-down list. If the filter is not used, the report displays all the intervals, regardless of whether there were any stops or not.

**Trailer**  
Intervals filtration by the presence or absence of trailers assigned to the unit. Works similarly to the filtration by the driver.

**Trips**  
The filter allows you to display only those intervals that intersect with trips \(it is not required for the entire trip to be a part of the interval\) or only those that do not intersect with the trips. It is convenient to use the _Trips_ filter, for example, in the report on geofences: in order to cut off excess visits to the same geofence during the unit's parking \(when the coordinates are unsteady\), select the _With trips_ filter.

**Violation**  
The filter is available in the _Eco driving_ table and allows to enter the name masks of the violations that are to be taken into account while generating a report.

