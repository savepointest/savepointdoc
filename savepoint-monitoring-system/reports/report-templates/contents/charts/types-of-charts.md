# Types of Charts

As with the tables, there are several **types** of charts:

* [Regular](https://docs.wialon.com/en/hosting/user/reports/templ/contents/charts/types#grafiki_tipa_obychnyj);
* [Processed fuel level](https://docs.wialon.com/en/hosting/user/reports/templ/contents/charts/types#obrabotannyj_uroven_topliva);
* [Speed/Fuel consumption](https://docs.wialon.com/en/hosting/user/reports/templ/contents/charts/types#skorostrasxod_topliva).

### Regular Charts <a id="regular_charts"></a>

The charts of this type differ in that the X axis always lays time, and the data for the Y axis is selected on the _Data_ tab from the list:

* Speed \(km/h or mph\);
* Altitude \(meters or feet\);
* Engine operation \(on/off\);
* Engine efficiency sensor;
* Voltage \(volts\);
* Temperature \(degrees Celsius\);
* Engine revs \(rpm\);
* Cargo weight;
* Counter sensor;
* Custom sensors;
* Custom digital sensors \(on/off\);
* Absolute mileage;
* Mileage in trips;
* Instant mileage;
* Fuel level \(liters or gallons\);
* Processed fuel level \(liters or gallons\);
* Fuel consumption by ImpFCS;
* Fuel consumption by AbsFCS;
* Fuel consumption by InsFCS;
* Fuel consumption by FLS;
* Fuel consumption by math;
* Fuel consumption by rates.

![](https://docs.wialon.com/en/hosting/_media/user/reports/templ/contents/charts/curves_selection.png)

You can simultaneously select two points. In this case, the chart will contain two curves, for example, speed and engine revs. You can select even more points but note that only two variables can exist in one chart in addition to time. It means if Y-axis represents speed scale on the left and temperature scale on the right, nothing can be added to this graph. But if Y-axis represents speed scale on the left and consumption by ImpFCS on the right, it is still possible to add consumption by AbsFLS and other methods, since they are all measured in the same metrics.

The picture below shows the speed chart combined with the fuel level chart. To receive such a chart, it is required to set the chart type as _Regular_ and select the _Speed_ and _Fuel level_ data.

![](https://docs.wialon.com/en/hosting/_media/reports/chart-management.png)

Each curve on a chart is assigned its own color. On the left, in the _Report Result_ block, you can specify which color corresponds which curve. Their names are taken from the report template. In addition to the name for the curves, the units of measurement are also indicated.

The names of the lines of the chart can be changed in its properties in the report template. However, if the curve is built based on some sensor, then it is given the name of the sensor.

Click on the curve name in the _Report Result_ section to enable/disable its display on the chart.

**Smoothing**

Almost all charts of the _Regular_ type are provided in two forms: raw and smoothed \(_**smoothed**_ is indicated in parentheses after the name\). Smoothing affects the style of the chart display. The chart without smoothing is built straight from a message to message, and, as a result, has an angular outline. If you choose smoothing, the chart has a smoother outline. The level and algorithm of smoothing for all charts is the same.

Below is an example of a chart in which a raw speed chart is displayed with an orange line, and a blue one shows a smoothed chart.

![](https://docs.wialon.com/en/hosting/_media/reports/chart06.png)

**Fuel Level Charts**

_Fuel level_ chart represents 'raw' data, whilst in the _Processed fuel level_ chart the filtration is applied.

**Mileage Charts**

Four kinds of mileage charts can be created: absolute mileage, mileage in trips, instant mileage, and instant mileage smoothed. The first two show how mileage changed \(increased\) over time. Absolute mileage chart is built on the basis of all messages, which means that any inaccuracy and outlying data affect the resulting chart. Mileage in trips chart displays the data taking [trip detector](https://docs.wialon.com/en/hosting/cms/units/trip) settings into account. Below you see the chart with curves for absolute mileage \(blue\) and mileage in trips \(orange\).

![](https://docs.wialon.com/en/hosting/_media/reports/chart-mileage.png)

The _Instant mileage_ chart represents the data in the _mileage from the previous message to the current one_ form, that is the difference in the distance between two adjacent messages. This kind of chart can be useful to detect excessive mileage during connection loss, or to detect made-up additions to the mileage in cases where it is determined by special sensors \(see the settings of the mileage counter in the [unit properties](https://docs.wialon.com/en/hosting/cms/units/counters). Instant mileage can be smoothed.

### Special Charts <a id="special_charts"></a>

Along with the regular charts, the following charts are available:

* Processed fuel level
* Speed/Fuel Consumption by…

![](https://docs.wialon.com/en/hosting/_media/charts/other_charts.png)

Settings for these charts are fixed and cannot be changed. Editing is available only for the name of the chart. Also, it is possible to select the required sensors \(indicate [the mask of the sensor](https://docs.wialon.com/en/hosting/user/reports/templ/contents/charts/properties#filtr)\) or [split sensors](https://docs.wialon.com/en/hosting/user/reports/templ/contents/charts/properties#parametry).

#### Processed Fuel Level <a id="processed_fuel_level"></a>

The _Processed fuel level_ chart shows the values which are used while calculating fuel level, fillings and thefts in tables.

The chart shows the dependence of fuel level on mileage \(mileage/liters\). It can also show the dependence of the fuel level on time \(time/liters\) if the [_Time-based fuel level sensors consumption_](https://docs.wialon.com/en/hosting/cms/units/fuel#fuel_consumption) option is turned on in the unit settings.  
In both cases the chart is processed taking the filtration into account, which is set on the _Fuel Consumption_ tab \(the _Filter fuel level sensors values_ option\) or in the [sensor properties](https://docs.wialon.com/en/hosting/cms/units/sensors/props#additional_properties).

Below are two fuel level charts: the first one is processed \(time-based FLS and filtration are on, the filtration level is 25\), and the second one is not processed.

![](https://docs.wialon.com/en/hosting/_media/reports/chart08.png)

![](https://docs.wialon.com/en/hosting/_media/reports/chart07.png)

A special _Processed fuel level_ chart should be distinguished from two similar regular charts:

1. Regular _Fuel level_ chart represents the _raw_ data \(no filtration is applied\). The _Time-based fuel level sensors consumption_ checkbox does not affect the chart.
2. Regular _Processed fuel level_ chart represents dependence of filtered and smoothed on the basis of mileage data from time.

These regular charts can represent data only in the _Time/Fuel level_ form. At the same time, it is possible to overlay other charts, such as, for instance, the voltage chart.

#### Speed/Fuel Consumption Chart <a id="speedfuel_consumption_chart"></a>

This chart shows the dependence of average fuel consumption on speed. The data for it is taken from fuel consumption sensors of different types \(such as impulse, absolute, instant\) or fuel level sensor, or predefined consumption by math or rates. The corresponding calculation methods must be specified in the properties of the unit in the [_Fuel Consumption_](https://docs.wialon.com/en/hosting/cms/units/fuel) tab.

![](https://docs.wialon.com/en/hosting/_media/reports/chart09.png)

