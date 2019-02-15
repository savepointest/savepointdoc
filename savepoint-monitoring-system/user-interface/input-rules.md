# Input Rules

All fields for editing are checked for correctness of the input data. If the data is incorrect, the field is highlighted in red.

#### Incorrect entries are: <a id="incorrect_entries_are"></a>

* Not enough characters in the name or a phone number. The names of monitoring units, unit groups and users must consist of at least 4 characters. Other objects like places, geofences, drivers, report templates, etc. can have names from one character in length.
* The Excessive number of characters \(more than 50\) in names of monitoring units, unit groups, and users.
* Letters in numeric fields \(phone numbers, sensor values, radius, fuel consumption, and trip detector settings, etc.\)
* Forbidden characters:
  * double quotation marks **''**
  * curly brackets **{** **}**
  * the backslash **\**
* Partly forbidden characters:
  * **spaces** are not allowed at the beginning and at the end of editable fields \(however, they are allowed at the middle\);
  * **comma** cannot be used in numeric fields as a separator \(to introduce fractional numbers use a period as a separator\).
  * in report templates \(column names, table titles, and statistics fields\) you cannot use a comma, colon, or **&** symbol.

Using angle brackets \('&gt;' and '&lt;'\) is allowed but not recommended as, in some cases, they are automatically replaced with '&gt;' and '&lt;'.

If any entry in a dialog is not valid, it is impossible to save changes or create an object, because the _OK_ button becomes inactive. There can also be the _Incorrect entry_ alert when trying to save incorrect data.

#### Phone numbers and e-mail addresses <a id="phone_numbers_and_e-mail_addresses"></a>

**Phone numbers** must be entered in an [international format](http://en.wikipedia.org/wiki/Telephone_numbering_plan#Standards) and contain all the necessary codes \(country code, communication statement or city code, and then the phone number itself\). Brackets, spaces and hyphens are not allowed. The only symbol that can be used for entering phone numbers is **plus**\(+\) which, if necessary, is typed at the beginning of the number. Examples: _+19176726154, +15551234567_.

**E-mail addresses** must be in the format _username — the 'at' sign \(@\) — domain name_. E-mails can contain letters of Latin alphabet, as well as dots \(.\), hyphens \(-\) and underscores \(\_\). Example: _username@domain.net_.![](https://docs.wialon.com/en/hosting/lib/exe/indexer.php?id=user%3Agui%3Ainput&1550214029)

|  |
| :--- |


