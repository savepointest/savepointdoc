# Monitoring Options

All the options that can be found in the _Monitoring_ panel are described below. Depending on the tasks assigned, you can choose to display some columns and hide the others. To do this, the _Can change settings_ option must be activated in the [user properties](https://docs.wialon.com/en/hosting/cms/users/props).

To customize the columns in the _Monitoring_ panel, press the special button \(three vertical dots\) in the upper right corner. In the left column, mark the checkboxes that should be displayed in the worklist and in the [monitoring options menu](https://docs.wialon.com/en/hosting/user/monitor/extra#monitoring_options_menu). In the right column, you can select the options that are used more rarely — they will be shown in the additional menu and will be available there.

All the options in the _Monitoring_ panel can nominally be divided into two types:

1. _Of information._ These icons contain some information about the current state of the unit \(movement/stop, sensor value, connection state, data accuracy\). For additional information, see the tooltip which appears when you hover the mouse cursor over the icon.
2. _Of action._ A click on these options allows to perform an action on the unit \(event registration, command or report execution, messages query, track building, properties editing, removal from the work list, etc.\). As a rule, all further instructions can be found in the corresponding dialogs. Active action buttons turn blue when you mouse over them.

The icons in the upper part of the worklist can also be used. In some cases, it allows to [sort the units](https://docs.wialon.com/en/hosting/user/monitor/list#simple_list_mode) according to some properties \(e.g. at the top are the moving units, at the bottom — the stationary ones, and vice versa\).

![](https://docs.wialon.com/en/hosting/_media/monitor/icons.png)

### Secondary Information <a id="secondary_information"></a>

All the options in the _Monitoring_ panel are divided into 5 sections. The first one contains the _Secondary information_ option, which allows to display the contents of the text columns under the unit names. The following alternatives are possible:

* None;
* Address;
* Geofence;
* Driver’s name;
* Driver’s phone number;
* Trailer.

When the private mode of the trip is detected \(if the unit has the [_Private mode_](https://docs.wialon.com/en/hosting/cms/units/sensors/types#digital) type sensor with the [_Do not show unit location_](https://docs.wialon.com/en/hosting/cms/units/sensors/props) option enabled\), the information about the last known location during the previous ‘business’ trip is displayed as the current address or geofence.

### Options of information <a id="options_of_information"></a>

Next two sections include the options connected with the display of the information about the units. If one or several parameters in the first section \(text parameters\) are turned on, you can adjust the width of the corresponding columns in the _Monitoring_ panel. To do it, hover the mouse cursor over the space between the columns whose width you want to change. When the dotted line appears, drag it to the desired side.

#### Location <a id="location"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/location.png)This column displays the location of the units either in the form of addresses or in the form of [geofences](https://docs.wialon.com/en/hosting/user/geo/geo). By pressing the icon in the header, the units in the worklist can be sorted according to their location \(in the direct or reverse alphabetical order\). _Resolving_ means the address is being searched. _N/A_ appears for units whose location is not available, for example, in case a unit has never sent any messages.

* _Addresses_ Depending on the [selected format](https://docs.wialon.com/en/hosting/user/set/maps), addresses can be longer \(if they include state, region, and other elements\) or shorter \(e.g., street and building number only\).
* _Geofences_ If geofences are chosen to determine the location, once a unit gets into several of them, all the geofences are displayed and separated by commas. They are also sorted by area \(from smaller to a larger one\) and highlighted in the color selected in the geofence properties. If a unit is outside of all available geofences, the address is displayed as its location. In any case, this column is the widest in the _Monitoring_panel which is why it is not recommended to turn it on if there is not enough space on the screen. 

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Attention!_  
To determine whether a unit is inside a geofence, the option _Presence in geofences_ should be activated in the _General Settings_ tab. This option is enabled automatically if you select geofences for the location column.

When the private mode of the trip is detected \(if the unit has the [_Private mode_](https://docs.wialon.com/en/hosting/cms/units/sensors/types#cifrovye) type sensor with the [_Do not show unit location_](https://docs.wialon.com/en/hosting/cms/units/sensors/props) option enabled\), the last known location is displayed as the address or geofence instead of the current one and the ![](https://docs.wialon.com/en/hosting/_media/icons/private_mode.png) icon appears in the unit’s caption, as well as next to its name in the monitoring panel.

#### Drivers <a id="drivers"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/driver.png)The column with the information about the [drivers](https://docs.wialon.com/en/hosting/user/drivers/drivers). This column can contain the driver’s photo, photo, and name, or photo and phone number depending on the display option chosen in the _Monitoring_ panel customizer. The tooltip always contains the photo, name, and phone number of the driver.

* ![](https://docs.wialon.com/en/hosting/_media/icons/driver0.png) — no drivers bound;
* ![](https://docs.wialon.com/en/hosting/_media/icons/driver1.png) — the assigned driver has no photo;
* ![](https://docs.wialon.com/en/hosting/_media/icons/driver2.png) — several drivers are bound to the unit;
* ![](https://docs.wialon.com/en/hosting/_media/icons/driver3.png) — the assigned driver is running out of the allowed driving time \(monitored when the [_Driver activity_](https://docs.wialon.com/en/hosting/cms/units/adv#driver_activity) option is activated in the unit properties on the _Advanced_ tab\). If a photo is uploaded for the driver, an exclamation mark is displayed to the right of it instead of the icon.

#### Trailers <a id="trailers"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/trailer.png)The column with the information about the [trailers](https://docs.wialon.com/en/hosting/user/trailers/trailers). This column may contain the photo or photo and name of the trailer depending on the display option chosen in the _Monitoring_ panel customizer. The tooltip always contains the photo and name of the trailer bound to the unit.

* ![](https://docs.wialon.com/en/hosting/_media/icons/trailer0.png) — no trailers bound;
* ![](https://docs.wialon.com/en/hosting/_media/icons/trailer1.png) — the bound trailer has no photo;
* ![](https://docs.wialon.com/en/hosting/_media/icons/trailer2.png) — several trailers are bound \(see more information in the tooltip\).

#### Unit Tracking <a id="unit_tracking"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/eye_off.png)/![](https://docs.wialon.com/en/hosting/_media/icons/eye_on.png) In order to monitor the unit and always see it upon receiving the message, press the tracking icon next to its name. The icon will turn green, and a dot will appear inside of it. The unit should be already checked in the first \(_Show on map_\) column. If you click the icon in the header, the option will be applied to all the units marked in the first column.

#### Motion State <a id="motion_state"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/state.png)This column shows whether a unit is moving or stationary, as well as whether the ignition is on or off \(in case there is a corresponding [sensor](https://docs.wialon.com/en/hosting/cms/units/sensors/sensors)\). The motion state is defined on the basis of speed information in the latest message or a real-time motion sensor, if available.

To monitor the unit motion state, it is necessary to indicate the validity period of motion state icons \(the corresponding line in the _Monitoring_ panel customizer\). The validity period is the time interval \(in minutes\), after which the traffic state signs become inactive. Moreover, when the validity period expires, [unit movement directions](https://docs.wialon.com/en/hosting/user/monitor/display#other_markings) become hidden. The validity period can take a value from 1 to 999 minutes.

* ![](https://docs.wialon.com/en/hosting/_media/icons/state1.png) — the unit is moving \(if there is an ignition sensor, this icon also shows that the unit is moving with the engine off, that is, it is being towed or transported\);
* ![](https://docs.wialon.com/en/hosting/_media/icons/state2.png) — the unit is moving, the engine is on;
* ![](https://docs.wialon.com/en/hosting/_media/icons/state3.png) — the unit is stationary;
* ![](https://docs.wialon.com/en/hosting/_media/icons/state4.png) — the unit is stationary, the engine is on;
* ![](https://docs.wialon.com/en/hosting/_media/icons/state5.png) — the last message from the unit was received over an hour ago: the unit was moving;
* ![](https://docs.wialon.com/en/hosting/_media/icons/state6.png) — the last message from the unit was received over an hour ago: the unit was stationary;
* ![](https://docs.wialon.com/en/hosting/_media/icons/state7.png) — the unit data is received with the help of [LBS detection](https://docs.wialon.com/en/hosting/cms/units/adv#messages_validity_filtration);
* ![](https://docs.wialon.com/en/hosting/_media/icons/state8.png) — the data obtained with the help of LBS detection is outdated;
* ![](https://docs.wialon.com/en/hosting/_media/icons/state9.png) — there are no messages from the unit.

In case the unit is stationary, the tooltip displays the duration of this state. If the unit has a [real-time motion sensor](https://docs.wialon.com/en/hosting/cms/units/sensors/types), the information about the duration is absent.

#### Data Accuracy <a id="data_accuracy"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/actuality.png)This column indicates the data accuracy: how many satellites locked the unit and when the latest message was received. To find out the exact time of the latest information update, hover the mouse cursor over the icon and study the tooltip.

The _first bar_ indicates the availability of the satellites:

* ![](https://docs.wialon.com/en/hosting/_media/icons/act1.png) green — the satellites are available \(see the exact number of the locked satellites in the tooltip\);
* ![](https://docs.wialon.com/en/hosting/_media/icons/act4.png) red — the satellites are not available;
* ![](https://docs.wialon.com/en/hosting/_media/icons/act5.png) grey — the satellites are not available for the period greater than the one indicated in the _Options customizer_ menu for the _Motion state_ option.

The _second bar_ shows the latest data received from the unit:

* ![](https://docs.wialon.com/en/hosting/_media/icons/act1.png) green — the unit sent the data less than 5 minutes ago;
* ![](https://docs.wialon.com/en/hosting/_media/icons/act2.png) yellow — the unit sent the data within the last hour;
* ![](https://docs.wialon.com/en/hosting/_media/icons/act3.png) orange — the unit sent the data in the last 24 hours;
* ![](https://docs.wialon.com/en/hosting/_media/icons/act4.png) red — no messages for a long period of time;
* ![](https://docs.wialon.com/en/hosting/_media/icons/act5.png) grey — the object never sent the data.

You can customize the unit filtering in the _Monitoring_ panel and/or on the map by the relevance of the latest message. To do this, change _Without filtration_to _Monitoring panel_ or _Panel + Map_ and specify the filtration interval in minutes. The filtration can affect only the work list in the _Monitoring_ panel or both the worklist and the map. Read more about the dynamic work list [here](https://docs.wialon.com/en/hosting/user/monitor/list#dynamic_work_list).

[Actualizer](http://apps.wialon.com/?lang=en#actualizer) app can help reveal inactive units. This application allows to set any period of inactivity.

#### Connection State <a id="connection_state"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/connection_.png)Shows whether there is a connection with the unit at the moment.

* ![](https://docs.wialon.com/en/hosting/_media/icons/connection.png) — the unit is connected;
* ![](https://docs.wialon.com/en/hosting/_media/icons/connection0.png) — the unit is not connected.

A unit is considered to be connected if it has TCP or UDP commands available, or it has sent messages within last X minutes. The required number of minutes can be indicated in the corresponding line of the _Monitoring panel_ customizer \(from 0 to 999\). By default, the value is 0. It means that the connection state is determined automatically and does not depend on the time of receiving messages.

#### Sensor State <a id="sensor_state"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/sensor-state.png)This column displays the state of the [sensor](https://docs.wialon.com/en/hosting/cms/units/sensors/sensors):

* ![](https://docs.wialon.com/en/hosting/_media/icons/sensor-red.png) ![](https://docs.wialon.com/en/hosting/_media/icons/sensor-green.png) ![](https://docs.wialon.com/en/hosting/_media/icons/sensor-blue.png) \(or any other color\) — visualizes the sensor value \(the color is set in the [sensor properties](https://docs.wialon.com/en/hosting/cms/units/sensors/props#intervals_and_colors), and the sensor is selected in the [_Advanced properties_](https://docs.wialon.com/en/hosting/cms/units/adv#usage_of_sensor_colors) tab\);
* ![](https://docs.wialon.com/en/hosting/_media/icons/sensor-text.png) — text parameters \(can be properly adjusted through a custom sensor\);
* ![](https://docs.wialon.com/en/hosting/_media/icons/sensor-unknown.png) — the option is not activated for this unit;
* ![](https://docs.wialon.com/en/hosting/_media/icons/support0.png) — the value is unknown.

When placing the mouse cursor over the square, you can see the name of the sensor and its value \(or description\) in the tooltip.

#### Battery level <a id="battery_level"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/battery-level.png)In this column the the battery level of the device is displayed. There are 4 available states:

* ![](https://docs.wialon.com/en/hosting/_media/icons/battery-red.png) — battery level from 0 to 25%;
* ![](https://docs.wialon.com/en/hosting/_media/icons/battery-orange.png) — battery level from 26 to 50%;
* ![](https://docs.wialon.com/en/hosting/_media/icons/battery-yellow.png) — battery level from 51 to 75%;
* ![](https://docs.wialon.com/en/hosting/_media/icons/battery-green.png) — battery level from 76 to 100%.

The exact value of the charge is shown in the icon's tooltip. If there is no [proper sensor configured](https://docs.wialon.com/en/hosting/cms/units/adv#usage_of_sensor_colors) for the unit, then next to its name in this column the ![](https://docs.wialon.com/en/hosting/_media/icons/sensor-unknown.png) sign is displayed, the tooltip of which says: _State is unknown_. If the sensor sends an invalid date that cannot be converted into percent using the calculation table, then in the column the ![](https://docs.wialon.com/en/hosting/_media/icons/support0.png) icon is displayed. In its tooltip it is written: _Error_.

### Options of action <a id="options_of_action"></a>

The parameters of the last two sections are designed for the execution of some action on the unit.

#### Quick Track <a id="quick_track"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/track_.png)The buttons allow to build a track of unit movements.

* ![](https://docs.wialon.com/en/hosting/_media/icons/track.png) — show a track on the map;
* ![](https://docs.wialon.com/en/hosting/_media/icons/track0.png) — remove a track from the map;
* ![](https://docs.wialon.com/en/hosting/_media/icons/track_no.png) — not enough rights to query tracks for this unit.

When pressing the _Show Track_ button next to a unit, the track of this unit appears on the map. In the panel settings, you should also specify the interval for track building: _Yesterday_, _Week_, _Month_ or _Other_ \(manual mode\). Other parameters \(such as line width, annotations, markers, trip detector, etc.\) are taken from the [_Tracks_](https://docs.wialon.com/en/hosting/user/tracks/tracks) panel. All 'quick' tracks are displayed in the _Tracks_ panel where you can manipulate them in the same way as the usual ones: show/hide, remove from the map, etc. Track colors can be set in the unit properties in the _Advanced_ tab or in the _Tracks_ panel as well.

#### Messages <a id="messages"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/msg_.png)Request [messages](https://docs.wialon.com/en/hosting/user/msg/msg) from a unit.

* ![](https://docs.wialon.com/en/hosting/_media/icons/messages-01.png) — display messages;
* ![](https://docs.wialon.com/en/hosting/_media/icons/messages_-01.png) — not enough rights to query messages from this unit.

The requested data is displayed in the _Messages_ panel. The standard time interval \(_Today_, _Yesterday_, _Week_ or _Month_\) for the query is set in the _Monitoring_ panel customizer. If _Other_ is selected, the interval is taken from the _Messages_ panel. In this case, only messages with data are loaded, and the style of display is taken from the panel itself.

#### Quick Report <a id="quick_report"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/report.png)Quick [report](https://docs.wialon.com/en/hosting/user/reports/reports) execution.

* ![](https://docs.wialon.com/en/hosting/_media/icons/report-02.png) — execute a report;
* ![](https://docs.wialon.com/en/hosting/_media/icons/report-03.png) — not enough rights to execute reports for this unit or a report template is unavailable.

The requested report is generated in the panel based on the template selected in the _Monitoring_ panel customizer. Standard time interval \(_Today_, _Yesterday_, _Week_ or _Month_\) is also configured there. The time interval can either be standard or _Other_, which means it is taken from the _Report_ panel.

#### Media <a id="media"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/picture_.png)View the latest [media files](https://docs.wialon.com/en/hosting/user/monitor/pics) \(pictures or video\) received from the unit \(works for the devices that have such functionality\).

* ![](https://docs.wialon.com/en/hosting/_media/icons/picture.png) — the button to view media files;
* ![](https://docs.wialon.com/en/hosting/_media/icons/picture0.png) — no pictures \(video\) available.

#### Video <a id="video"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/video.png)Opening a mini-window in the mode of video monitoring.

* ![](https://docs.wialon.com/en/hosting/_media/icons/video_active.png) — click the button to open a mini-window in the mode of video monitoring;
* ![](https://docs.wialon.com/en/hosting/_media/icons/video_inactive.png) — there is no video available for the unit.

#### Commands <a id="commands"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/cmd_.png)Buttons to send [commands](https://docs.wialon.com/en/hosting/user/monitor/cmd) to units:

* ![](https://docs.wialon.com/en/hosting/_media/icons/cmd.png) — there are available commands;
* ![](https://docs.wialon.com/en/hosting/_media/icons/cmd-gprs.png) — there are available commands, including GPRS commands \(using TCP or UDP channel\);
* ![](https://docs.wialon.com/en/hosting/_media/icons/cmd-gprs0.png) — there are available commands, including GPRS commands, however, the current user does not have enough access rights to execute them;
* ![](https://docs.wialon.com/en/hosting/_media/icons/cmd0.png) — there are no commands available or no rights to execute them.

#### SMS <a id="sms"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/sms_.png)[Send SMS](https://docs.wialon.com/en/hosting/user/tools/sms) to the unit or driver \(the addressee is selected in the drop-down menu if both options are available\). For full functionality, the current user should have the rights to send SMS, as well as the right to _Edit connectivity settings_ of the unit.

* ![](https://docs.wialon.com/en/hosting/_media/icons/sms.png) — send SMS to the unit or driver;
* ![](https://docs.wialon.com/en/hosting/_media/icons/sms0.png) — the user has the right to send SMS, but there are no available phone numbers of the unit or driver.

#### Events Registrar <a id="events_registrar"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/reg_.png)Manual registration for such events as fuel fillings, maintenance service and other events in the unit history.

* ![](https://docs.wialon.com/en/hosting/_media/icons/reg.png) — open registrar;
* ![](https://docs.wialon.com/en/hosting/_media/icons/reg0.png) — not enough rights to register events for this unit.

#### Properties <a id="properties"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/dialog.png)View [unit](https://docs.wialon.com/en/hosting/cms/units/units#unit_properties_dialog) or [group](https://docs.wialon.com/en/hosting/cms/groups/props) properties dialog \(depending on the mode of work list display\). In case of groups, the button can be different depending on the [access rights](https://docs.wialon.com/en/hosting/cms/rights/rights).

* ![](https://docs.wialon.com/en/hosting/_media/icons/edit.png) — some group properties can be edited;
* ![](https://docs.wialon.com/en/hosting/_media/icons/view.png) — view only.

#### Clear List <a id="clear_list"></a>

![](https://docs.wialon.com/en/hosting/_media/icons/del-all.png)The buttons used to clear the list. To remove all the units or groups from the list, press the button in the header of the table. The same button is located in front of each unit or group and allows to remove the items individually.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) If the options are selected for the additional menu \(i.e. checked in the second column of the _Monitoring_ panel customizer\), you can find them in the column with the icon ![](https://docs.wialon.com/en/hosting/_media/icons/menu_.png) under the button ![](https://docs.wialon.com/en/hosting/_media/icons/menu.png).

#### Other <a id="other"></a>

Other buttons and signs that can be found in the _Monitoring_ panel:

| ![](https://docs.wialon.com/en/hosting/_media/icons/check_box.png) | The units that are selected for display on the map are checked in the first column of the table. To select all the units, check the icon at the top of the table. |
| :--- | :--- |
| ![](https://docs.wialon.com/en/hosting/_media/icons/az.png) | A switch-button which shows that the items of the work list are sorted by name in direct order. |
| ![](https://docs.wialon.com/en/hosting/_media/icons/za.png) | A switch-button which shows that the items of the work list are sorted by name in reverse order. |
| ![](https://docs.wialon.com/en/hosting/_media/icons/list.png) | A switch-button which shows that the worklist displays singular units. |
| ![](https://docs.wialon.com/en/hosting/_media/icons/tree.png) | A switch-button which shows that the worklist displays a tree view of the units \(with grouping\). Read more about the [work list settings](https://docs.wialon.com/en/hosting/user/monitor/list). |
| ![](https://docs.wialon.com/en/hosting/_media/icons/add-units.png) | The button to find and add the units or groups to the list. |
| ![](https://docs.wialon.com/en/hosting/_media/icons/add-all.png) | The button to add all available units or groups to the [work list](https://docs.wialon.com/en/hosting/user/monitor/list). |
| ![](https://docs.wialon.com/en/hosting/_media/icons/customizer.png) | _Monitoring_ panel customizer \(columns selection\). |

![](https://docs.wialon.com/en/hosting/lib/exe/indexer.php?id=user%3Amonitor%3Aicons&1550649929)

