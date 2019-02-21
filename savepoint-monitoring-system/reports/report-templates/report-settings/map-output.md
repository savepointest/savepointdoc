# Map Output

The lines of the online report, which contain information about the location of the unit at the time of an event, are highlighted in blue. If you click on the line with the left mouse button, the message is marked on the map with a special marker, and the map, in turn, is centered on its location. A similar option works for some _Regular_ [charts](https://docs.wialon.com/en/hosting/user/reports/templ/contents/charts/charts) \(where the X scale represents time\): when using the trace tool, you move to the message on the map.

Some elements can be drawn on the map as a part of the report. They can be selected in the _Map output_ section of the report template dialog. These can be [tracks](https://docs.wialon.com/en/hosting/user/tracks/tracks) traveled by unit, [geofences](https://docs.wialon.com/en/hosting/user/geo/geo), as well as special [markers](https://docs.wialon.com/en/hosting/user/reports/templ/settings/map?&#markers_in_reports) in the form of small icons which can be put in the places of events, fillings, thefts, speedings, etc. All this is configured when creating or editing a report template on the [_Settings_](https://docs.wialon.com/en/hosting/user/reports/templ/settings/settings) tab in the _Map output_ section.

![](https://docs.wialon.com/en/hosting/_media/reports/map.png)

All graphical elements are shown for the current report. If generating a new report, all tracks and markers from the previous report are erased and replaced by new. When switching to other panels, all graphical elements from the current online report, as well as a map position and zoom remain on the map. To remove them, return to the _Reports_ panel and click the _Clear_ button. Alternatively, the graphics of any panel can be hidden or displayed again. To do this, check the corresponding boxes in the horizontal menu. More information about using map with different panels can be found [here](https://docs.wialon.com/en/hosting/user/gui/map#using_the_map_with_different_panels).

### Graphical Elements Filtration <a id="graphical_elements_filtration"></a>

Intervals filtration is supported for some graphical elements \(e.g. markers of speedings, events, fillings, thefts, parkings, and stops, as well as trip routes\) adjusted upon working with a report template. To set intervals filtration means to indicate parameters considered for displaying graphical elements on the map. The values of filtration parameters are indicated for each element individually. A set of available filtration parameters for such an element corresponds to a set used for the [intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) in a similar-type table.

To open the filtration parameters dialog, it is necessary to click the corresponding icon \(![](https://docs.wialon.com/en/hosting/_media/icons/filtration.png)\) to the right of a graphical element. Note that to set the filtration parameters, it is required to check the box of a corresponding graphical element first.

![](https://docs.wialon.com/en/hosting/_media/tables/markers_filtration.png)

If intervals filtration has been already set for a table of the corresponding type, and such a filtration needs to be set for displaying graphical elements on the map as well, you can facilitate a process of indicating the filtration parameters by uploading those applied to the table. To do so, select a corresponding table in the drop-down list \(the first line of the dialog\) and click _Upload_.

To reset the indicated filtration parameters, click _Clear_. To leave the dialog without applying changes, press _Cancel_. To apply selected settings, click _OK_.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Attention!_  
The filtration set for displaying graphical elements on the map also affects the corresponding markers and backgrounds chosen for [charts](https://docs.wialon.com/en/hosting/user/reports/templ/contents/charts/properties#filter).

### Tracks in Reports <a id="tracks_in_reports"></a>

The routes traveled by a unit in a selected period of time can be shown on the map. To do this, select one of the options: _Trip routes_ or _All messages on map_in the report template dialog. In accordance with the first option, only the intervals considered as trips \(according to the [Trip Detector](https://docs.wialon.com/en/hosting/cms/units/trip)\) are displayed as tracks with different colors. In this case, it is required to activate the _By trips_ option in the advanced user settings. In the case of the _all messages on map_ option, all the messages with valid coordinates are converted into a track regardless of trips, parkings, stops, etc. If in the unit history there are intervals where the connection was lost \(there were no messages for a long time\) or coordinates were not determined in messages, such intervals are displayed with a dashed line.

By default, the routes are drawn with blue color. However, you can choose another color or even have multi-colored tracks according to the speed or sensor state. The set of colors to be used in tracks is defined in [Unit Advanced Properties](https://docs.wialon.com/en/hosting/cms/units/adv)\).

Besides, to get the information about track points, hover the mouse cursor over and see the information in a tooltip \(time, speed, coordinates, altitude, sensor values\). Note that messages are searched in the radius of 50 pixels to the cursor.

![](https://docs.wialon.com/en/hosting/_media/tracks/point.png)

If tracks or all messages are on, then such tables as _Trips_, _Rides_, _Engine hours_, _Speedings_ are supplied with an additional first column containing the icon of the binoculars. When clicking on the icon, the map is centered at a certain segment of the track, and this segment is highlighted by a bold red line on the map.

![](https://docs.wialon.com/en/hosting/_media/reports/binoculars.png)

Tracks can be rendered for units groups, too \(see the [Advanced Reports](https://docs.wialon.com/en/hosting/user/reports/adv/adv) section\). It is reasonable to assign different colors for units in a group to differentiate them on the map. However, note that the number of simultaneously drawn messages can be limited by your service provider.

![](https://docs.wialon.com/en/hosting/_media/reports/group_tracks.png)

### Geofences in Reports <a id="geofences_in_reports"></a>

Created [geofences](https://docs.wialon.com/en/hosting/user/geo/geo) can be a part of a report. They are displayed on the map if you check the _Render geofences_ box in the _Map_ section of the report template.

![](https://docs.wialon.com/en/hosting/_media/reports/geopoi.png)

Geofences are displayed with their captions and images or icons \(if you have selected any\). The color and the font size of the caption is taken from their properties. Apart from that, additional options can be applied to geofences:

* _Group icons_. The geofences that overlap each other can be replaced by one conditional item, and its tooltip contains the detailed information. The same can be applied to [markers](https://docs.wialon.com/en/hosting/user/reports/templ/settings/map?&#markers).
* _Consider geofence visibility scale_. By default, all the geofences are rendered on the map. However, they can be seen or hidden according to their visibility parameter set in the [properties](https://docs.wialon.com/en/hosting/user/geo/new?&#set_geofence_properties).

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Note._  
Geofences are taken only from the same account as the report template itself.

### Markers in Reports <a id="markers_in_reports"></a>

Most types of reports can have additional information visualized on the map with the help of special markers. To get these markers in a report, select the required markers in a report template.

The table below presents all possible markers and their icons.

| ![](https://docs.wialon.com/en/hosting/_media/icons/parking.png) | Parking marker | Marks a location where, according to the [trip detector](https://docs.wialon.com/en/hosting/cms/units/trip), a parking takes place. A tooltip shows the beginning of a parking time and parking duration. |
| :--- | :--- | :--- |
| ![](https://docs.wialon.com/en/hosting/_media/icons/stop.png) | Stop marker | Marks a location where, according to the [trip detector](https://docs.wialon.com/en/hosting/cms/units/trip), a stop takes place. A tooltip shows the beginning of a stop time and stop duration. |
| ![](https://docs.wialon.com/en/hosting/_media/icons/filling.png) | Filling marker | Marks a location where, according to sensors data, a fuel filling takes place. A tooltip shows filling time and the amount of fuel filled. |
| ![](https://docs.wialon.com/en/hosting/_media/icons/theft.png) | Theft marker | Marks a location where, according to the sensors data, a fuel theft takes place. A tooltip shows theft time and the amount of fuel stolen. |
| ![](https://docs.wialon.com/en/hosting/_media/icons/event.png) | Event marker | Marks the locations where events were automatically registered by means of [notifications](https://docs.wialon.com/en/hosting/user/notify/action). The events [registered manually](https://docs.wialon.com/en/hosting/user/monitor/reg), including fuel fillings, are also shown by such markers if a location \(and preferably a description\) is indicated during event registration. A tooltip shows the event time and the text of the event. |
| ![](https://docs.wialon.com/en/hosting/_media/icons/violation.png) | Violation marker | If you select event markers, then both event and violation markers are to be displayed because a violation is a special case of an event. |
| ![](https://docs.wialon.com/en/hosting/_media/icons/speeding.png) | Speeding marker | Marks a location where speed limits indicated in the [unit properties](https://docs.wialon.com/en/hosting/cms/units/adv#speeding) were violated. A tooltip shows the initial time of the speeding interval \(i.e. the time of receiving the first message with a speed value exceeding the allowed one\), the allowed speed \(indicated in the unit properties\), the value of speeding and the total duration of a speeding interval. |
| ![](https://docs.wialon.com/en/hosting/_media/icons/pics.png) | Image marker | Marks a location where [pictures](https://docs.wialon.com/en/hosting/user/monitor/pics) from a unit were received. |
| ![](https://docs.wialon.com/en/hosting/_media/icons/vid.png) | Video marker | Marks a location where [videos](https://docs.wialon.com/en/hosting/user/monitor/pics) from a unit were received. |

The panoramic images of the territory can be displayed when clicking on the markers of parkings and stops. For this, maps with panoramas \(for instance, Yandex Panorama or Google Street View\) should be selected in [user settings](https://docs.wialon.com/en/hosting/user/set/maps). If there are pictures of the territory with the coordinates of the marker, when pointed at it, the cursor changes from _arrow_ to _hand_. Click on the marker to open a panorama snapshot in the window of the [_Address_](https://docs.wialon.com/en/hosting/user/tools/address) tool. Double-click on another such marker to update the information.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Note._  
When enabling event markers, in addition to event markers you get violation markers because a violation is a special case of an event.

Markers appear on the map after a report is generated. If you see no markers, it means there are no events of the indicated type or the current map scale is not enough \(try to zoom in\).

When you hover the mouse cursor over a marker, you see additional information in a tooltip: for stops and parkings — starting time and duration, for events and violations — time and notification text, for fillings and thefts — time and fuel volume, for speedings — starting time, speed limitation as it is defined in unit properties, how much the speed is exceeded, and duration of this speeding.

![](https://docs.wialon.com/en/hosting/_media/reports/markers.png)

Moreover, markers, as well as geofences can be grouped in case they overlap each other — indicate the _Group icons_ option in the report template for it. In case of markers grouping, a number of elements included in a group is indicated. More detailed information about what happened in that place is available in the tooltip. However, if there are more than 100 grouped markers, only their names appear in the tooltip, without detailed information.

![](https://docs.wialon.com/en/hosting/_media/reports/markers2.png)

You can enable the _Marker numbering_ option in a report template. In this case, each marker has its sequence number which is indicated below the marker in red color. Numbers are assigned chronologically, and each marker type has its own enumeration.

![](https://docs.wialon.com/en/hosting/_media/reports/markers3.png)

### Unit Last Location <a id="unit_last_location"></a>

The last location of the unit can be displayed on the map. To enable this feature, select the _Unit last location_ checkbox in map output settings of the report template. The last location does not depend on the reported interval, it is taken from the latest message received from the unit. Units are displayed on the map by their icons or by motion state signs \(depending on [User settings](https://docs.wialon.com/en/hosting/user/set/general#unit_visualization_on_map)\) as well as by their names considering the [Unit label color](https://docs.wialon.com/en/hosting/cms/units/adv#unit_label_color) option. In the pop-up tooltip you can find the time when the message was received, the speed at that point, altitude, and the values of mileage and engine hours counters.

![](https://docs.wialon.com/en/hosting/_media/reports/last-popup.png)

