odbc driver written in go. Implements database driver interface as used by standard database/sql package. It calls into odbc dll on Windows, and uses cgo (unixODBC) everywhere else.

To get started using odbc, have a look at the [wiki](../../wiki) pages.

**dmodbc** driver is the odbc-compatible driver for DBMaker database management system. It calls into dmapi54.dll on Windows, and use cgo linked to libdmapic.a on Linux.

For more information about DBMaker, please refer to [DBMaker web site](www.dbmaker.com.cn).
