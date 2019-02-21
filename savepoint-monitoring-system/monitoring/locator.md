# Locator

Locator is used to generate links and share the current location of your units. Conditionally the locator can be divided into two parts — links creation and their viewing. Links are created in the locator dialog window. To open the dialog, choose the corresponding item in the [user menu](https://docs.wialon.com/en/hosting/user/gui/top#user_menu). Viewing is performed on the map of the locator map, which becomes available when clicking on the provided link.

### Viewing on the Map <a id="viewing_on_the_map"></a>

Open a link to view the map of the locator where units are displayed along with geofences \(if they have been indicated in the link creation settings\). Gurtam Maps, OpenStreetMap, and, if available, Google Maps are used to show the location of units. To choose a map layer, point the cursor on the ![](https://docs.wialon.com/en/hosting/_media/icons/layer.png) icon below the scaling buttons \(upper left corner\). You can also enable/disable displaying of geofences on the map here.

If the life span of the link is less than 48 hours, it will be shown in the upper right corner of the window.

![](https://docs.wialon.com/en/hosting/_media/monitor/locator.png)

#### Units <a id="units"></a>

A unit is presented on the map by its icon. The unit name and movement direction arrows are shown as well \(by default\). You can also activate units traces, or so called _tails_ \(switched off by default\). Click the ![](https://docs.wialon.com/en/hosting/_media/icons/settings.png) button in the lower right corner to enable/disable the above mentioned settings.

If among the units presented on the map you need to monitor a particular one, you can use the monitoring tool. Click on the corresponding button \(![](https://docs.wialon.com/en/hosting/_media/icons/follow-off.png)/![](https://docs.wialon.com/en/hosting/_media/icons/follow-on.png)\) in the right top corner and select the necessary unit from the dropdown list. Afterwards the map will be scaled and centered on the selected unit. To disable scaling and centering, select a dash from the dropdown list. Note that you cannot monitor all the available units at once. Therefore, if you select _All units_ in the dropdown list, only search is performed, and all the available units get into the field of view.

After the unit has been found, you can view its latest data. The data is shown in the window that is opened by clicking on the unit. The amount of provided information depends on the unit state \(moving/stationary\). If it is moving \(movement arrow is an indicator\), then the following parameters are shown for it: speed, time of movement, its duration and covered distance. For a unit which is not moving such parameters as speed and covered distance are irrelevant, therefore only two parameters are shown for it: the time of the start of the stationary state and its duration. Besides, regardless of the unit state the header of the opened window contains such information as the time passed from the last message and address from the last message. Note that upon receiving new messages either position of a unit on the map or its current parameters are automatically refreshed.

If it is necessary to know where the unit \(units\) was since the launch of the locator, you can generate and view its track. The track is displayed for a period of not more than 24 hours. To do this, click on the button ![](https://docs.wialon.com/en/hosting/_media/icons/track-locator.png) in the upper right corner and select the required unit from the dropdown list. Afterwards, a track is built, and the map is scaled in order for the whole track to be displayed. If the tracks are built for several units at a time, they are shown in different colors on the map and the map itself is scaled so that they all get in the field of vision. To remove a track from the map, click on the track building button again or uncheck the boxes of the units whose tracks you want to delete. Note that in the locator the track color is selected randomly and it does not depend on any unit settings.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Note._  
The track of movements can be viewed only if a user indicates such a possibility when creating the link.

#### Sensors <a id="sensors"></a>

If sensor masks have been indicated when generating a link, in the left part of the window of the locator there will be a list of units with their names, the time of receiving the last message and the latest location, as well as the names of the sensors, their values and metrics. If for some sensor [intervals and colors are set](https://docs.wialon.com/en/hosting/cms/units/sensors/props#intervals_and_colors), the adjusted color will be used for showing its value in the list.

![](https://docs.wialon.com/en/hosting/_media/monitor/locator2.png)

#### Current Location <a id="current_location"></a>

Locator provides a possibility of defining your current location on the map. This is particularly helpful if you use a locator from a mobile device.

To determine your current location press the ![](https://docs.wialon.com/en/hosting/_media/icons/position.png) button in the lower right corner. Afterwards, the map is scaled and centered on your location. ![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Due to browser restrictions, the determination of the current location is only available during the connection via the _https_ protocol.

If a particular unit has been chosen using the monitoring tool, and then you press the defining location button, both the unit and your current location get into the field of vision. However, as it was stated before, upon arrival of new messages from the unit selected in the monitoring tool, the map continues scaling and centering on it until the monitoring is disabled \(select dash from the dropdown list\).

#### Scaling <a id="scaling"></a>

When the locator is opened, the map is automatically scaled so that all units get into the field of vision. To move around the map, drag it using the mouse.

The map can be scaled using either the corresponding buttons in the upper right corner \(+/-\) or the mouse scroll. A graduated scale located in the lower left corner helps you understand the distances on the map.

Depending on the scale used and the number of items available, some icons can overlap each other. In this case, the assembly of icons is replaced by the group icon \(the number of elements is shown for every group\):

![](https://docs.wialon.com/en/hosting/_media/icons/group.png) — for units;  
[![](https://docs.wialon.com/en/hosting/_media/icons/zone_group.png)](https://docs.wialon.com/en/hosting/_detail/icons/zone_group.png?id=user%3Amonitor%3Alocator) — for geofences.

Click on the group item to see the list of all items \(icon + name\).

### Links Creation <a id="links_creation"></a>

Links are generated and edited in the locator dialog, which is accessible through the [user menu](https://docs.wialon.com/en/hosting/user/gui/top#user_menu).

To create a new link, click the _New link for sharing units_ button and fill in the fields of the form.

![](https://docs.wialon.com/en/hosting/_media/monitor/locator1.png)

Indicate the activation time for the link in the upper left corner of the dialog. It can be _Now_ or any other moment in the _future_ \(indicate the date and time in the calendar\). Note that the activation time cannot exceed 100 days.

Furthermore, enter the lifespan of the link into the corresponding field. The value can be indicated in minutes, hours, or days \(select from the dropdown list\). Note that you can specify any value \(from 0 to 1000\) or make it unlimited \(enter 0\).

You can enter a note for your link in the upper right corner of the window. This allows to distinguish the link in the general list. Besides, the note \(if entered\) is shown in the header of the page of the locator itself.

You can also check the _Geofences_ box here to share them in the link. Moreover, you can provide the possibility of generating and viewing the track of a unit by activating the _Tracks_ checkbox. ![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) The user that provides the possibility to view the track of a unit must have the _Query reports or messages_ right.

Below, you select the units whose location you want to share. The selection is made in the list on the left. Transfer the required units to the list on the right \(use double clicks or the _Add_ button\).

For the convenience of choosing units or unit groups, the contents of the list can be changed using the filter above it. The following variants are available: _All_, _Units_, _Unit groups_, _Units outside groups_. To find the required unit quickly, you can also use the dynamic filter.

Sensors with their values and metrics can also be shown in the locator. To do this, it is necessary to enable the corresponding option and [indicate the masks](https://docs.wialon.com/en/hosting/user/gui/masks#name_mask)of the sensors to be displayed.

To generate the link, click _OK_. To dismiss the changes, press _Cancel_.

#### List of Links <a id="list_of_links"></a>

Generated links get in the corresponding list containing such information as the start and end time of its operation, how much is left before the expiration date \(if the activation time has already come\), the number of units, as well as whether geofences and tracks are shown on the map of the locator. When you hover the cursor over the number of units, its list is shown in the tooltip. If there is less than one hour left before the link's expiration, the corresponding line is highlighted in red.

On the right, there are the following buttons:  
![](https://docs.wialon.com/en/hosting/_media/icons/edit.png) — edit link parameters,  
![](https://docs.wialon.com/en/hosting/_media/icons/copy.png) — copy locator,  
![](https://docs.wialon.com/en/hosting/_media/icons/delete.png) — remove link from the list.

Click on the link to open it in a new tab. To copy the URL of a link, click on the button to the right of it.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Attention!_  


* After expiration, the link is automatically deleted.
* When the user password is changed, all locator links are automatically deleted.

### Locator Integration <a id="locator_integration"></a>

Use the following form of code to integrate the locator into your web-site:

```text
<iframe src="link_address&lang=en" width="700" height="400"></iframe>
```

Necessary actions:

* In the link list click on the icon to the right of the link and copy it.
* Paste the copied link instead of _link\_address_.

Such parameters as _width_ and _height_ stand for the corresponding properties of the integrated window. The _Lang_ parameter stands for the language used.

### Manipulations with Link <a id="manipulations_with_link"></a>

As has been described earlier, there are 3 settings for the unit displaying \(movement direction, name, 'tails'\). Changing these settings the corresponding information is added to the locator's URL:

'Tail' \(on/off\)  


```text
&tails=1/0
```

Name \(on/off\)  


```text
&labels=1/0
```

Arrow \(on/off\)  


```text
&directs=1/0
```

Therefore, to save the applied settings and use them afterwards, it is necessary to utilize not the original link \(created in the locator dialog\), but the modified one \(received when the settings of unit presentation on the map are changed\).

Moreover, there is a possibility to select a map source in advance. The information on the map source is added to the locator URL. The procedure is the same for any available map, consider the example of the OpenStreetMap:

```text
&map=OpenStreetMap
```

If it is necessary to display the tracks of all available units on the map, use the parameter

```text
&build_tracks=all
```

In this case, the map shows the tracks rendered since the creation of the link.

