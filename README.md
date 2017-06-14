odbc driver written in go. Implements database driver interface as used by standard database/sql package. It calls into odbc dll on Windows, and uses cgo (unixODBC) everywhere else.

To get started using odbc, have a look at the [wiki](../../wiki) pages.

**dmodbc** driver is the odbc-compatible driver for DBMaker database management system. It calls into dmapi54.dll on Windows, and use cgo linked to libdmapic.a on Linux. NOTE, dmodbc need not unixODBC or windows ODBC Driver Manager.

e.g.
```
db, err := sql.Open("dmodbc","DSN=DB1;UID=SYSADM;PWD=xxx;");
db.Query(...)
...
```

For more information about DBMaker, please refer to www.dbmaker.com.tw .
