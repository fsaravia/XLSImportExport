This is a small library to handle MS Excel files.

It relies on Apache POI library (http://poi.apache.org/)

Usage for reading from file:

```java
XLSImport importer = new XLSImport("/path/to/file");
Sheet selectedSheet = importer.selectSheet(0);
Row selectedRow = importer.selectRow(0);
//Obtain values
String string = importer.getString(0);
double double = importer.getDouble(0);
boolean boolean = importer.getBoolean(0);
Date date = importer.getDate(0);
Object object = importer.getValue(0);//Just call getValue if you don't need to know the type
```
