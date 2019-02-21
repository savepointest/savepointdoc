# Work List Management



To monitor units, you need to place them in the work list. Only units presented in the worklist can be used to display on the map, as well as to apply various control elements: jobs and notifications execution, reports generating, drivers and trailers assigning, messages or tracks viewing, finding nearest units, etc.

The work list has several display modes:

* ![](https://docs.wialon.com/en/hosting/_media/icons/list.png) [simple list mode](https://docs.wialon.com/en/hosting/user/monitor/list#singular_units);
* ![](https://docs.wialon.com/en/hosting/_media/icons/tree.png) [tree-like mode](https://docs.wialon.com/en/hosting/user/monitor/list#treelike_view).

![](https://docs.wialon.com/en/hosting/_media/monitor/worklist.png)

Each of these lists is independent, and their settings are stored separately. When you switch between them, all settings that were last applied to this type of list are restored.

### Simple List Mode <a id="simple_list_mode"></a>

**Adding units to the work list**

To add units to the work list, use the following buttons in the header of a list:

* ![](https://docs.wialon.com/en/hosting/_media/icons/add-all.png) — add _all_ units available;
* ![](https://docs.wialon.com/en/hosting/_media/icons/add-units.png) — add particular unit\(s\). The [search tool](https://docs.wialon.com/en/hosting/user/monitor/list#search_tool) is used.

Moreover, there are alternative ways of adding units to the work list:

* from the [Online Notifications](https://docs.wialon.com/en/hosting/user/notify/online) window \(adding a unit that triggered the notification\);
* [dynamic formation](https://docs.wialon.com/en/hosting/user/monitor/list#dynamic_work_list) of the list depending on the relevance of the data.

Units created in the monitoring system or CMS Manager are automatically added to the worklist of the monitoring panel of the [user-creator](https://docs.wialon.com/en/hosting/cms/rights/creator) \(you may need to refresh the page or log in again\). If the group view monitoring mode is activated in the worklist, the new unit automatically gets in the group it was added to at creation, or to the _Units outside groups_ \(if it does not belong to any\).

If the [filtration on the basis of data accuracy](https://docs.wialon.com/en/hosting/user/monitor/list?&#dynamic_work_list) is used and the created unit does not meet the specified conditions, automatic addition to the list does not happen.

**Removing units from the worklist**

Units can be removed from the worklist individually or all at once:

* ![](https://docs.wialon.com/en/hosting/_media/icons/del.png) — the button next to each unit to remove this particular unit from the list;
* ![](https://docs.wialon.com/en/hosting/_media/icons/del-all.png) — the button in the header of the list to clear the work list \(to remove all units\).

Note that deleting units from the work list does not lead to their deleting from the system. They can be added back to the worklist using the ways described above. Units can be deleted from the system in the [_Units_](https://docs.wialon.com/en/hosting/user/units/units#units_management) panel.

**Sorting**

By default, the work list is sorted by names arranged in direct alphabetical order. The order can be reversed. To do this, use the switch button ![](https://docs.wialon.com/en/hosting/_media/icons/az.png) or ![](https://docs.wialon.com/en/hosting/_media/icons/za.png) in the header.

Besides, it is possible to sort units by other attributes such as motion state, connection quality, etc. To do this, click the corresponding button in the header:

* ![](https://docs.wialon.com/en/hosting/_media/icons/location.png) — location \(if Gurtam Maps are selected as the [map source](https://docs.wialon.com/en/hosting/user/set/maps)\);
* ![](https://docs.wialon.com/en/hosting/_media/icons/sensor-state.png) — sensor state;
* ![](https://docs.wialon.com/en/hosting/_media/icons/cmd_.png) — commands;
* ![](https://docs.wialon.com/en/hosting/_media/icons/state.png) — motion state;
* ![](https://docs.wialon.com/en/hosting/_media/icons/actuality.png) — last message time;
* ![](https://docs.wialon.com/en/hosting/_media/icons/connection_.png) — online connection state;
* ![](https://docs.wialon.com/en/hosting/_media/icons/picture_.png) — media files;
* ![](https://docs.wialon.com/en/hosting/_media/icons/track_.png) — quick track;
* ![](https://docs.wialon.com/en/hosting/_media/icons/driver.png) — driver information;
* ![](https://docs.wialon.com/en/hosting/_media/icons/trailer.png) — trailer information.

For instance, to sort units by the motion state, use the corresponding button ![](https://docs.wialon.com/en/hosting/_media/icons/state.png). The list is rearranged in such a way that all the moving units appear at the top of the list, and those that are not moving appear at the bottom. To reverse the motion state order of units, click the button again.

The presence or absence of certain columns is adjustable in the [_Monitoring Panel Customizer_](https://docs.wialon.com/en/hosting/user/monitor/icons).

### Tree-like Mode <a id="tree-like_mode"></a>

In this mode, work list units are displayed in groups. Next to the name of the group in parenthesis you can find the number of units included in it. To view the units in the group or the current information on them, expand the group \(_+_ in front of the group name\). Any group unit can be removed from the work list \(though it is not removed from the group itself\).

To add all groups currently not presented in the worklist, click the _Add all available_ button ![](https://docs.wialon.com/en/hosting/_media/icons/add-all.png). At the same time, if the list was empty, the groups are added with all the units included in them. If the group has already been present in the worklist, the list of its units remains unchanged.

When you add units that are not included in any group, they are automatically placed in the _Units outside groups_ ![](https://docs.wialon.com/en/hosting/_media/icons/fake_group.png) group. Such a group cannot be edited, although it has many characteristics typical of an ordinary unit group.

To expand/collapse a unit group \(i.e. show/hide its units\), use the +/- button in front of a group name. To display group units on the map, check a corresponding box. To display a particular unit from a group, expand the group and mark the checkbox with this unit.

If at the end of the list when the group is expanded there is the ellipsis \(…\), this means that not all the group units have been added to the list at the moment. When you hover the cursor over the ellipsis, you can see how many units are not displayed, and add them if necessary.

A tooltip shows the list of all units included in the group.

The following actions can be performed over a unit group from the _Monitoring_ panel:

* ![](https://docs.wialon.com/en/hosting/_media/icons/cmd.png) — [commands](https://docs.wialon.com/en/hosting/user/monitor/cmd) sending;
* ![](https://docs.wialon.com/en/hosting/_media/icons/view.png) or ![](https://docs.wialon.com/en/hosting/_media/icons/edit.png) — [unit group's properties](https://docs.wialon.com/en/hosting/cms/groups/props) viewing/editing.

### Search Tool <a id="search_tool"></a>

There is a convenient tool for finding units and adding them to the work list. To open the unit search dialog, click the _Add to the list_ button ![](https://docs.wialon.com/en/hosting/_media/icons/add-units.png) in the worklist header.

Unit search dialog displays all the available groups \(in square brackets\) and units in alphabetical order. To add units or unit groups, double-click on them. If the simple list mode has been activated, then single units \(one or more\) are added to the work list even if you double-click on a group.

If the tree-like mode has been activated, a group is added to the work list in a collapsed form. To add a unit group with a complete set of units, double-click on a group. To add a unit group with some particular unit, click on this unit then. When you add units that do not belong to any of the groups, they are automatically placed in the _Units outside groups_ group ![](https://docs.wialon.com/en/hosting/_media/icons/fake_group.png).

In order for the added units to be instantly displayed on the map, activate the _Show added units on map_ checkbox in the unit search dialog.

**Search by criteria**

If you have a large number of units/groups, you can use special filters to quickly find the item. The dropdown list contains the following search criteria: name, creator, custom fields, profile fields, phone number, unique ID, device type, access from the user, geofences, sensor, drivers, trailers, passengers, etc.

![](https://docs.wialon.com/en/hosting/_media/monitor/list.png)

Select a search parameter and then type a keyword into the next field. For instance, to find all MANs, select search by name, and in the template field type _man_. All units and groups which names contain the combination of characters _man_ \(both at the beginning and at the end of the name\) will be found and displayed immediately. Comma sign \(,\) can be applied to string together several requests. For example, to find all MANs and all Ivecos, type _**\*man\*,\*iveco\***_.

If you leave the search field empty, all the units that have the selected property \(sensors, ID, etc.\) will be displayed, for example, all units that have a driver assigned to them. Then you can type a driver's name or code to narrow the search.

Most of the search parameters \(except for geofences, drivers, and trailers\) are taken from and can be viewed and changed in the [Unit Properties](https://docs.wialon.com/en/hosting/user/units/units#unit_properties_dialog). When using a search by a sensor, not only the name of a sensor can be entered in the template field, but also a part of its description, parameter type or parameter name.

After the first search is complete, you can continue the search on the second \(third, etc.\) level: search among the results of the previous search. To do this, click _Add to the search list_ ![](https://docs.wialon.com/en/hosting/_media/icons/find-multi.png). The principles of inquiry formation remain the same.

If your search is successful and you want to include the results in the worklist, you can do this with a double click or using the buttons:

* ![](https://docs.wialon.com/en/hosting/_media/icons/list-add.png) — add a search result to the worklist;
* ![](https://docs.wialon.com/en/hosting/_media/icons/list-replace.png) — replace the existing work list with the search results.

### Dynamic Work List <a id="dynamic_work_list"></a>

The work list in the _Monitoring_ panel can be formed dynamically according to the time the last message from a unit was received. Units are removed and added to the list and map automatically. The work list updated every 10 seconds.

The function can be enabled in the [Monitoring panel customizer](https://docs.wialon.com/en/hosting/user/monitor/icons#data_accuracy). Change the _Without filtration_ option to _Monitoring panel_ or _Panel + Map_ and specify the filtration interval in minutes. Then only those units from which data was received during the specified interval will be displayed in the _Monitoring_ panel. If the _Panel + Map_ option is selected, the units are added not only to the worklist but also to the map.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Attention!_  
With this mode enabled, some functions of the system become unavailable or operate differently:

1. Manipulations with the work list \(such as searching, adding, and removing units\) are impossible.
2. The filtration by the time of the last message does not affect the worklist if the [treelike view](https://docs.wialon.com/en/hosting/user/monitor/list#tree_mode) is selected.

