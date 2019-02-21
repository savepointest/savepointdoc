# Address

Many reports use the following address information: initial or final location of the unit during the trip, the place of a fuel filling or theft, the position during parking or stop, location where the connection was lost, message received, event registered, etc. Both the map selected as [geodata source](https://docs.wialon.com/en/hosting/user/set/maps) and the created geofences can be used as the source of the address information.

![](https://docs.wialon.com/en/hosting/_media/reports/address.png)

### Addresses from Map <a id="addresses_from_map"></a>

Specify the format for displaying the address information. To do this, select which elements of the address should be displayed \(country, region, city, street, and house are available\), and arrange them in the preferred order, pulling up or down the double arrow ![](https://docs.wialon.com/en/hosting/_media/icons/drag.png). If none of the five items is selected, the coordinates are displayed.

This format is especially relevant if the units are moving around the city. For addresses outside the city \(near roads\), the following two settings are important:

**Min radius**  
If at a distance indicated as the maximum distance from the unit, no city is found, the address is bound to another city. The radius of the city, which can get into the address information, is indicated in this parameter. It may be required, for example, that only large cities appear in addresses.

**Max distance from unit**  
If the unit is on the road and at a specified distance from it there is a city, the name of the road and the distance to this city get to its address.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Note_.  
If you find inaccurate address information in the reports, you can update the map of your region/city. To do this, send a new map of your region in the [proper format](https://docs.wialon.com/en/hosting/cms/gis/gis) to the technical support.

### Addresses from Geofences <a id="addresses_from_geofences"></a>

Sometimes maps may not contain the exact addresses in certain regions. In such cases, you can use [geofences](https://docs.wialon.com/en/hosting/user/geo/geo) as addresses. Besides, you can specify your own names for certain addresses.

If the _Use geofences for addresses_ option is activated, additional parameters become available. In particular, you can choose to display geofence's description alongside with its name \(the _Add geofence description to address_ option\). To see the distance at which the unit is away from the geofence, specify the **radius of geofence search**. The maximum allowable value is 100 km or miles \(depending on the selected system of measures\).

The range of geofences used as addresses is adjustable. By default, all geofences that belong to the same resource as the report template are used. However, geofences from _all_ available resources can be used if necessary. Alternatively, to narrow this range, you can specify a particular group of geofences to be used \(it should be created in the same resource as the report template itself\). Select the option in the _Specify geofences_ drop-down list \(groups of geofences are displayed in square brackets\).

If the geofences are selected as addresses, but the location of the unit is not found, the address information is taken from the map and is formed according to the parameters specified above. When two geofences overlap each other, a smaller one is selected for the address.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) To work with these options, activate the [_Geofences_](https://docs.wialon.com/en/hosting/cms/accounts/services) service in the account properties.

