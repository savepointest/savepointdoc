# Filters and Masks

When creating various objects in the monitoring system \(geofences, drivers, custom fields, sensors, etc.\), lists are generated from them. Objects from the lists are displayed in the alphabetic order, with numbers first, then letters of the Latin alphabet, and then Cyrillic. Uppercase and lowercase letters are not taken into account. When you create a new object \(for example, new job or custom field\), it is originally added to the end of the list. When you later open this list, the objects will be arranged in the alphabetical order. After renaming, the object remains at its former place until you reopen the list.

Filters and masks are used for convenience. They allow to narrow the list of items in such a way that only the objects necessary for users are shown. Also, they allow to find the objects with particular characteristics or name in the list and specify the objects of tracking system towards which a report, notification, etc. will be applied.

### Dynamic Search <a id="dynamic_search"></a>

If the list contains a large number of items, it may be difficult to quickly find the required one. For your convenience, you can use the fast dynamic search. It is applicable for most panels. Start entering the name of the item \([geofences](https://docs.wialon.com/en/hosting/user/geo/geo), [units](https://docs.wialon.com/en/hosting/user/units/units), [routes](https://docs.wialon.com/en/hosting/user/routes/routes), etc. — depending on the panel you currently in\). The name can be typed starting from any place. While you enter the text, the list shows the items that match your query.

![](https://docs.wialon.com/en/hosting/_media/gui/filter.png)

If you leave the filter field empty, _all_ the available items will be displayed in the list.

The dynamic filter can also be found in the unit properties dialog, [unit groups](https://docs.wialon.com/en/hosting/user/units/groups), and users when adjusting the access rights. Moreover, the dynamic filter is used to select a resource when creating notifications, jobs, geofences, drivers/trailers \(their groups, automatic binding lists\), and also report templates.

The peculiarities of the dynamic filter usage in the Monitoring panel are described in the [_Unit List Management_](https://docs.wialon.com/en/hosting/user/monitor/list#units_search) section.

When searching, you can also enter the special characters such as \* and ?, the usage of which is described [below](https://docs.wialon.com/en/hosting/user/gui/masks#name_mask).

### Name Mask <a id="name_mask"></a>

Besides the dynamic search, filters are also used to specify an item, which is affected by [report](https://docs.wialon.com/en/hosting/user/reports/reports), [notification](https://docs.wialon.com/en/hosting/user/notify/notify), etc. To do this, specify a mask for the name of the element where you can use special characters: **asterisk \(\*\) and question mark \(?\)**.

An asterisk sign is a special symbol, which can be inserted into the query text to indicate any combination of valid characters in the unit name. An asterisk can be put anywhere in the query \(at the beginning, in the middle, at the end\) or in several places at once, depending on what part of the name is known or is the same for a number of items. For example, if you type _\*H\*nda\*_, all _Hondas_ and _Hyundais_ will be found.

Another special symbol that can be used is the question mark \(?\). It replaces any single character \(only one character\). The same as the asterisk sign, it can be put at any place of the query.

The request is case sensitive.

For example, a unit has two fuel sensors with the names _Fuel level sensor_ and _Fuel in tank_. It is necessary to create a notification that takes into account the readings of both of these sensors. To do this, in notification properties you need to set the name mask so that it matches both sensors. In this case, the best choice is _\*Fuel\*_:

![](https://docs.wialon.com/en/hosting/_media/gui/mask.png)

In all cases where it is suggested to set a mask, you can do without the use of asterisks and question marks, but in this case, you need to enter the exact name as it is in the system.

To find _all_ items of a certain type \(users, sensors, geofences, etc.\), simply enter one asterisk in the query field.

Masks are used:

* in [notifications](https://docs.wialon.com/en/hosting/user/notify/notify) to specify the monitored sensor, route or driver, as well as set SMS text mask or parameter in messages;
* in user properties to set host mask for [users](https://docs.wialon.com/en/hosting/cms/users/props);
* in [reports](https://docs.wialon.com/en/hosting/user/reports/reports) to specify the driver, sensor, event/violation, route and its geofence, and when selecting geofences;
* in the Messages panel to [filter](https://docs.wialon.com/en/hosting/user/msg/manage) found messages;
* in all panels of the mask instead of the [dynamic filter](https://docs.wialon.com/en/hosting/user/gui/masks#dynamic_filter).

### Manipulations with Lists <a id="manipulations_with_lists"></a>

When working with lists, keys and keyboard shortcuts can be used. Using the keys facilitates a lot of operations, such as list navigation, search for necessary items and their selection.

#### Dropdown Lists <a id="dropdown_lists"></a>

Dropdown lists are widely used in the monitoring system. They provide a possibility to work with a large number of items. For example, this can be a list of units available when generating a report, requesting messages, etc., a list of tables when editing report templates, etc.

When building tracks or querying messages and reports, you can use dynamic search in dropdown lists. For tracks and messages, you can quickly find a necessary unit in the dropdown list, for reports you can find templates or objects. To use the dynamic search, click the corresponding dropdown list and start entering the name. You can use a [wildcard character](https://docs.wialon.com/en/hosting/user/gui/masks#name_mask) asterisk \(\*\) to facilitate the search. As a result, the dropdown list is filtered according to the indicated symbols.

![](https://docs.wialon.com/en/hosting/_media/gui/dropdown.png)

To work with the dropdown list, you can use a keyboard. Use arrows \(up/down\) for navigation through the list and the _Enter_ key for choosing a necessary item.

#### Multiple Selection List Box <a id="multiple_selection_list_box"></a>

In the lists of such type, you can select multiple items. To choose several items throughout the list, hold the _Ctrl_ button, and consequently click on the necessary items.

![](https://docs.wialon.com/en/hosting/_media/gui/multiselect.png)

Moreover, the following keys, and their combinations can be used:

_Home_ — move to the beginning of the list;  
_End_ — move to the end of the list;  
&lt;⇑&gt; \(up arrow\) — move to the previous item;  
&lt;⇓&gt; \(down arrow\) — move to the next item;  
_Ctrl + A_ — select all;  
_Shift + Home_ — select everything from the current place to the beginning of the list;  
_Shift + End_ — select everything from the current place to the end of the list;  
_Shift + ⇑_ — consequently select the items going up from the current one;  
_Shift + ⇓_ — consequently select the items going down from the current one.

#### Checkbox List <a id="checkbox_list"></a>

Multiple selection lists may contain checkboxes indicating whether the item is selected or not. The _Ctrl + click_ combination can be used in such lists in order to check/uncheck all the items at once.

![](https://docs.wialon.com/en/hosting/_media/gui/checkedlist.png)

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Attention!_  
When working on MacOS, it is necessary to use the _Cmd + click_ combination instead of _Ctrl + click_.  


