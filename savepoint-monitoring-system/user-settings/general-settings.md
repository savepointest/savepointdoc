# General Settings

The first tab of the [User Settings dialog](https://docs.wialon.com/en/hosting/user/set/set) contains general settings. Here you indicate your time zone, input your e-mail address, change the password to enter the system, and set many other parameters.

![](https://docs.wialon.com/en/hosting/_media/set/set1.png)

### Basic <a id="basic"></a>

**Language**  
The language menu. Contact your service administrator to expand the list of available languages.

**Time zone**  
The choice of time zone influences the time parameters that are displayed in all dialogs and panels.

**Daylight saving time**  
Specify DST options if you use summer and winter time in your region — choose the most appropriate DST schedule on the dropdown list. _None_ — summer time is not used.

**Persian calendar**  
This option allows to activate the Iranian calendar also known as Persian solar calendar. It is used in Iran and Afghanistan. If the option is chosen, the Persian calendar replaces the usual \(Gregorian\) calendar in the places where a user should indicate some time interval \(to build a track, to query messages or a report, to set up a job or assign a route, etc.\) Note that the Persian calendar can be used to indicate particular dates of an interval only \(from – to\). Working with _quick intervals_ \(_Today_, _Yesterday_, _Week_, _Month_, _Year_\), the Gregorian calendar is applied. If the interface is in Arabic, the calendar is in Farsi \(the language spoken in Iran\) and is shown from right to left. Otherwise, it is in English \(in Latin characters and Arabic numbers\) and is shown from left to right \(see [details](https://docs.wialon.com/en/hosting/user/gui/calendar#the_persian_calendar)\). Enabling/disabling the Persian calendar requires reloading the page.

**Date and time format**  
Select the format of the date and time that is convenient for you. Depending on the entered mask, the data elements can be arranged in different order and have a different appearance. A month, for example, can be displayed with a word or a number, a year with two or four digits, and so on. In addition, the day can also be included. The syntax instructions for each field are given in a tooltip. In the drop-down list, you can select one of the predefined masks. The table below shows some examples of formats:

| Date mask | Time mask | Result 1 | Result 2 |
| :--- | :--- | :--- | :--- |
| yyyy-MM-dd | HH:mm:ss | 2014-01-25 09:45:33 | 1987-12-02 17:20:00 |
| d/MM/yy | HH:mm | 25/01/14 09:45 | 2/12/87 17:20 |
| d MMMM yyyy dddd | hh:mm:ss tt | 25 January 2014 Saturday 09:45:33 am | 2 December 1987 Wednesday 05:20:00 pm |
| dd MMM yyyy ddd | hh:mm tt | 25 Jan 2014 Sat 09:45 am | 02 Dec 1987 Wed 05:20 pm |

**First day of week**  
Select either Monday or Sunday as the first day of the week. This affects the appearance of the [calendar](https://docs.wialon.com/en/hosting/user/gui/calendar) and the manner of counting weeks in general.

**Measurement system**  
Select one of the available [measurement systems](https://docs.wialon.com/en/hosting/cms/convers/convers). The corresponding units of measurement are used in such [tools](https://docs.wialon.com/en/hosting/user/tools/tools) as Distance, Area, Routing, Nearest Units. The measurement system also influences address processing, as well as the creation of [routes](https://docs.wialon.com/en/hosting/user/routes/routes). However, the earlier created units and resources \(together with geofences, jobs, and notifications\) possess the measurement system selected upon their creation. As for reports, their measurement system is set separately \(refer to [_Advanced settings of a report template_](https://docs.wialon.com/en/hosting/user/reports/templ/settings/general)\).

**City**  
In this field, you can indicate your city. It is used in the [Nearest Units](https://docs.wialon.com/en/hosting/user/tools/nearest) and [Address](https://docs.wialon.com/en/hosting/user/tools/address) tools as the default city. Enter the name of the city. When you enter the first letters, the dropdown menu with the names corresponding to the request opens automatically. You can either continue typing in the name or choose it from the drop-down menu \(there can be several cities with the same names in different countries\).

In addition, this setting determines the position of the map when entering the monitoring system. However, if there are monitored units on the map, the map is scaled so that all of them are in sight.

**Distance from unit to geofence**  
This option activates the calculation of the distance from a unit to a geofence when using the latter as the address. The maximum allowable value is 100 km or miles \(depending on the selected system of measures\).

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) To work with this option, activate the [_Geofences_](https://docs.wialon.com/en/hosting/cms/accounts/services) service in the account properties.

**Play sound for events**  
A sound can be played when an [online notification](https://docs.wialon.com/en/hosting/user/notify/notify#online_notification) is triggered or a [driver's message](https://docs.wialon.com/en/hosting/user/monitor/cmd#chat_with_driver) is received. In Windows OS, [QuickTime Alternative](http://www.free-codecs.com/download/QuickTime_Alternative_Lite.htm) can be used as a media player. If you use Opera, you may need additional adjusting, so that the request to play or save the sound does not appear.

**Automatically display popup events**  
If this option is activated, the [online notifications](https://docs.wialon.com/en/hosting/user/notify/notify#online_notification) and the [messages from drivers](https://docs.wialon.com/en/hosting/user/monitor/cmd#chat_with_driver) are automatically shown on the display. If it is deactivated, only a number in the red circle in the bottom panel of the program near the corresponding icon indicates that new events have been received.

**Use keyboard shortcuts**  
Check this box to activate the [Shortcuts](https://docs.wialon.com/en/hosting/user/gui/keys).

**Infinite map**  
Allows the circular \(_infinite_\) movement of the map to the right or left. This option should be activated _only_ when tracking is carried out around the 180th longitude \(Fiji, Chukotka, etc.\).

**Driver's activity**  
Check this boxto show the information on driver's activity in the unit and driver [tooltips](https://docs.wialon.com/en/hosting/user/monitor/extra#unit_s_tooltip), as well as in the [extended unit information](https://docs.wialon.com/en/hosting/user/monitor/extra#extended_unit_information).

**Render charts on server**  
Check this box to use the static charts in the monitoring system.

### Show Additional Information about the Unit <a id="show_additional_information_about_the_unit"></a>

In this section of the settings, you can choose what additional information about the unit should be displayed in the tooltip or in the worklist.

In the **left column**, check the boxes with the elements that should be shown in the [unit tooltip](https://docs.wialon.com/en/hosting/user/monitor/monitor#unit_s_tooltip) \(displayed as you hover the mouse pointer over the unit's icon\). In the **right column**, check the boxes with the elements that should be shown in the [extended unit information](https://docs.wialon.com/en/hosting/user/monitor/monitor#extended_unit_information) in the work list.

To select or remove the selection of all the items from any column, hold the _Ctrl_ key on the keyboard and check any box of the corresponding column. You can change the order of those elements of the tooltip to the left of which there is the icon ![](https://docs.wialon.com/en/hosting/_media/icons/drag.png). To do this, drag the double arrow icon up or down.

The unit tooltip can include the following information:

**Last message**  
The time when the most recent message was received and how long ago.

**Icon**  
Unit's icon of a larger size. If the icon has not been selected from the [library](https://docs.wialon.com/en/hosting/cms/units/image) and has been uploaded by the user, it is displayed in its original size, but not larger than 128\*128 pixels.

**Location**  
The most recent detected address of the unit.

**Presence in geofences**  
If a unit in the latest message was within a certain [geofence](https://docs.wialon.com/en/hosting/user/geo/geo), the name of the geofence is displayed in the unit tooltip in the color that is assigned to it in the geofence properties. This option also affects units count in the _Geofences_ panel.

**Speed**  
The speed indicated in the latest positional message.

**Altitude**  
The altitude indicated in the latest positional message \(if the device is able to give such data\).

**Counters**  
The values of mileage counter and engine hours counter. To learn more, see [Counters](https://docs.wialon.com/en/hosting/cms/units/counters).

**Satellites**  
The number of satellites locked in the latest positional message.

**Coordinates**  
GPS coordinates of the unit, taken from the latest positional message received \(in decimal degrees\).

**Sensor values**  
[Sensors](https://docs.wialon.com/en/hosting/cms/units/sensors/sensors) configured for the unit and their known values. The custom sensor name is displayed and the value processed according to the calculation table of this sensor.

**Connectivity settings**  
Device type, unique ID\(s\), and phone number\(s\) specified in the [unit properties](https://docs.wialon.com/en/hosting/cms/units/general). This information is available to users with the _Edit connectivity settings_ access right.

**Parameters**  
The latest known [parameters](https://docs.wialon.com/en/hosting/user/msg/msg#data_messages). Their names and values match those in the messages without conversion to other units.

**Drivers**  
The name, photo, and phone number of the [driver\(s\)](https://docs.wialon.com/en/hosting/user/drivers/drivers) currently bound to the unit.

**Trailers**  
The name and photo \(if available\) of the [trailer\(s\)](https://docs.wialon.com/en/hosting/user/trailers/trailers) currently bound to the unit.

**Custom fields**  
[Custom fields](https://docs.wialon.com/en/hosting/cms/units/fields) from the properties of the unit \(general or/and admin fields depending on access rights\).

**Profile**  
[Profile information](https://docs.wialon.com/en/hosting/cms/units/charact) of the unit.

**Maintenance state**  
Specified [service intervals](https://docs.wialon.com/en/hosting/cms/units/maint) and terms for their implementation \(days/engine hours/kilometers left or expired\).

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _The unit tooltip_ contains information about the unit and its latest message. _The message tooltip_ \(as well as the tooltips of _charts_ and _tracks_\) only contains information about the message itself, i. e. does not include connectivity settings, icon, custom fields, profile, maintenance state, drivers, trailers.

**Multicolor sensors in unit tooltip**  
Depending on the option selected in the drop-down list, the name and value of the sensor or only its value can be displayed in accordance with the color scheme adjusted on the first tab of the [sensor's properties](https://docs.wialon.com/en/hosting/cms/units/sensors/props#intervals_and_colors). If this option is disabled, the information about sensors is displayed in black.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Note._  
The mileage and engine hours counters are refreshed once a minute, as well as the information about drivers and trailers. Checking for presence in geofences is performed every two minutes. Other information is refreshed instantly.

### Unit Visualization on Map <a id="unit_visualization_on_map"></a>

**Replace unit icons with motion state signs**  
When the box is checked, all [icons](https://docs.wialon.com/en/hosting/cms/units/image) of the units are replaced by conventional signs showing their activity. The green arrow indicates that the unit is moving, and its direction shows — which way. The yellow circle means that the unit is standing with the engine running, the red square — that the unit is standing with the engine off. See [_Unit presentation on map_](https://docs.wialon.com/en/hosting/user/monitor/display#unit_presentation_on_map).

**Display overlapping units in one icon**  
![](https://docs.wialon.com/en/hosting/_media/icons/group.png)If two or more units are _overlapping_, their icons are grouped into the common one. It facilitates the visual perception of the map. The common icon is selected in the library \(the _Library_ button appears on the right when the setting is activated\) and has a value indicator showing a number of units in it. To see the list of units the common icon contains, hover your mouse cursor over the icon for a pop-up window to appear. Upon clicking the common icon the map is scaled in such a way that all the units of the common icon get into the visual field. Note that overlaying icons cannot be grouped into the common one on the 2 largest scales. When you view the map on such a scale, accuracy is important, so all the icons are visible, regardless of their overlapping.

**Show unit icons at map borders**  
If a unit is outside the visible area, its icon is displayed at the map border in the direction where the unit is located. Click on this icon to see this unit on the map.

**Blur icons of inactive units**  
Check this box in order to differentiate [unit states](https://docs.wialon.com/en/hosting/user/monitor/display#displaying_inactive_units) on the map.

**Trace**  
It is possible to indicate the length of the trace which is added to a moving unit on the map \(the _Points in traces_ parameter\) and select the color and width for it.

### Other Items on Map <a id="other_items_on_map"></a>

**Display names of routes' checkpoints on map**  
Depending on the checkbox, [route](https://docs.wialon.com/en/hosting/user/routes/routes) checkpoints can be displayed with or without their names on the map.

**Display names of geofences on map**  
Depending on this checkbox, [geofences](https://docs.wialon.com/en/hosting/user/geo/geo) can be displayed on the map with their names or without them. The color of the captions is adjusted in [geofence properties](https://docs.wialon.com/en/hosting/user/geo/new?&#set_geofence_properties).

**Display overlapping geofences in one icon**  
![](https://docs.wialon.com/en/hosting/_media/icons/zone_group.png)If several icons of geofences overlap when displayed on the map, they can be grouped into one. Place the cursor over this icon to know what geofences are hidden behind it. Note that for reports this option is set independently — in the [advanced options](https://docs.wialon.com/en/hosting/user/reports/templ/templ#options) of a report template.

**Render geofences on server**  
By default, all [geofences](https://docs.wialon.com/en/hosting/user/geo/geo) are rendered in the browser. Rendering on the server is advisable if not a very powerful computer is used for monitoring but the speed of internet connection is quite high. In such cases, the performance of the Wialon system increases significantly. When displaying a big number of geofences \(more than 500\), the option of rendering geofences on the server is activated automatically. ![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) If more than 1000 geofences are displayed, they are grouped in one icon in case of overlapping.![](https://docs.wialon.com/en/hosting/lib/exe/indexer.php?id=user%3Aset%3Ageneral&1550214120)

|  |
| :--- |


