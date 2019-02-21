# Maps

Maps settings are adjusted in the [User Settings dialog](https://docs.wialon.com/en/hosting/user/set/set) on the _Maps_ tab.

![](https://docs.wialon.com/en/hosting/_media/set/set3.png)

**Map source**  
Here you can enable or disable certain layers of maps by checking the appropriate boxes. Changes are applied after clicking _OK_ and refreshing the page. To select a different map as a base layer, choose it in the [maps menu](https://docs.wialon.com/en/hosting/user/gui/map#map_source).

The following maps can be used in Wialon: Google, Bing, Kosmosnimki, 2GIS, WikiMapia, Visicom, Yandex, HERE, Regio, Luxena, what3words, MyIndia, ArcGIS, GoMap.az, Mapbox, OpenStreetMap, and additional layers OpenSeaMap, OpenWeatherMap, AerisWeather.Besides, Gurtam Maps are available by default.

Some maps go in blocks. For example, when you enable Google Maps, several map layouts appear on the menu at once: Google Streets, Google Physical, Google Satellite, Google Hybrid, Google Map Maker, Google Map Maker Hybrid, and Google Street View for [tracking on mini map](https://docs.wialon.com/en/hosting/user/monitor/minimap#mini_map_modes). Moreover, if the additional layers are available \(for example, traffic layer, maritime navigation\), they can be visually displayed on top of any chosen map.

If there is no option to activate a map type, address your request to [Gurtam Help System](http://support.gurtam.com/).  
![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Use of cartographic services is stipulated by the procedures established by the author or by another right holder of such services. When choosing a cartographic service you confirm that you acknowledge and accept the full responsibility for its possible misuse.

**Geodata source**  
In this section, you can select the source of address information used in the _Monitoring_ panel, in the tooltips of units and tracks, in the _Messages_ panel, while creating geofences and routes. Possible sources of geodata are Gurtam, Google, Visicom, Yandex, Mapbox, HERE, Luxena, what3words, ArcGIS. Only the maps that are activated in the site's properties are displayed in the list of available.

If _Google \(standard\)_ or _Yandex \(standard\) — geocoding_ [service](https://docs.wialon.com/en/hosting/cms/accounts/services) is activated for the account and Google or Yandex is selected as the geodata source, the information about the location of the unit is shown in the reports in accordance with the format of the maps provider.

For the Gurtam geodata source, it is possible to activate the _MGRS coordinates_ option if the user has the _MGRS_ [service](https://docs.wialon.com/en/hosting/cms/accounts/services).

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) If a geodata source other than Gurtam is chosen, the _Address format_ block becomes unavailable.

**Address format**  
Here you can specify the format for displaying address information in tooltips, tools, messages, and other places. Choose which of standard address components should be displayed: country, region, city, street, and house \(at least one of these items should be selected\). For example, if your units move mainly within the same city or town you can omit the country, region, and city and leave only the street name and house number in addresses. Address components can be put in any order. To change this order, drag components up and down using the arrow-shaped buttons. This format affects addresses mainly in cities/towns/villages.

This format is especially relevant if the units are moving around the city. For addresses outside the city \(near roads\), the following two settings are important:

* _Max distance from unit_ determines that if the unit is on the road or close to it and there is a city/town/village at a specified distance, the address is displayed as the name of the road and the distance to that city \(if several cities are found, then to the nearest one\).
* _Min city radius_ determines that if at a distance specified as _Max distance from unit_, no settlement is found, then the address is bound to some other city. The radius of the city that can get into the address information can be specified in this parameter. It may be necessary, for example, if only large cities should appear in addresses.

**Format of coordinates**  
The coordinates of the cursor shown in the lower right corner of the [map](https://docs.wialon.com/en/hosting/user/gui/map) can be either in degrees or in degrees and minutes. This option _only_ influences the cursor's position format.

For the _Map source_ and _Format of coordinates_ blocks there is a possibility to check all the boxes at once. To do so, hold the _Ctrl_ key and check any box of the corresponding block.

