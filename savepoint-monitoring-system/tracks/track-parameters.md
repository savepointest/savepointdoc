# Track Parameters

After you have built a [track](https://docs.wialon.com/en/hosting/user/tracks/tracks), it is impossible to change its parameters \(time, unit, color, annotations\). In case of error, delete the incorrect track and create a new one.

### Track Color <a id="track_color"></a>

There are four mutually exclusive color settings for the track: _By trips_, _By Speed_, _By sensor_ and _Single_. One of these settings, except the first one, can be initially set on the _Advanced_ tab of the unit settings. If the setting is not specified, or a single color of the track is selected, the _By trips_ option is selected by default in the track panel.

For a _Single_ track, you can choose a color in the palette every time you build a track, or, if the color is not specified, for each new track the color will be selected automatically from the color range \(it is selected circle-wise\). The color is selected in the same manner if the _Single_ setting is applied to the unit, and another color is chosen manually from the palette.

### Track Line Thickness <a id="track_line_thickness"></a>

Indicate the **thickness** of the track in pixels \(from 1 to 15\). A track can be represented as unconnected points \(the points from which the messages were received\). If you need this option, select the _Points only_ option.

![](https://docs.wialon.com/en/hosting/_media/tracks/points.png)

### Markers <a id="markers"></a>

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Markers can be used only if you have access to reports.

You can enable markers to highlight the places of significant events on the track. The choice of possible markers is the same as in reports:

* ![](https://docs.wialon.com/en/hosting/_media/tracks/markers.png)![](https://docs.wialon.com/en/hosting/_media/icons/theft.png) fuel thefts,
* ![](https://docs.wialon.com/en/hosting/_media/icons/speeding.png) speeding,
* ![](https://docs.wialon.com/en/hosting/_media/icons/filling.png) fuel fillings,
* ![](https://docs.wialon.com/en/hosting/_media/icons/event.png) events \(if a violation took place, the marker is red\),
* ![](https://docs.wialon.com/en/hosting/_media/icons/pics.png) pictures from messages,
* ![](https://docs.wialon.com/en/hosting/_media/icons/vid.png) video from messages,
* ![](https://docs.wialon.com/en/hosting/_media/icons/parking.png) parking places,
* ![](https://docs.wialon.com/en/hosting/_media/icons/stop.png) short stops,
* ![](https://docs.wialon.com/en/hosting/_media/icons/initial.png) initial position,
* ![](https://docs.wialon.com/en/hosting/_media/icons/final.png) final position.

Select the markers before building a track. To activate a marker, just click on its icon to make it colorful. If at least one kind of marker is selected, additional marker options can be applied:

* [![](https://docs.wialon.com/en/hosting/_media/icons/numbering.png)](https://docs.wialon.com/en/hosting/_detail/icons/numbering.png?id=user%3Atracks%3Aparams) numbering,
* [![](https://docs.wialon.com/en/hosting/_media/icons/groupping.png)](https://docs.wialon.com/en/hosting/_detail/icons/groupping.png?id=user%3Atracks%3Aparams) grouping.

Markers in tracks are drawn and used on the same principles as [in reports](https://docs.wialon.com/en/hosting/user/reports/map/markers#markers_on_map).

### Annotations <a id="annotations"></a>

Indicate whether you want **annotations** to be displayed. Annotations are hints which are attached to each point of the track to show the date and time when the message was received, as well as the speed of the movement of the unit at that time. Annotations are rather informative but they make the visual perception of the track more complicated. That is why sometimes it is reasonable to switch them off. Full information about any point of the track can be obtained from the tooltip that appears when you hover the cursor over a point. ![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) The system of measures in the annotations depends on the settings of the current user, not on the settings of the unit.

![](https://docs.wialon.com/en/hosting/_media/tracks/annotations.png)

### Trip Detector <a id="trip_detector"></a>

Trip detector checkbox affects the distance value and track visualization. For example, in the places of stops and parkings not a conglomeration of points will be displayed, but just one, and the mileage will include only the intervals detected as trips.

Also, this option allows you to view the trips made within the track. Press the _+_ to the left of the track to expand the list of its trips. Click on the required trip to center the map on it. Note that the Track Player tool works for the whole track. The trip detector is set up in [Unit Properties =&gt; Trip Detector](https://docs.wialon.com/en/hosting/cms/units/trip).

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) The mileage in tracks can sometimes differ from the mileage in reports \(if there are invalid messages within the interval\). In such cases, more accurate mileage is provided in reports.

