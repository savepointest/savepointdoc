# Working with Messages

Working with messages is query messages, view and filter them, and delete them.

### Requesting Messages from Server <a id="requesting_messages_from_server"></a>

The request is formulated in the [_Messages_](https://docs.wialon.com/en/hosting/user/msg/msg), in the top left corner of the window. Specify the following parameters:

1. Select a unit. The dropdown list contains not all the units available to you, but only the units from the [work list](https://docs.wialon.com/en/hosting/user/monitor/list) of the monitoring panel. In case the worklist is empty \(when the [dynamic work list](https://docs.wialon.com/en/hosting/user/monitor/list#dynamic_work_list) is used or when units were deleted from the work list manually\), the units to which you possess the corresponding rights are displayed. The button in the shape of a spanner located to the right of the dropdown list serves to open the [Unit Properties dialog](https://docs.wialon.com/en/hosting/cms/units/units#unit_properties_dialog). 
2. Specify the time interval to show messages for.![](https://docs.wialon.com/en/hosting/_media/msg/query.png) The principle of interval adjustment is the same as in the reports \(see [Query and View Reports](https://docs.wialon.com/en/hosting/user/reports/query/query)\). The second and fourth steps can be combined if you choose one of the _quick intervals_ \(the buttons _Today_, _Yesterday_, _Week_, and _Month_\).  
3. Select the message type from the dropdown list \(each type is described in detail below\): 
   * [**data messages**](https://docs.wialon.com/en/hosting/user/msg/data),
   * [**SMS messages**](https://docs.wialon.com/en/hosting/user/msg/sms),
   * [**sent commands**](https://docs.wialon.com/en/hosting/user/msg/cmd),
   * [**registered events**](https://docs.wialon.com/en/hosting/user/msg/reg),
   * [**log**](https://docs.wialon.com/en/hosting/user/msg/log).  
4. At the end, press the _Execute_ button. The table will be generated in the right part of the window. To clear the table \(and the map\), press _Clear_.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Note._  
There are alternative ways to query messages:

* from the [Monitoring panel](https://docs.wialon.com/en/hosting/user/monitor/monitor);
* from the table or chart of the [online report](https://docs.wialon.com/en/hosting/user/reports/query/online#transfer_from_tabular_report_to_messages).

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Note that to display the _messages track_ on the map, you should check if the corresponding [layer](https://docs.wialon.com/en/hosting/user/gui/map#visible_layers) is active.

### Viewing Messages <a id="viewing_messages"></a>

Messages of any type are displayed in the form of a table.

If a long time interval is selected, there can be many messages. In this case, they are presented on several pages. Use the navigation panel \(blue arrows\) to move from page to page, or enter the page number manually and press _Enter_ to display a certain page. Apart from that, in the dropdown list, you can set the number of messages to be displayed on one page: 25, 50, 100, 500, 1000.

![](https://docs.wialon.com/en/hosting/_media/msg/table.png)

To change the chronological order of the messages, click on the heading of the _Time_ column. The current sorting direction is shown by the arrows: ![](https://docs.wialon.com/en/hosting/_media/icons/arrow-down.png) — for the direct order; ![](https://docs.wialon.com/en/hosting/_media/icons/arrow-up.png) — for the reverse one. This setting is remembered by the system and used until you change it manually.

The width of the columns can be adjusted. To do this, move the cursor to the border of the column, click the left mouse button and while holding it, drag the border to the desired direction. If you want to expand the table, press the _Set column auto width_ button so that the letter _A_ appears there ![](https://docs.wialon.com/en/hosting/_media/icons/autowidth.gif). In this case, the column width will be set according to contents in the cells. To save the column width when moving through the pages, make the button inactive ![](https://docs.wialon.com/en/hosting/_media/icons/autowidth0.gif). Note that when loading many messages \(500, 1000 per page\), it is better to disable the column auto width because it can considerably slow down the loading process especially if the number of parameters differs from one message to another.

The contents of the table are adjustable. It is possible to hide and display any column. To display the columns, click the ![](https://docs.wialon.com/en/hosting/_media/icons/customizer.png) button in the right corner of the header of the table. Then select the columns you need in the dropdown list. Note that all the columns cannot be hidden simultaneously. If sensors are displayed, each of them has its own column that can be enabled or disabled. By default, only [visible sensors](https://docs.wialon.com/en/hosting/cms/units/sensors/sensors) are displayed \(the rest can be enabled manually\).

### Messages Filter <a id="messages_filter"></a>

To quickly find a necessary message, use a special filter. ![](https://docs.wialon.com/en/hosting/_media/icons/filter.png)[Data messages](https://docs.wialon.com/en/hosting/user/msg/data) \(with parameters displayed as raw data\) can be filtered by parameter names and parameter values, [SMS messages](https://docs.wialon.com/en/hosting/user/msg/sms) and [registered events](https://docs.wialon.com/en/hosting/user/msg/reg) — by message/event text, [sent commands](https://docs.wialon.com/en/hosting/user/msg/cmd) — by values of additional parameters, [log](https://docs.wialon.com/en/hosting/user/msg/log) — by the description of the action. The filter is disabled for data messages with the parameters shown as sensor values.

The rules for setting the filter were given [above](https://docs.wialon.com/en/hosting/user/gui/masks#name_mask). You can use wildcard characters \(\* or ?\) or input your query without them. For example, to find all messages with images enter 'image'. Other available parameters depend on the type of equipment used.

To search for several parameters at once, enter their masks separated by commas. In this case, the results are highlighted in different colors and moved to the beginning of the line. Their order corresponds to the entered masks.

For parameter values, the usage of the _\*_ and _?_ signs is supported if string values are compared. That is, the search can be specified as: _adc? = 0.5 \*_. Only operators _=_ \(equal\) and _&lt;&gt;_ \(not equal\) are used in this case.

In addition, the filter supports the following operations: _=_, _&gt;_, _&lt;_, _&gt;=_, _&lt;=_ _&lt;&gt;_. For instance, a search can be specified as follows:

* param = 3.1415 \(equal\);
* param &gt; 3.14 \(more\);
* param &lt; 3.14 \(less\);
* param &gt;= 3.14 \(more o equal\);
* param &lt;= 3.14 \(less or equal\);
* param &lt;&gt; 3.1415926535 \(not equal\);
* 2.71 &lt; param &lt; 3.15 \(more …, but less …\).

The characters _\*_ and _?_ can be used for parameter names. Therefore, a search can be specified as: _adc? &gt; 0.5_.

The search of input/output values is carried out according to the principle _if any of the values is equal, greater or less_, that is, the query _I / O &lt;2_ will include _I/O = 0/2_ among the results, since there is a value _0_, which is less than _2_.

To apply the filter, press _Enter_ or the _Apply_ button on the right of the filer. After this, messages that contain the requested parameters or text will be displayed in the table. To remove the filter and show all available messages again, clear the query text field and apply the filter again. If the filter is applied, the number of found \(filtered\) messages is displayed on the left.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Attention!_  
The filter only works on the current page with messages. However, when you go through the pages, the filter is applied to each new page automatically.

### Deleting Messages <a id="deleting_messages"></a>

The message can be deleted if you think it is invalid. To delete messages you need to have enough the appropriate access to the unit.

In the last column of the table, mark the messages that should be deleted \(one or more\). Then click the _Delete_ button ![](https://docs.wialon.com/en/hosting/_media/icons/del.png) and confirm your intentions. If the checkbox in the header of the table is ticked, all messages on the current page will be selected.

After the operation, the newly deleted messages still remain in the table but become inactive. The next time when you load messages, the deleted messages will be completely removed from the database.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Note._  
It is impossible to delete the last incoming message, as well as the last message with the position \(valid coordinates\). That is why the delete checkbox for these messages is always dimmed.![](https://docs.wialon.com/en/hosting/lib/exe/indexer.php?id=user%3Amsg%3Amanage&1550650499)

|  |
| :--- |


