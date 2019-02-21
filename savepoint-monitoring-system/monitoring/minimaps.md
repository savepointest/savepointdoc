# Minimaps

The minimap is an additional window \(help window\) focused on the current information about the selected unit. Double click on the name of a unit in the monitoring list to open its minimap. The selected unit is centered on the map. Moreover, the window can be open by double-clicking on a unit on the map. However, in this case, the unit is not centered on the map.  


![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Note that if no messages with coordinates have been received from a unit, nothing happens when you double click on it.

![](https://docs.wialon.com/en/hosting/_media/monitor/mini-window.png)

### Minimap Modes <a id="minimap_modes"></a>

There are three modes available for minimaps: video, info, and map modes. They can be switched using the buttons ![](https://docs.wialon.com/en/hosting/_media/icons/video_active.png)/![](https://docs.wialon.com/en/hosting/_media/icons/map.png)/![](https://docs.wialon.com/en/hosting/_media/icons/info.png) in the right corner of the mini window header.

**Video**  
This mode allows to monitor a unit online and look through the video for a previous period. To activate the video mode, the user must enable the corresponding [service](https://docs.wialon.com/en/hosting/cms/accounts/services?&#list_of_services).

Besides the methods mentioned above, to switch to the video monitoring mode you can press the [corresponding button](https://docs.wialon.com/en/hosting/user/monitor/icons#video) in the _Monitoring_ panel.

At the top of the mini window, there are _Live_ and _Archive_ modes switch buttons \(on the left\), as well as the button for video display settings \(on the right\). By pressing the latter, it is possible to choose the cameras \(the maximum number of cameras is defined by the settings of the device\) and change their order by pulling the arrows on the left from the camera name to the required position. By default, the first camera is displayed.

![](https://docs.wialon.com/en/hosting/_media/monitor/video1.png)

The video is displayed in real time. Click on it to stop the broadcast; click again to resume it. The button in the lower right corner of the video allows you to switch to full-screen mode. At the same time, broadcasting from other cameras stops.

In addition to the standard player, video playback is also possible via a third-party player. To do this, enter the player’s IP address and protocol in the _IP_ field in the _Device configuration_ \(Unit properties → General → Device type → Icon ![](https://docs.wialon.com/en/hosting/_media/icons/edit.png)\).

Note that the protocol of the link to a third-party player must match the protocol of the monitoring site.

**Info**  


Switch to the info mode using the corresponding button in the minimap header. This mode dispays [extended unit information](https://docs.wialon.com/en/hosting/user/monitor/extra#extended_unit_information) selected in the right column of checkboxes in the corresponding block of [_User Settings_](https://docs.wialon.com/en/hosting/user/set/general#show_additional_information_about_the_unit).

**Map**  
The main purpose of the map mode is to show the location of a unit, as well as its speed and address from the last received message. The map cannot be moved, because it is automatically centered on the last position of a unit and it does not leave the field of vision. Except for this peculiarity, working with mini windows in the map mode is completely identical to working with the main map.

In the map mode, with the help of the corresponding buttons in the lower right corner of the mini-window, you can activate [Google Street View](http://en.wikipedia.org/wiki/Google_Street_View) or Yandex Panorama. These are submodes which allow to track units along the 'real' streets. Google Street View is a Google Maps feature that allows you to view panoramic views of the streets of many cities around the world from a height of about 2.5 meters. The service makes it possible to view houses, roads and all surrounding objects on the street, creating the illusion of a virtual presence. At the moment, the service covers North America, Australia, New Zealand, Western Europe, Japan, Indonesia, and Brazil. Yandex Panorama is also a panoramic view technology featured in Yandex maps. At the moment, Yandex Panorama allows you to view the panoramas of the streets of Russia, Ukraine, Belarus, Kazakhstan, and Turkey.

![](https://docs.wialon.com/en/hosting/_media/monitor/street_view.png)

Google Street View required the activation of Google Maps \([_User Settings_](https://docs.wialon.com/en/hosting/user/set/maps)\) and requires the availability of [coverage](http://en.wikipedia.org/wiki/Google_Street_View#Coverage) for the geographical area. For Yandex Panorama to work, activate the Yandex map and cover the corresponding viewing area.

### Online Notifications in Minimaps <a id="online_notifications_in_minimaps"></a>

Minimaps provide you with an alternative way of viewing [online notifications](https://docs.wialon.com/en/hosting/user/notify/online). Upon online notification triggering an opened minimap of a corresponding unit is highlighted in red. If the minimap is hidden, then it will be shown automatically upon receiving of a notification. To receive and view online notifications in minimaps, it is necessary to check the _Blink minimap_ box while choosing a [notification action](https://docs.wialon.com/en/hosting/user/notify/action).

![](https://docs.wialon.com/en/hosting/_media/monitor/minimap_notification.png)

An icon indicating a number of unread notifications appears in a minimap's header near the mode switcher. Click the icon to view received notifications. The concept of work with notification is identical to the one used in the online notifications window. To return to the initial mode used, click the notifications icon once again. ![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Note that a minimap is not synchronized to the online notifications window, therefore reading or deleting notifications in a minimap does not lead to any changes in the window of online notifications.

The maximum number of minimaps corresponds to 9 items. That is why if all the available windows are already opened, and a notification has come for a unit not opened in a minimap, then a notification will be available in the window of online notifications only.

### Manipulations with Minimaps <a id="manipulations_with_minimaps"></a>

There are a scaled icon and a unit name in the header of every help window in order to simplify the search of the necessary one. A mode switch and a close button are also situated in the header. You can open up to 9 help windows in the tracking system. Besides, you can use only one minimap per unit.

The button ![](https://docs.wialon.com/en/hosting/_media/icons/view_minimap.png) in the left corner of the [bottom panel](https://docs.wialon.com/en/hosting/user/gui/bottom) can be used to hide/show all minimaps at once. Apart from that, to avoid excessive information, minimaps are automatically hidden when you switch to the _Reports_, _Messages_, and _Routes_ panels \(but even then, they can be shown forcibly if necessary\). Minimaps are shown automatically upon leaving these panels.

The latest used layout of minimaps is restored each time a user authorizes in the system.  


