# Events

All events registered by the system \(including [violations](https://docs.wialon.com/en/hosting/user/reports/tables/violations)\) can be shown in the report on events.

There are different ways to add events to the unit history:

1. Using [notifications](https://docs.wialon.com/en/hosting/user/notify/action#register_event_for_unit) if the method of delivery is _Register event for unit_.
2. Manually using the [events registrar](https://docs.wialon.com/en/hosting/user/monitor/reg).
3. Save, reset, change the values of [counters](https://docs.wialon.com/en/hosting/cms/units/counters) with the help of the corresponding [jobs](https://docs.wialon.com/en/hosting/user/jobs/counters) or [notifications](https://docs.wialon.com/en/hosting/user/notify/action#set_counter_value).
4. Manually using custom events registered from the [online notifications](https://docs.wialon.com/en/hosting/user/notify/online) window.
5. Automatically, upon completing a [route](https://docs.wialon.com/en/hosting/user/routes/routes) by the unit.

To get a report on specific events, in the report template you can additionally specify a **mask**. Based on this mask, only those events whose text \(description\) corresponds to the specified parameters \(for instance, the [notification text](https://docs.wialon.com/en/hosting/user/notify/text)\) will be selected for the report generation.

The following columns can be displayed in this report:

* **Event time** — the time when the event happened.
* **Time received** — the time when the server received the data.
* **Event text** — the text that was specified when creating a notification or when registering an event manually.
* **Location** — the location of the unit at the moment of the event. If the event is registered manually, the unit's location is detected on the basis of messages received upon event registration. The same is true for the events registered by storing counters' values in the unit properties.
* **Driver** — the name of the [driver](https://docs.wialon.com/en/hosting/user/drivers/drivers) \(if identified\).
* **Count** — the count of events.
* **Notification text** — the text available upon registering an event from an online notifications window.
* **Notes** — an empty column for your custom comments.

![](https://docs.wialon.com/en/hosting/_media/tables/events.png)

In addition, you can use special [markers](https://docs.wialon.com/en/hosting/user/reports/templ/settings/map#markers) for this report: a green flag stands for an event, a red flag — for a violation. In the tooltip, you can find the detailed information. The markers of events and violations are enabled with the help of additional settings in the report template _Event markers_.

![](https://docs.wialon.com/en/hosting/_media/tables/markers-events.png)

