# Trips

This kind of report shows the intervals of movement with the indication of time, location, and other parameters such as speed, mileage, fuel, and many others. The intervals of movement \(trips\) are detected according to the parameters set in the [Trip Detection](https://docs.wialon.com/en/hosting/cms/units/trip) and adjusted for each unit individually.

The following columns can be included in this kind of report:

* **Beginning** — the date and time when the trip began.
* **Initial location** — the address where the device was at the beginning of the trip.
* **Initial coordinates** — the geographical coordinates of the location of the unit at the beginning of the trip \(in decimal degrees\).
* **End** — the date and time when the trip ended.
* **Final location** — the address where the device was at the end of the trip.
* **Final coordinates** — the geographical coordinates of the location of the unit at the end of the trip \(in decimal degrees\).
* **Driver** — the name of the [driver](https://docs.wialon.com/en/hosting/user/drivers/drivers) \(if identified\).
* **Trailer** — the name of the [trailer](https://docs.wialon.com/en/hosting/user/trailers/trailers) \(if bound\).
* **Passengers count** — the number of [passengers](https://docs.wialon.com/en/hosting/user/passengers/passengers) transported within a trip.
* **Duration** — the time interval of the trip.
* **Total time** — the time from the beginning of the first trip to the end of the last trip.
* **Off-time** — the period of time passed from the end of the previous trip to the beginning of the current one \(defined beginning from the second trip\).
* **Following off-time** — the period of time passed from the end of the current trip to the beginning of the next one.
* **Engine hours** — the time of the operation of engine hours during the trip.
* **Mileage** — the distance traveled during the whole trip.
* **Mileage \(adjusted\)** — the mileage taking a coefficient set in unit properties \(the _Advanced_ tab\) into account.
* **Urban mileage** — the distance traveled in the urban area.
* **Suburban mileage** — the distance traveled in the suburban area \(i.e. at high speed\). The urban/suburban speed line is indicated in the[Unit Properties —&gt; Advanced](https://docs.wialon.com/en/hosting/cms/units/adv) \(the _Urban speed limit_ setting\).
* **Initial mileage** — the mileage sensor value at the beginning of the trip. If the mileage parameter was not saved throughout the reported period, the mileage is counted from 0.
* **Final mileage** — the mileage sensor value at the end of the trip.
* **Toll roads mileage** — the distance that the unit passed during the trip on the roads on which the Plato system is used.
* **Toll roads cost** — a sum of money \(in RUB\) for the toll roads mileage calculated on the basis of the covered distance and the Platon tariff.
* **Avg speed** — the average speed within the trip.
* **Max speed** — the maximum speed registered within the interval.
* **Trips count** — the number of completed trips.
* **Counter** — the counter sensor value.
* **Initial counter** — the counter value at the beginning of the trip.
* **Final counter** — the counter value at the end of the trip.
* **Avg engine revs** — the average rate of engine revolutions.
* **Max engine revs** — the maximum rate of engine revolutions.
* **Avg temperature** — the average temperature value registered in a trip.
* **Min temperature** — the minimum temperature value registered in a trip.
* **Max temperature** — the maximum temperature value registered in a trip.
* **Initial temperature** — the temperature value at the beginning of a trip.
* **Final temperature** — the temperature value at the end of a trip.
* **Status** — the unit status registered during the current trip \(if there are several, the first one is displayed\).
* **Cargo weight** — the weight of a cargo transported within a trip.
* **Messages count** — the number of messages that formed the trip.
* **Consumed** — the volume of consumed fuel detected by any sort of fuel sensor. If several such sensors are available, their values sum up.
* **Consumed by ImpFCS/AbsFCS/InsFCS/FLS/math/rates** — the volume of consumed fuel detected by a fuel sensor \(such as impulse/absolute/instant fuel consumption sensor, fuel level sensor\) or calculated by math or rates. More information about fuel in reports can be found [here](https://docs.wialon.com/en/hosting/user/reports/dat/dat#fuel_in_reports).
* **Rates deviation by ImpFCS/AbsFCS/InsFCS/FLS** — the difference between consumed fuel detected by a sensor and consumption rates. If a number in this cell is negative, it means the detected consumption does not exceed the indicated rates.
* **Avg consumption** — the average fuel consumption by any sort of fuel sensor. If several such sensors are available, their values sum up.
* **Avg consumption by ImpFCS/AbsFCS/InsFCS/FLS/math/rates** — the average fuel consumption during the trip detected by one of the methods mentioned above.
* **Avg consumption in idle run by …** — the average fuel consumption during the idle run.
* **Avg mileage per unit of fuel by …** — the average fuel consumption \(per one liter/gallon\) detected by one of the methods mentioned above.
* **Initial fuel level** — the fuel level at the beginning of the trip.
* **Final fuel level** — the fuel level at the end of the trip.
* **Max fuel level** — the maximum fuel level during the trip.
* **Min fuel level** — the minimum fuel level during the trip.
* **Penalties** — the penalties calculated for the adjusted [_Eco Driving_](https://docs.wialon.com/en/hosting/cms/units/eco) criteria.
* **Rank** — the received penalty points converted into a grade using a 6-point scoring system.
* **Notes** — an empty column for your custom comments.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Attention!_  
Availability of the _Toll roads mileage_ and _Toll roads cost_ columns is stipulated by a special service. Contact your service provider if you would like to use this functionality.

![](https://docs.wialon.com/en/hosting/_media/tables/trips.png)

See [Data in Reports](https://docs.wialon.com/en/hosting/user/reports/dat/dat) to find more about formatting time, mileage, fuel, etc.

Also, the [intervals filtration](https://docs.wialon.com/en/hosting/user/reports/templ/contents/tables/filtration) by duration, mileage, engine hours, speed range, stops, sensors, driver, fuel fillings, fuel thefts, and geofences/units can be applied to this table.

The tracks of the trips can be displayed on the map. To make use of this feature, in the report template, select the [options](https://docs.wialon.com/en/hosting/user/reports/templ/settings/map#tracks_in_reports) connected with the rendering of tracks on the map.  


