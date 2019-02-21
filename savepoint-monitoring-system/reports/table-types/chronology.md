# Chronology

The _Chronology_ report gives information about all the actions and changes in the unit state during the indicated period of time. Unlike most of the tables that are dedicated to a particular state \(parkings, sensors, trips, etc.\), this table combines events of various kinds, which allows to see the complete picture of the movement.

The following types of events can be included in the report \(in the template select the required\):

* Trips
* Parkings
* Stops
* Engine hours
* Fillings
* Thefts
* Events
* Drivers
* Trailers
* Speedings
* Connection loss
* Sensor trigger \(enter one or two masks to indicate the required sensors; note that when you enter a mask, the sensors are firstly filtered by their type \(digital sensors\), and then by name\)

The following columns can be selected to form the table:

* **Type** — trip, parking, stop, engine hours, filling \(or reg. filling\), theft, event \(or violation\), driver, connection loss, sensor.
* **Beginning** — the time taken from the message that precedes the one in which the beginning of the given state was fixed.
* **Initial location** — the location of the unit at the initial moment.
* **End** — the moment when the detected activity finished.
* **Final location** — the location of the unit at the final moment.
* **Duration** — how long the state lasted.
* **Description** — for trips and speedings — mileage, for events and violations — the text of notification, for engine hours — duration, for drivers — driver's binding/unbinding and name, for fuel fillings and thefts — the volume of fuel and sensor name, for sensors — sensor activation/deactivation.
* **Notes** — an empty column for your custom comments.

![](https://docs.wialon.com/en/hosting/_media/tables/chrono.png)

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Note that the system does not calculate the duration of the state for fillings and thefts. Therefore, the beginning and end time for fillings/thefts, as well as the initial and final location coincide in the _Chronology_ table, and the duration column displays zero value.

