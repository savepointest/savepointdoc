# Logs

## Logs <a id="logs"></a>

The _Log_ table can be generated for units, unit groups, users, resources, retranslators or routes. The log contains records about changes made in the properties of the object or its contents. To view the log of a unit, in addition to the _Query messages or reports_ access right, you need the _Manage log_ access.

* **Time** — the date and time when the change was saved.
* **User** — the name of the user who made the change. You can specify the username mask in the report template so that only the changes made by a certain user will be displayed.
* **Item name** — the name of the item. ![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) This column is used only in the user report.
* **Item type** — a unit, unit group, user, resource, retranslator or route.
* **Action** — the description of the change made.
* **Host** — the address of the computer from which the user made the changes, or _job_ or _notification_ if the change was made as a result of automatic system actions.
* **Notes** — an empty column for custom notes.

Log example for a resource:

![](https://docs.wialon.com/en/hosting/_media/tables/log1.png)

The user log presents two types of information: changes made by the user and changes made by other users in regards to this user as a system object. There is also the _Item name_ column available in the log:

![](https://docs.wialon.com/en/hosting/_media/tables/log2.png)

_Group itself_ is an additional parameter for the log of a unit group. If this checkbox is disabled, the log shows the changes made to units in the group \(the [detalization](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/settings#detalization) is required in this case\):

![](https://docs.wialon.com/en/hosting/_media/tables/log4.png)

If the _Group itself_ option is enabled, the log shows the changes made to the unit group as a system object:

![](https://docs.wialon.com/en/hosting/_media/tables/log3.png)

