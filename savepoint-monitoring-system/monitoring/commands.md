# Commands

A command is a request that can be sent to a unit. In response, the unit can send its coordinates, take a picture, activate an output, block engine, etc. Available commands depend on the [type of device](http://gurtam.com/en/gps_tracking/gps_hardware.html)used and its configuration.

To be executed, a command should be configured in [Unit Properties](https://docs.wialon.com/en/hosting/cms/units/aliases) in the corresponding tab. To send a command, the user must have the rights specified in its properties, as well as the _Execute commands_ right in relation to the unit.

### Standard Commands <a id="standard_commands"></a>

17 standard commands are reserved in Wialon:

| Icon | Command | Name in the system | Parameters |
| :--- | :--- | :--- | :--- |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_query_pos.png) | Query position \(request current coordinates of the unit\) | query\_pos | — |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_block_engine.png) | Block engine | block\_engine | — |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_unblock_engine.png) | Unblock engine | unblock\_engine | — |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_output_on.png) | Activate output | output\_on | output number |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_output_off.png) | Deactivate output | output\_off | output number |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_download_msgs.png) | Download messages | download\_msgs | time interval \(from – to\) |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_set_report_interval.png) | Set data transfer interval \(how often unit sends data to the server\) | set\_report\_interval | interval in seconds |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_custom_msg.png) | Send custom message \(to send a non-standard command to a unit\) | custom\_msg | command text |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_driver_msg.png) | Send message to driver | driver\_msg | message text |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_send_position.png) | Send position | send\_position | coordinates |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_send_route.png) | Send route | send\_route | checkpoints |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_send_waypoints.png) | Send waypoints | send\_waypoints | checkpoints |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_query_config.png) | Query configuration | request\_configuration | — |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_start_stop.png) | Start/Stop WiaTag | wiatag\_service | — |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_upload_cfg.png) | Upload configuration | upload\_cfg | path to configuration file |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_upload_sw.png) | Upload firmware | upload\_sw | path to firmware file |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_query_photo.png) | Query snapshot | query\_photo | — |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_query_camera.png) | Query snapshot from camera | query\_photo\_cam | camera's number |
| ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_query_ddd.png) | Query DDD file \(for tachographs\) | query\_ddd | — |

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) To download the requested configuration file, use the [_Disketta_](http://apps.wialon.com/?lang=en#disketta) application \(the required file is located in the _Unit_ folder\). To find out the name of the configuration file, generate a [table with messages](https://docs.wialon.com/en/hosting/user/msg/manage#request_messages_from_server) for the corresponding period.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) If your device supports a command that is not mentioned in the list above, this command can still be sent. To do this, use the standard command _Send custom message_. In this case, you should know the exact name of the command \(as it is written in the device configuration\).

### Sending and Tracking Commands <a id="sending_and_tracking_commands"></a>

There are several ways to send a command to a unit:

* Manually [from the Monitoring panel](https://docs.wialon.com/en/hosting/user/monitor/cmd#executing_commands_from_the_monitoring_panel), including sending the command to a whole group of units.
* As a [job](https://docs.wialon.com/en/hosting/user/jobs/cmd) ran automatically according to a schedule.
* As an action for a triggered [notification](https://docs.wialon.com/en/hosting/user/notify/action) \(command is sent when specified conditions are met\).
* From a mobile device using a plain SMS text message.
* From the [Wialon Mobile Client](https://docs.wialon.com/en/hosting/mobile/mobile0/commands).

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Such commands as _Upload configuration_ and _Upload firmware_ have their own peculiarities. If these commands have been saved for units without selecting a file, sending these commands as a job/notification or sending them to the whole group of units is impossible.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Such commands as _Send route_ and _Send waypoints_ also have some peculiarities. When you send them, you should manually indicate the route parameters. Therefore, these commands cannot be sent via job or notification.

Information about commands sent to a unit is available:

* In the [Messages](https://docs.wialon.com/en/hosting/user/msg/cmd) panel \(all commands sent to a unit\).
* In the [Executed commands](https://docs.wialon.com/en/hosting/user/reports/tables/cmd) report \(only successfully executed commands\).
* Immediately after sending a command — in the [log](https://docs.wialon.com/en/hosting/user/gui/log).

### Executing Commands from the Monitoring Panel <a id="executing_commands_from_the_monitoring_panel"></a>

A command can be sent from the _Monitoring_ panel. This option must be activated in the [Monitoring panel customizer](https://docs.wialon.com/en/hosting/user/monitor/icons). The button can have different looks:  
![](https://docs.wialon.com/en/hosting/_media/icons/cmd.png) there are available commands for the selected unit;  
![](https://docs.wialon.com/en/hosting/_media/icons/cmd-gprs.png) there are GPRS commands among the available ones;  
![](https://docs.wialon.com/en/hosting/_media/icons/cmd0.png) or ![](https://docs.wialon.com/en/hosting/_media/icons/cmd-gprs0.png) there are no commands supported by the selected unit or the current user has not enough access to the unit.

Put the cursor over the active button next to the required unit to see the list of available commands. The list can contain only commands configured in [Unit Properties =&gt; Commands](https://docs.wialon.com/en/hosting/cms/units/aliases). Furthermore, only commands available at the moment are shown \(the availability of link types is important here\).

![](https://docs.wialon.com/en/hosting/_media/monitor/cmd1.png)

1. Click the command button ![](https://docs.wialon.com/en/hosting/_media/icons/cmd.png) or ![](https://docs.wialon.com/en/hosting/_media/icons/cmd-gprs.png).
2. Select the required units. This step can be omitted if a command is sent to one unit.
3. Select a command from the list of commands available at the moment. When sending a command to several units, special symbols indicate whether this command can be sent to all selected units or only to some of them:

* ![](https://docs.wialon.com/en/hosting/_media/icons/support.png) all selected units support this command;
* ![](https://docs.wialon.com/en/hosting/_media/icons/support0.png) not all of the selected units support this command \(more information is in the tooltip\).

![](https://docs.wialon.com/en/hosting/_media/monitor/cmd2.png)

1. If needed, set additional parameters, for example, input/output index, report interval, path to load a configuration or firmware file, [checkpoints of the route](https://docs.wialon.com/en/hosting/user/monitor/cmd#route_sending), etc.
2. Press _OK_. The command is executed immediately, and its result is reported in the [log](https://docs.wialon.com/en/hosting/user/gui/log). To show or hide the log window click on the double-arrow in the right bottom corner of the window.

While executing the _Send custom message_ command, it is possible to enter the text in the following ways:

* You can enter the message manually in the corresponding field. To make the search process easier during the next command execution, it is possible to add a message to a group. The principle of working with groups has been described [above](https://docs.wialon.com/en/hosting/cms/units/aliases).
* It is possible to choose a previously saved message. In the drop-down list of groups, choose the one which contains the message. Below, you get the list of available messages. Select the required one and press _OK_ to execute the command.

![](https://docs.wialon.com/en/hosting/_media/monitor/cmd4.png)

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Note._  
To send a command to a group of units, it is necessary for this command to be registered in the properties of each of these units on the _Commands_ tab and have the same name. If, when sent to several units, the command is called the same, but belongs to a different type and the parameters are not specified, then the command is sent without parameters and, as a result, cannot be executed.

### Chat with Driver <a id="chat_with_driver"></a>

The operator \(dispatcher\) can exchange messages with [drivers](https://docs.wialon.com/en/hosting/user/drivers/drivers). To do this, select the _Send message to driver_ command and enter the text.

In case the driver answers, the message appears in a special pop-up window. A new message can be accompanied by a sound \(see [User Settings](https://docs.wialon.com/en/hosting/user/set/general)\). If you have unread messages, the number of them is indicated in the red circle next to the chat icon in the bottom panel. If there are any messages in the window \(either read or unread\), the icon itself is active which means it is colored and can be clicked on.

![](https://docs.wialon.com/en/hosting/_media/monitor/cmd3.png)

Newly received messages are added to the top of the list. Unread notifications have a blue background by default. To expand/hide the full text of a message, use the switch button \(+/-\) or click on the header of the notification outside the text.

When clicking on a message, the map is centered on the place where this message was sent. When clicking on the unit name, the map is focused on its last location.

To delete a message, click on the cross to the right of its title. You can also delete the read messages or all messages if you use the appropriate buttons at the bottom of the messages window. The window is closed automatically when you delete all messages. If the online notifications window is closed by clicking on the grey cross in the upper right corner, the window stops appearing automatically when new notifications are received. Click on the corresponding button in the bottom panel to open the window.

In addition, the window itself can be dragged around the screen and resized. The position and size of the window are remembered until the next opening.

The operator can quickly send a reply to the driver \(the _Send messages to driver_ command should be configured in the unit properties in advance\). Click on the green triangle-shaped button and enter the response text in the dialog box to send it.

Besides, you can generate the report called [_Chat_](https://docs.wialon.com/en/hosting/user/reports/tables/chat), which contains all the chat history including the operator and driver messages for the specified period of time.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Note. The automatic appearance of messages from the drivers on the screen can be turned off. To do this, uncheck the _Automatical display popup events_box in the user settings. In this case, the arrival of a new notification will be indicated only by the appearance of a figure in a red background in the bottom panel of the program next to the communication icon. To read the notifications, you need to click on this sign.

It is convenient to communicate with the driver with the help of a specially developed app — [Chatterbox](http://apps.wialon.com/?lang=en#chatterbox). This application allows to send not only commands but also text messages.

### Sending Route/Sending Waypoints <a id="sending_routesending_waypoints"></a>

To send a route, it is necessary to indicate its name in the corresponding field of the dialog.

To send a route/waypoints, it is necessary to indicate its checkpoints in the command dialog. Checkpoints can be found in various sources: addresses, geofences, routes. You can apply the search filter \(buttons at the top of the dialog\) which helps you to expand/narrow the number of sources to be used. Enabled button means that the corresponding source is applied as a filter.

To indicate a checkpoint, start typing in the corresponding field. In the dropdown list, depending on the filter used, you can find the possible variants along with their source information.

Moreover, you can add a checkpoint directly from the map. To do this, click on the ![](https://docs.wialon.com/en/hosting/_media/icons/point_on_map.png) icon to the right of the field. Move on the map to the target position, and double-click on it. As a result, a checkpoint will be indicated automatically.

If a checkpoint is added from a route, all the points of the route are added. However, if the route contains moving units as checkpoints, they will be omitted.

the coordinates of the first checkpoint are used when you add them from line or polygon type geofences.

After the required checkpoint is entered, a green check mark appears to the right of it. This check mark is a point validity indicator which shows that a checkpoint possesses coordinates. The checkpoint name cannot be edited, it is filled in automatically. If you try to edit the name, the search results will be reset \(point validity indicator disappears\) and you should start the search again. Every indicated checkpoint has a _Notice_ field under it. This field is optional.

The indicated checkpoints can be saved as a route, and afterwards you can use it in the [_Routes_](https://docs.wialon.com/en/hosting/user/routes/routes) panel of the tracking system. To do this, check the box at the bottom of the dialog. You can also give a name to the route during checkbox activation \(for sending waypoints only\). Click _OK_ to complete the procedure. Route saving takes place simultaneously with the sending of the command.

![](https://docs.wialon.com/en/hosting/_media/monitor/send_route.png)

