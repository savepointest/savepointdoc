# General

In the _General_ section, the format of the date and time, the measurement system, and also, depending on the [type of the report](https://docs.wialon.com/en/hosting/user/reports/templ/templ#creating_a_report_template), a number of other options are activated, described below.

![](https://docs.wialon.com/en/hosting/_media/reports/general.png)

**Multiple drivers/trailers**

This option is useful if a table added to the report template contains such columns as _Driver_ or _Trailer_. If the box is not checked, then, regardless of the number of drivers/trailers appointed to a unit for the particular interval \(trip, parking, etc.\), only the first one is shown in the table. If the box is checked, then all the drivers/trailers appointed to a unit for the particular interval are shown in the table.  


**Mileage/fuel/counters with accuracy to two decimal places**

This option allows you to always see all the mileage, fuel and sensor values to within two decimal places. If the option is not activated, the default settings are used: mileage is less than 20 and fuel less than 50 is output to the nearest hundredth, and the values ​​above are indicated in whole numbers; any values ​​of the sensor counters — only integers.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) If you see _0.00_ in a cell, it means the initial value had thousands or even smaller fractions, which can be seen if you export report to XML, CSV or Excel.

**Exclude thefts from fuel consumption**

This option can be useful if you want to ignore thefts when calculating fuel consumption in different tables and statistics. By default, however, thefts are considered a part of fuel consumption. That is if the option is enabled, such columns as _Consumed by FLS_ and _Average consumption by FLS_ are calculated without considering fuel thefts.

**Mileage from trips only**

This option affects mileage calculation. If the checkbox is not marked, the mileage is calculated according to all messages without any filtering. If the checkbox is marked, only the part of the mileage that is considered a trip is taken into account.

**Consider track-geofence intersections**

This option allows to detect a visit to a geofence in case the trip had an intersection with the geofence by any segment of its track. This option can be applied to such reports as [_Geofences_](https://docs.wialon.com/en/hosting/user/reports/tables/geofences), and [_Rides_](https://docs.wialon.com/en/hosting/user/reports/tables/rides).

**Connection loss based on GPS data**

This option can be applied to the _Connection problems_ and _Chronology_ tables, as well as to charts when selecting the background for connection loss. If the checkbox is marked, time intervals with no messages from units or messages without coordinates are shown in the corresponding reports or in charts. If no checkbox is marked, you can see only time intervals without messages.

**Skip empty rows**

This option allows to hide the rows without any data.

**Mileage and fuel with accuracy to two decimal places**

This option allows you to always see all the mileage and fuel values with an accuracy of two decimal places. If the option is not activated, the default settings are used: mileage less than 20 and fuel less than 50 are displayed to the nearest hundredth, and the values above — as whole numbers.

**Date and time format**

This option allows you to select a convenient format for displaying the date and time. Initially, the date and time mask parameters are taken from the [_User Settings_](https://docs.wialon.com/en/hosting/user/set/general) dialog. However, they can be changed at your discretion.

**Persian calendar**

This option makes it possible to use the Persian solar calendar in the resulting report for the fields with the indicated date.

**Measurement system**

This option defines the metrics for such parameters as mileage, speed, fuel, and temperature in reports.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Note._  
Depending on the [measurement system](https://docs.wialon.com/en/hosting/cms/convers/convers) selected in the report template for which the [intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) has been applied, you should remember that the values of filtration parameters are not converted into the corresponding values ​​of another measurement system. Nonetheless, the metrics are changed to the corresponding metrics of the selected system. For example, if you have 50 kilometers mileage and 100 kilometers per hour speed, after choosing the US measurement system, you receive 50 miles mileage and 100 miles per hour speed.

