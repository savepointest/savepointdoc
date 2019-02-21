# Mapping a Track

![](https://docs.wialon.com/en/hosting/_media/tracks/params.png)

To build a track in the _Tracks_ panel, do the following:

1. Select a **unit** in the dropdown list. Its contents depend on the [worklist](https://docs.wialon.com/en/hosting/user/monitor/list) in the _Monitoring_ panel and access to the units. In case the worklist is empty \(when the [dynamic work list](https://docs.wialon.com/en/hosting/user/monitor/list#dynamic_work_list) is used or when units were deleted from the work list manually\), the units to which you possess the corresponding rights are displayed.
2. Adjust the desired [**parameters**](https://docs.wialon.com/en/hosting/user/tracks/params) for the track \(color, thickness, etc.\).
3. Define the **time interval** within which you want to get the data.
4. After filling in all the fields, press _Show Track_.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) To display the _tracks_ on the map, the corresponding [layer](https://docs.wialon.com/en/hosting/user/gui/map#visible_layers) must be activated.

The principle of interval adjustment is the same as in the reports \(see [Query and View Reports](https://docs.wialon.com/en/hosting/user/reports/query/query)\). The third and fourth steps can be combined into one if you use one of the _quick intervals_ \(the buttons _Today_, _Yesterday_, _Week_, and _Month_\).

A point-to-point track that is built according to the preset parameters will appear on the map \(if the unit has any messages with the coordinates for the period\). If it takes too long for the track to appear on the map, it means you either indicated an interval that is too long or your Internet speed is too low.

If within the indicated period the unit was not moving, there will be no track on the map. However, it can be found in the list of tracks below, and the distance traveled will be 0 km.

A track or its part can be displayed on the map as a dashed line. Such a situation indicates that the data in this part of the track might be inaccurate. For instance, the maximum interval between the messages is exceeded \(see the [_Advanced_](https://docs.wialon.com/en/hosting/cms/units/adv#parameters_used_in_reports) tab\) or the number of satellites is less than 4 \(if the [validity filtration of messages](https://docs.wialon.com/en/hosting/cms/units/adv#messages_validity_filtration) is disabled\).

![](https://docs.wialon.com/en/hosting/_media/tracks/invalid.png)

When the private mode of the trip is detected \(if the unit has the _Private mode_ type sensor with the _Do not show unit location_ option enabled\), the _work_ trips are connected with the straight dashed line.

Alternative methods to build a track on the map are:

* In the [_Monitoring_](https://docs.wialon.com/en/hosting/user/monitor/monitor) panel with the help of quick track buttons.
* In the [_Messages_](https://docs.wialon.com/en/hosting/user/msg/data) panel when you view data messages.
* In the [_Reports_](https://docs.wialon.com/en/hosting/user/reports/templ/settings/map) panel, if the appropriate option is selected in the report template.

