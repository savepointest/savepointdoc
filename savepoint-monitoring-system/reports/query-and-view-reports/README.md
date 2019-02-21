# Query and View Reports

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) It is not possible to generate a report if no templates have been created in advance.

![](https://docs.wialon.com/en/hosting/_media/reports/query.png)

To generate a report, set its parameters \(template, object, time interval\) and click _Execute_. The report runs in the background. Once executed, the message at the bottom of the screen appears and the icon in the _Reports_ tab starts to flash.

**Template**  
Select the required report template from the drop-down list. By default, the one that was created and edited last within the current session is selected. To the right of the list is the button for editing the properties of the selected template ![](https://docs.wialon.com/en/hosting/_media/icons/edit.png)\).

**Object**  
Select the system object that you want to execute the report on \(the current user should have the _Query messages or reports_ [access right](https://docs.wialon.com/en/hosting/cms/rights/rights)\). Depending on the report type specified in the template, you can select a unit, unit group, user, driver, trailer, route, resource, retranslator, group of drivers or trailers, passenger or group of passengers. For the [_Unit group_](https://docs.wialon.com/en/hosting/user/reports/adv/group) report type, you can specify more than one object. Click the _Add object_ button ![](https://docs.wialon.com/en/hosting/_media/icons/add.png) and in the drop-down list, select the required unit or unit group \(shown in square brackets\). If specific objects are [bound](https://docs.wialon.com/en/hosting/user/reports/templ/binding/binding) to the template, only they will be available in the drop-down list. To view/edit the properties of the selected system object, click the button in the form of a wrench to the right of it.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) If the report type is _Unit_, only those objects that are currently in the _Monitoring_ panel [work list](https://docs.wialon.com/en/hosting/user/monitor/list) \(and _not all_ the objects to which you have the required access\) are included in the drop-down list. In case the worklist is empty \(when the [dynamic work list](https://docs.wialon.com/en/hosting/user/monitor/list#dynamic_work_list) is used or when units were deleted from the work list manually\), the units to which you have the _Query messages or reports_ access right will be displayed.

**Interval**  


The report execution interval can be specified in two ways: manually or with the help of one of the available pre-set intervals.

Use buttons _Today_, _Yesterday_, _Week_, _Month_ to select a pre-set interval. If you press one of those four quick buttons, the report launches immediately \(there is no need to press _Execute_\).

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) If the _Week_ interval is selected, the report is executed for the last _full week_, that is, for the previous week from Monday to Sunday. The _Month_ interval works in the same way.

To select the interval manually, there are several options \(the drop-down list to the right of the _Interval_ field\):

* _Specified interval_ For such an interval you can specify the date and time of the beginning and end \(to minutes\). 
* _Starts 'From' until today_ Specify the exact start time. The current time will be automatically set as the end of the interval. 
* _For previous_ The number and the time interval \(minutes/hours/days/weeks/months/years\) for such an interval are indicated below. To select a numerical value for the interval, use the arrow keys or the mouse wheel. Valid values are from 1 to 99. Press and hold the arrows to rewind at an increased speed. When the _Include current_ option is activated, the report is executed not for the last full period, but for the current one.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) When choosing an interval, note that the number of lines of the generated report is limited to 250 000 for optimal system performance. If the number of lines in the final report or the time of its execution exceeds the allowed period, in the parenthesis next to the name of the table appears the mark _cropped_.

There are alternative ways to receive reports in the monitoring system:

* receive reports by e-mail at the specified time \(adjusted through [jobs](https://docs.wialon.com/en/hosting/user/jobs/rep)\);
* receive a report when an event happens \(adjusted through [notifications](https://docs.wialon.com/en/hosting/user/notify/action)\);
* quick report generation from the [monitoring panel](https://docs.wialon.com/en/hosting/user/monitor/icons#quick_report).

