# Sensor Tracing

This table shows sensor values at certain points in time. The table can be exported in MS Excel where you can build any custom charts based on the data provided.

![](https://docs.wialon.com/en/hosting/_media/tables/tracing1.png)The report can include _all messages_ or take a value in a time interval \(like take a value every 10 minutes\). One or the other alternative is chosen when configuring report template. If tracing interval is indicated, the system will search and display sensor value from the message which is the closest to the necessary point in time.

Available columns:

* **Speed** — the speed of the unit from the message from which the value was taken.
* **Coordinates** — the coordinates of the unit from the message.
* **Location** — the location of the unit at the moment of sending the message with the sensor's value.
* **Sensor** — the name of the sensor.
* **Time** — the time of the message from which the value was taken.
* **Value** — the value \(numbers only\).
* **Formatted value** — the value based on the indicated units of measurement or the value of the text sensor.
* **Driver** — the name of the driver \(if available\).
* **Trailer** — the name of the trailer \(if bound\).
* **Notes** — an empty column for custom notes.

![](https://docs.wialon.com/en/hosting/_media/tables/tracing.png)

Activate the appropriate checkbox to get a separate column for each sensor. This option is available only in reports for single units, not for unit groups. If you choose this option, the columns _Values_ or/and _Formatted value_ will be generated for each sensor individually. This allows exporting sensor values to MS Excel and eventually building various charts and diagrams on this basis.

If you activate the options _Each sensor in separate column_ and _Skip invalid values_ simultaneously, only the lines that have at least one sensor's value is shown in the generated report. The lines without any sensor's value are not shown. The name of a column containing formatted values is marked by a special symbol \(\*\). Formatted value fields may contain textual information \(in brackets\) indicated for [value intervals](https://docs.wialon.com/en/hosting/cms/units/sensors/props#intervals_and_colors).

![](https://docs.wialon.com/en/hosting/_media/tables/tracing2.png)

In addition, you can choose a driver/trailer and geofences/units to be controlled \(see [intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) for details\).

### Invalid Values <a id="invalid_values"></a>

If a received value is out of range \(the bounds are indicated in sensor properties\), then a dash \(« —– »\) is displayed in the lines with the values of the sensor. To exclude such rows, check the _Skip invalid values_ option in the report template.

The cases when a sensor sends text values \(as opposed to numeric\) or no values at all are also considered _invalid_.

In order for the text parameters to be recognized as valid and displayed in the _Formatted value_ column, activate the [_Text parameters_](https://docs.wialon.com/en/hosting/cms/units/sensors/props#additional_properties) option when creating a custom sensor.

