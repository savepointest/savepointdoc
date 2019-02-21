# Unit Presentation on Map

By default, a unit on the map is displayed by an [icon assigned to it](https://docs.wialon.com/en/hosting/cms/units/image) which is selected when the unit is configured, and a caption with its name. Icons for units can be selected from a standard set, e. g. ![](https://docs.wialon.com/en/hosting/_media/icons/standard.png), or you can upload your own image in the [Image](https://docs.wialon.com/en/hosting/cms/units/image) tab. In addition, the icon can rotate depending on the course \(direction\) of the unit. This feature is also defined in the unit properties.

![](https://docs.wialon.com/en/hosting/_media/monitor/rotation.png)

![](https://docs.wialon.com/en/hosting/_media/icons/group.png)Icons that overlap each other on the map can be replaced by the common icon with a number indicator. To do this, select [_Display overlapping units in one icon_](https://docs.wialon.com/en/hosting/user/set/general#unit_visualization_on_map) in the _User Settings_ dialog.

### Alternatives for Icons <a id="alternatives_for_icons"></a>

Unit icons can be replaced with the motion state signs. This option is called _Replace unit icons with motion state signs_ and is set in the [User Settings](https://docs.wialon.com/en/hosting/user/set/general#unit_visualization_on_map). The following symbols are possible:

* green arrow — the unit is moving, the direction of the arrow indicates the direction of movement;
* red square — the unit is not moving \(if there is an ignition [sensor](https://docs.wialon.com/en/hosting/cms/units/sensors/sensors), it also means that the unit is standing with the engine off\);
* yellow circle — the unit is standing with the engine on \(only for units with ignition sensors\).

![](https://docs.wialon.com/en/hosting/_media/monitor/signs.png)

Besides, the colors of these icons \(arrow, square, circle\) can be different and depend on the value of the sensor. This functionality is adjusted in the [_Advanced_](https://docs.wialon.com/en/hosting/cms/units/adv#usage_of_sensor_colors)tab of the unit properties. In other words, the shape of the icon is defined by the state \(standing still — square, moving — arrow\), and the color depends on the sensor value \(intervals and colors are adjusted in the [sensor properties](https://docs.wialon.com/en/hosting/cms/units/sensors/props#intervals_and_colors)\).

Unit names can be shown or hidden when displaying a unit on the map. It depends on the state of the \(![](https://docs.wialon.com/en/hosting/_media/icons/name.png)\) button in the [layers menu](https://docs.wialon.com/en/hosting/user/gui/map#visible_layers) on the map.

### Displaying Inactive Units <a id="displaying_inactive_units"></a>

Monitoring units are conventionally divided into active and inactive ones. Inactive units are units that have not received messages with coordinates for more than 48 hours. Other units are considered active.

The system supports the possibility of differentiating unit states on the map. To do this, check the _Blur icons of inactive units_ box in the [user settings](https://docs.wialon.com/en/hosting/user/set/general#unit_visualization_on_map). In this case, inactive units are displayed on the map with blurred icons and transparent names. If the signs of motion are used instead of icons, then the signs and names are displayed as transparent. If the _Display overlapping units in one icon_ box is checked in the _User Settings_, and all the units with overlapping icons are inactive, the icon for them is displayed blurred. Moreover, the icons of drivers or trailers bound to the inactive unit are also blurred until they are unbound.

![](https://docs.wialon.com/en/hosting/_media/monitor/inactive.png)

### Displaying Units with LBS Detector <a id="displaying_units_with_lbs_detector"></a>

The _LBS detection_ is an alternative method of finding units on the map. The accuracy of this method is inferior to determining the location using GPS, but if the unit experiences troubles with the GPS connection you can switch to the _LBS detection_ method. To do this, it is necessary to check the [_Allow positioning by cellular base stations_](https://docs.wialon.com/en/hosting/cms/units/adv#messages_validity_filtration) box on the _Advanced_ tab of the unit properties dialog. Therefore, if the _LBS detected_ data is more recent than the GPS data, it is used to determine the current location of the unit.

When using the _LBS detection_, units are displayed on the map in the following way: the current icon of the unit is placed into a transparent white circle with a red dotted stroke, the brightness of the icon decreases.

![](https://docs.wialon.com/en/hosting/_media/monitor/lbs_units.png)

### Other Markings <a id="other_markings"></a>

![](https://docs.wialon.com/en/hosting/_media/monitor/tail.png)

If the unit is currently in motion, the green arrow shows the direction of its movement, and the unit can be followed by a blue _tail_ \(trace\) which shows the track for the last few messages. If the unit is stationary \(according to the last message\), this arrow is not shown. If there was no motion within several latest messages, it means that the trace is not shown or the page has just been loaded. The length of the trace is 5 messages, however, it can be changed together with the trace width and color in the [User Settings](https://docs.wialon.com/en/hosting/user/set/general#unit_visualization_on_map).

Direction arrows, traces, the names of assigned drivers and units can be disabled. To do this, use the corresponding buttons in the [layers menu](https://docs.wialon.com/en/hosting/user/gui/left#visible_layers) on the map:

![](https://docs.wialon.com/en/hosting/_media/icons/tail.png) — hide/show the traces of the unit;  
![](https://docs.wialon.com/en/hosting/_media/icons/name.png) — hide/show the name of the unit;  
![](https://docs.wialon.com/en/hosting/_media/icons/driver_name.png) — hide/show the name of the assigned driver \(if there are any\);  
![](https://docs.wialon.com/en/hosting/_media/icons/course.png) — hide/show the direction of movement of the unit.  


If the names of both units and assigned drivers are enabled simultaneously, the latter are shown in parenthesis. The colors of the captions are taken from the [unit properties](https://docs.wialon.com/en/hosting/cms/units/adv#unit_label_color).

The ![](https://docs.wialon.com/en/hosting/_media/icons/private_mode.png) icon to the left of the caption signals that the [_Do not show unit location_](https://docs.wialon.com/en/hosting/cms/units/sensors/props) option is activated for the unit and the private mode of the trip is detected.  


