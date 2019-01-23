
**dmodbc** driver is the odbc-compatible driver for DBMaker database management system. It calls into dmapi54.dll on Windows, and use cgo linked to libdmapic.a on Linux. NOTE, dmodbc need not unixODBC or windows ODBC Driver Manager.

e.g.
```
db, err := sql.Open("dmodbc","DSN=DB1;UID=SYSADM;PWD=xxx;");
db.Query(...)
...
```

For more information about DBMaker, please refer to www.dbmaker.com.tw .


