# Events Registrar

Different events can be registered in the unit history and then shown in the corresponding reports. Some events such as speeding, idling, visits to [geofences](https://docs.wialon.com/en/hosting/user/geo/geo), [sensor](https://docs.wialon.com/en/hosting/cms/units/sensors/sensors) values, etc. can be detected automatically by the system with the help of [notifications](https://docs.wialon.com/en/hosting/user/notify/notify). Other events such as fuel filling, maintenance or any custom events are registered in unit history manually with the help of a special tool — **Events Registrar**.

To display the registrar, press the button in the monitoring panel ![](https://docs.wialon.com/en/hosting/_media/icons/reg.png). If you do not see such a button, it can be added with the help of the [monitoring panel customizer](https://docs.wialon.com/en/hosting/user/monitor/icons).

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Attention!_  
To register events for a unit, the _Manage events_ access right is needed. Otherwise, the registrar button is not active.

In the drop-down menu, select the required type of the event:

* [make a record in unit log](https://docs.wialon.com/en/hosting/user/monitor/reg#record_in_the_log),
* [register custom event](https://docs.wialon.com/en/hosting/user/monitor/reg#custom_event),
* [register unit status](https://docs.wialon.com/en/hosting/user/monitor/reg#unit_status),
* [register filling](https://docs.wialon.com/en/hosting/user/monitor/reg#fuel_filling),
* [register maintenance work](https://docs.wialon.com/en/hosting/user/monitor/reg#maintenance_work).

![](https://docs.wialon.com/en/hosting/_media/monitor/reg.png)

Fill in the required fields and click _OK_. If you need to register several events for one unit, click _Save and continue_. The entry will be added to the log \(the corresponding caption appears in the lower-left corner of the dialog\), and you can proceed to register the next event.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Note._  
Units of measurement which you may encounter in the registrar dialog depend on the [measurement system](https://docs.wialon.com/en/hosting/cms/convers/convers) set in the unit properties.

### Record in the Log <a id="record_in_the_log"></a>

Using this option, you can add any text note to the unit log. It will be labeled as _Manual record_ and dated by the time of creation. Such records can be viewed in [messages](https://docs.wialon.com/en/hosting/user/msg/log) \(messages type _Log_\) and in [reports](https://docs.wialon.com/en/hosting/user/reports/tables/logs) generated for this unit \(query the _Log_ table\).

![](https://docs.wialon.com/en/hosting/_media/monitor/reg-log.png)

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) To add messages to the log, you should have not only the _Manage events_ access but also the _Manage log_ access.

### Custom Event <a id="custom_event"></a>

To register a custom event, enter its name, description, and location. To add the location, click on the ![](https://docs.wialon.com/en/hosting/_media/icons/point_on_map.png) icon to the right of it. On the map that appears, double-click on the required position. The address is defined by the maps selected as [geodata source](https://docs.wialon.com/en/hosting/user/set/maps) in User Settings. Gurtam Maps. In addition, the position can be entered manually. To clear the field, delete the address.

![](https://docs.wialon.com/en/hosting/_media/monitor/reg-custom.png)

The description of the registered event can be saved. To do this, click on the _Save_ icon to the right of it. The saved description appears in the list below. To select an existing description, click on it. To delete a description from the list, select it and click on the _Delete_ icon.

If you check the _Violation_ option, the event will be registered in the unit history as a violation, otherwise, it will be registered as a simple event. It means this event will appear in different kinds of reports: [Events](https://docs.wialon.com/en/hosting/user/reports/tables/events) or [Violations](https://docs.wialon.com/en/hosting/user/reports/tables/violations).

### Unit Status <a id="unit_status"></a>

Using this functionality, you can register the beginning of a state, which can be afterwards displayed in some reports. For instance, the status can be like _business/private_ is a vehicle is used both for personal and business needs.

![](https://docs.wialon.com/en/hosting/_media/monitor/reg-event.png)

The process of registration is the same as for the custom event. You choose the date and time and enter any text. The text can be saved and used in other registrations. It is important to set the correct date and time as they will be counted as the beginning of the status. The state comes to end when a new state is registered.

Statuses can be set automatically \(for example, when the unit enters a geofence\) — see [Notifications](https://docs.wialon.com/en/hosting/user/notify/notify). Columns with the corresponding contents are available in several reports which are [Trips](https://docs.wialon.com/en/hosting/user/reports/tables/trips), [Engine hours](https://docs.wialon.com/en/hosting/user/reports/tables/eh), [Rides](https://docs.wialon.com/en/hosting/user/reports/tables/rides), and [Parkings](https://docs.wialon.com/en/hosting/user/reports/tables/parkings).

### Fuel Filling <a id="fuel_filling"></a>

In the _Monitoring_ panel, you can manually register fuel fillings for units. Manual registration helps to estimate the difference between the registered fuel filling and the factual one, compare the consumed amount with consumption rates, calculate running costs, etc.

To register fuel filling, select the corresponding event in the drop-down list and fill in the required fields.

![](https://docs.wialon.com/en/hosting/_media/monitor/reg-filling.png)

Enter the volume of filled fuel and its cost. Fractional numbers \(up to hundredth\) can be also used for fuel volume and cost. To enter fractional numbers, use a _period_ as the separator. For example, to register fuel filling for 77 dollars and 88 cents, enter _77.88_.

Entered values are automatically added to the _Description_ field above. If necessary, you can edit the description manually. Then enter the date and time when the filling took place, possible deviation from this time in minutes and [specify](https://docs.wialon.com/en/hosting/user/monitor/reg#custom_event) the location.

Registered fuel fillings participate in the following reports: [_Fuel fillings_](https://docs.wialon.com/en/hosting/user/reports/tables/fillings), [_Events_](https://docs.wialon.com/en/hosting/user/reports/tables/events), [_Utilization cost_](https://docs.wialon.com/en/hosting/user/reports/tables/cost).

### Maintenance Work <a id="maintenance_work"></a>

To register a maintenance work, select the corresponding event in the drop-down list and fill in the required fields.

![](https://docs.wialon.com/en/hosting/_media/monitor/reg-service.png)

Enter the following data:

* kind of work \(type from the keyboard or select from the list below\);
* description;
* values of mileage and engine hours counters at the moment of the event \(the current values are displayed but you can edit them\);
* cost;
* service duration in minutes, hours or days \(choose the type of the interval from the drop-down list\);
* date and time of maintenance \(by default, the current date and time are displayed\);
* location \(press the _Select Location_ icon and double click on the map to specify the position or edit this field manually\).

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Attention!_ In the _Mileage_ field it is not possible to enter a value that exceeds 2147483 km.

In the upper part of the dialog, you see the list of service intervals from the [_Service intervals_](https://docs.wialon.com/en/hosting/cms/units/maint) tab. Check the services that have been carried out. This is required in order for the selected intervals to be zeroed and the countdown to start anew. Keep in mind that if you select any maintenance interval here, the contents of the _Kind of work_ field changes correspondingly.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Attention!_ Registered events are not editable. They can only be deleted from the unit history in the [_Messages_](https://docs.wialon.com/en/hosting/user/msg/msg#deleting_messages) panel \(special access is required\).

### Registered Events in Reports <a id="registered_events_in_reports"></a>

Registered fillings and maintenance can appear in the [report on events](https://docs.wialon.com/en/hosting/user/reports/tables/events) together with other actions. A registered custom event depending on your choice can get in the report on events or [report on violations](https://docs.wialon.com/en/hosting/user/reports/tables/violations). Both reports have the similar structure.

When transporting registration data to a report on events \(violations\), the information is distributed among the columns, the contents of which are taken from certain fields of the registration dialog. The table below gives a correspondence between the column of the report and the fields of the registrar.

| **Column Header** | **Column Content** |
| :--- | :--- |
| **Event time** | Date and time when the event happened. |
| **Time received** | Date and time when event was registered. |
| **Event text** | Text is taken from the _Description_ field. For maintenance, if there is no description, the text can be taken from the _Kind of work_ field. |
| **Location** | Unit location at the time of the event. It is taken from the coordinates indicated while registering the event \(press the _Select Location_ button, and double-click on the map\). |

If any of the above-mentioned fields are not filled out correctly, the corresponding columns will be empty.

Other reports that use registered events are the [report on maintenance](https://docs.wialon.com/en/hosting/user/reports/tables/maintenance) and [utilization costs](https://docs.wialon.com/en/hosting/user/reports/tables/cost).  


