# Export Report to File

To get a report as a file, press the _Export to file_ button ![](https://docs.wialon.com/en/hosting/_media/icons/export1.png).

Specify the desirable file format or several formats at once. Supported formats are HTML, PDF, Еxcel, XML, CSV. For some formats, you may need to specify additional export options.

![](https://docs.wialon.com/en/hosting/_media/reports/export.png)

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Reports in the form of files can also be received by e-mail automatically – using [jobs](https://docs.wialon.com/en/hosting/user/jobs/rep) and [notifications](https://docs.wialon.com/en/hosting/user/notify/action).

### Export Parameters <a id="export_parameters"></a>

The report file can be assigned any name by entering it manually in the _File name_ field of the export dialog. If the name is not specified, the file is formed with the default name.

Specify if the file should be archived. Archivation is compulsory for the files of HTML format, as well as for the files with the total size of more than 20 MBregardless of the state of the _Compress report files_ check box.

The _Split chart by:_ option allows to receive, depending on your selection, a separate chart for each day or week of the reporting period.

Indicate whether it is necessary to attach the map to the exported report. Graphical objects \(such as map, chart\) can be exported only into HTML or PDF files. Note that the map will be attached to the file only if any graphical elements \(such as [tracks, markers, geofences, etc.](https://docs.wialon.com/en/hosting/user/reports/templ/settings/map)\) are selected in the [report template](https://docs.wialon.com/en/hosting/user/reports/templ/templ). By default, the map is scaled in order fot the track/markers/last unit position to be seen on it. If these elements are not shown on the map, the map is not attached. If the _Squeeze in all graphics_ checkbox is marked, the map is scaled in such a way that geofences are shown on the map along with the above-mentioned elements. Only Gurtam Maps can be attached to the report. Furthermore, the map layer can be hidden \(using the _Hide cartographic basis_ option\) — in this case, tracks and markers are shown on the blank background.

The function of using a link to display the location \(if the coordinates are available\) is supported for the files exported in PDF or Excel. It works as follows: open the exported report \(PDF/Excel\), place the cursor on the corresponding field of a report, for example, the beginning/end time or address information from the unit \(the cursor pointer changes to _hand_\) and click on the link. Google Maps cartographic service will be opened in your browser, where the marker indicates the location. If there is no need to show the location, you can disable links to Google Maps in PDF and Excel files by marking the corresponding checkbox in the export parameters.

In order to disable the function described above, use the _Disable links to Google Maps in PDF and Excel files_ option.

More parameters can be adjusted for some file formats. Those additional parameters are described below.

Usually you export to a file a report that is already in the browser. However, you can also generate a new one according to the parameters set in the left panel. In this case, you should check the _Generate report_ option.

Press _OK_. Depending on the browser settings, you will be offered to open a file or save it.

### Report Formats <a id="report_formats"></a>

#### HTML <a id="html"></a>

Choose the HTML format to receive a report in the form of a web page, which can be opened in any Internet browser installed on the computer.

![](https://docs.wialon.com/en/hosting/_media/reports/export-html.png)

#### PDF <a id="pdf"></a>

PDF is a widely known file format. To view these files Adobe Acrobat Reader is used \(for Windows OS only\). This type of file is well suited for printing.

You can additionally specify the page orientation \(landscape or portrait\) and format \(A4 or A3\) when exporting a PDF-file.

For reports with a large number of columns, the _Page width_ option may also be appropriate. The standard page width is _fixed_ which means it depends on the selected page format and orientation. However, if the table is too wide and does not fit the specified page width, this table will not be exported \(only the heading will be displayed\). In such cases, you can select _automatic_ page width and the width of the page will correspond to the largest row in the table. If _Auto, compact_ is selected, the cell width is equal to the length of the largest word in it. If _Auto, no wrap_ is selected, the cell width is equal to the largest phrase in it \(no line breaks are applied\).

Note that if the automatic page width is selected, the page format and orientation become relative — they define only the height of the page, not the width.

![](https://docs.wialon.com/en/hosting/_media/reports/export-pdf.png)

#### Еxcel <a id="excel"></a>

Excel \(.xslx\) is a popular product from the Microsoft Office suite. Here the data is presented in the form of spreadsheets. The report is divided into several tab pages. The data is automatically stored in tables and is suitable for subsequent processing by the tools of this program.

![](https://docs.wialon.com/en/hosting/_media/reports/export-xls.png)

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) _Note_.  
When exporting a report to PDF, HTML, Excel the **alignment** is used. The columns with text \(names of sensors, geofences, drivers, users, SMS and notification text, location addresses, etc.\) are aligned to the left. The columns with numeric data \(time, duration, speed, mileage, fuel, payments, count, etc.\) are aligned to the right.

#### XML <a id="xml"></a>

XML represents information in the form of a text file used for storing structured data \(instead of existing database files\), for exchanging information between programs, and for creating more specialized markup languages \(such as XHTML\) on its basis.

![](https://docs.wialon.com/en/hosting/_media/reports/export-xml.png)

#### CSV <a id="csv"></a>

CSV is a text file format used for the presentation of tabular data. Each line of this file corresponds to one line of the table, and the columns are separated from each other by a special delimiter character - a comma \(,\) or a semicolon \(;\). Each table is saved in a separate file.

To export to a CSV file, you should additionally choose the encoding \(utf8, cp1251\) and a delimiter \(comma or semicolon\). Depending on the state of the _Show column headers_ checkbox, the file will start with the header line or immediately with the data.

![](https://docs.wialon.com/en/hosting/_media/reports/export-csv.png)

