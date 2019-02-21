# Export/Import Messages

Messages can be imported and exported. It concerns only the messages of the first type, that is, [data messages](https://docs.wialon.com/en/hosting/user/msg/data).

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Attention!_  
The size limit for the imported file/archive is 64 MB, which, in the case of the archive, is approximately 3.5 million messages.

### Export <a id="export"></a>

To export messages to a file, open the _Export and Import Messages_ tab in the lower left section of the window. Select the destination format and click _Export_. Depending on your browser configuration settings, you will be offered to open or save the file. The file with exported messages can be compressed. For this, leave the checkbox _Compress file_ marked.

![  ](https://docs.wialon.com/en/hosting/_media/msg/exp_imp.png)

The supported export formats are:

* OziExplorer track\(.plt\) — data format of the Ozi Explorer program that stores a track as a list of coordinates of the track points.
* NMEA messages \(.txt\) — a text file of the National Marine Electronics Association. This text protocol is used for marine navigation equipment. ![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Attention!_ Parameters \(sensors\) are not stored when exporting to this format.
* Google Earth \(.kml\) — an XML-based format used in the Google Earth program to transmit three-dimensional geospatial data.
* Wialon messages \(.wln\) — a format to be used with the Wialon software.
* Wialon binary messages \(.wlb\) — a binary format to be used with Wialon software.

### Import <a id="import"></a>

Saved files on the disk containing messages from the unit can be imported into the units you create. To import messages, select the _Export and Import Messages_ tab in the left section of the window.

The supported import formats are:

* Raw GPRMC navigator logs in the format defined by NMEA 0183 specification — searched in files with the extension .txt or .log.
* Wialon messages — search in files with the extension .wln.
* Wialon binary messages — search in files with the extension .wlb.

Click on the empty field, specify the file to import the messages from, and click _Upload_.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Hint._  
To speed up and simplify the process, first compress the files with ZIP or GZIP utilities. When uploading is completed, the files will be unpacked and processed on the server. This process can be traced in the log.

