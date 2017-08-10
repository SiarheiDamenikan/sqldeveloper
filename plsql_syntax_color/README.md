# Colour scheme for Oracle SQL Developer #

This is my colour scheme for Oracle SQL Developer. Tested on Oracle SQL Developer v4.15, v4.20, v17.2

![](screenshots/sqldev_1.png)

## Installation ##

Unfortunately Oracle doesn't make it easy to import a new colour scheme into SQL Developer, thus a little bit of hacking is required.

- Close SQL Developer. This is important. If you modify the scheme file while SQL Developer is open, your changes won't be saved.

- Locate file `dtcache.xml` in the SQL Developer's settings directory. On my system it is located in directory `c:\Users\Siarhei_Damenikan\AppData\Roaming\SQL Developer\system17.2.0.188.1159\o.ide.13.0.0.1.42.170225.201\`

- Locate `<schemeMap>` tag inside dtcache.xml file. Insert the content of [`color_scheme.xml`](https://github.com/SiarheiDamenikan/sqldeveloper/blob/master/plsql_syntax_color/color_scheme.xml) file inside `<schemeMap>` alongside the other colour schemes. Be careful not to break the XML.

![Insert the contents of color_scheme.xml after opening schemeMap tag](screenshots/insert_here.png)

- Launch SQL Developer. Navigate to menu Tools->Preferences, then select item Code Editor -> PL/SQL Syntax Colours in the left pane.

- Select "Damenikan" in the drop down list "Scheme" on the top of panel PL/SQL Syntax Color.

![](screenshots/sqldev_2.png)
