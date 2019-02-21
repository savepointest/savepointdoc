# Chart Properties

There are two tabs in the chart properties: [_Data_](https://docs.wialon.com/en/hosting/user/reports/templ/contents/charts/properties#vybor_dannyx) и [_Settings_](https://docs.wialon.com/en/hosting/user/reports/templ/contents/charts/properties#nastrojki_grafikov).

### Data Selection <a id="data_selection"></a>

On the _Data_ tab, you can select the curves that should be displayed in the chart. The selection is only available for charts of the [_Regular_](https://docs.wialon.com/en/hosting/user/reports/templ/contents/charts/types#regular_charts) type.

![](https://docs.wialon.com/en/hosting/_media/charts/curves_selection.png)

Mark the curves you want to see in the report. Two points can be checked simultaneously. In this case, two curves are displayed, for instance, speed and engine revs. There can be more curves, but only if there are no more than two variables in the chart, besides time.

To change the name of the point, click on it with the left mouse button and edit the text. To return the original name, click the _Default_ button ![](https://docs.wialon.com/en/hosting/_media/icons/rename.png) \(the button is inactive if the name has not been changed\).

In addition, it is possible to change the order of the items. To do this, drag the double arrow icon ![](https://docs.wialon.com/en/hosting/_media/icons/drag.png), located to the left of the required curve, up or down.

### Chart Settings <a id="chart_settings"></a>

In addition to selecting columns, the settings are available on the same-name tab.

![](https://docs.wialon.com/en/hosting/_media/charts/settings.png)

The tab is divided into two sections:

* [Parameters](https://docs.wialon.com/en/hosting/user/reports/templ/contents/charts/properties#parameters);
* [Filter](https://docs.wialon.com/en/hosting/user/reports/templ/contents/charts/properties#filter).

#### Parameters <a id="parameters"></a>

In the _Parameters_ section it is possible to activate the _Split sensors_ and _Count from zero_.

**Split sensors**

If a unit has several sensors of the same type and you need to create a chart for this type, then by default the curves of such sensors are displayed in the same chart. Check the _Split sensors_ option to create an individual chart for each sensor. For example, for a unit with two voltage sensors, external and internal, a chart with two curves \(the option is not checked\) can be built, as well as two charts with one curve \(if the option is checked\).

![](https://docs.wialon.com/en/hosting/_media/reports/chart01.png)

![](https://docs.wialon.com/en/hosting/_media/reports/chart02.png)

![](https://docs.wialon.com/en/hosting/_media/reports/chart03.png)

If for the data points selected for a chart there are several sensors, the upper one is split. Let us assume that a unit has two voltage sensors and two temperature sensors, and you are building a voltage/temperature chart for it. If the _Split sensors_ option is off, you will get one chart with four curves in it. If the _Split sensors_ option is on, you will get two charts with three curves on each: one chart will contain the first voltage sensor and both temperature sensors, and another one will contain the second voltage sensor and both temperature sensors.

**Count from Zero**

The _Count from Zero_ option is responsible for scaling the chart. By default, the range of the Y scale depends on the range of values falling within the specified interval. That is, if, for example, the temperature fluctuates from 3 to 5 degrees, then the reading on the Y scale starts at 3, and the curve, in this case, occupies the maximum space on the chart. If the _Count from zero_ option is activated, the Y-axis on the graph is always built from zero to the largest value \(if the values ​are negative, then from the lowest value to zero\).

The image below shows an example of two voltage charts for the same unit within the same time interval. The first chart is regular, the second — with the _Count from Zero_ option turned on.

![](https://docs.wialon.com/en/hosting/_media/reports/chart04.png)

![](https://docs.wialon.com/en/hosting/_media/reports/chart05.png)

#### Filter <a id="filter"></a>

The following settings are available in the _Filter_ section:

* Sensor masks;
* Markers;
* Background;
* Line color.

**Sensor masks**

This option allows you to specify the sensors on the basis of which the chart should be built. The option does not influence the _Speed_, _Altitude_, _Fuel consumption by math_ charts, as they can be built regardless of whether a unit has sensors or not.

Specify the [mask](https://docs.wialon.com/en/hosting/user/gui/masks#name_mask) of the required sensor. To do it, enter its full name or part of the name. You can use special characters: '\*' \(replaces any number of characters\) or '?' \(replaces one character\). The name of the sensor cannot contain commas.

If the masks are not specified, the sensors of the required for building the chart type are determined automatically.

**Markers**

This option allows to specify the event markers, which should be displayed in the chart. Here, the same [markers](https://docs.wialon.com/en/hosting/user/reports/templ/settings/map#markers) are used as for the events on the map.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) The setting of [graphical elements filtration](https://docs.wialon.com/en/hosting/user/reports/templ/settings/map#graphical_elements_filtration) influence the display of markers and backgrounds.

**Background** The intervals of such events as stops, parkings, trips, connection losses, and work of engine hours can be used as a chart background. Using these backgrounds you can correlate a chart value and an interval to which it corresponds. Different colors can be assigned for the event intervals. To select a color, click on the color box, choose the color from the palette and click _OK_.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) The background of the event intervals is opaque and has a display priority, that is, the interval above is overlapped by the lower ones. To change the priority, drag the desired interval of events up or down using the double arrow icon ![](https://docs.wialon.com/en/hosting/_media/icons/drag.png) to the left of the name of the desired interval.

**Line color**

This section allows to use the [sensor's color scheme](https://docs.wialon.com/en/hosting/cms/units/sensors/props#intervals_and_colors) to display the line of a corresponding chart. To apply the sensor's color scheme, indicate its mask in the field opposite the curve name \(the fields correspond to the items selected in the [_Data_](https://docs.wialon.com/en/hosting/user/reports/templ/contents/charts/properties#data_selection) tab\). If no mask is indicated, the default colors are used.

![](https://docs.wialon.com/en/hosting/_media/charts/line_colour.png)

