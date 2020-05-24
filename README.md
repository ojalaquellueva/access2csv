# Extract Microsoft Access database to CSV (access2csv)

## Overview

Extract a Microsoft Access database file (X.mdb or X.accdb) to one or more CSV files. 

## Requirements
* mdbtools (http://mdbtools.sourceforge.net)

## Usage
* Dumps files to subdirectory "csv" in working directory (whatever directory command is invoked from). Will create directory "csv" if it doesn't exist.

```
access2csv.sh [-i] [-f pathAndAccessFileName] 
```

Option | Details | Required
--- | --- | ---
-i  | Turn on interactive mode (runs in silent mode by default | No
-f  | Path and name MS Access file to extract | Yes

## Known issues
1. Does not handle spatial objects (e.g., shapefiles). As a consequence, tables containing spatial object columns will throw an error. 



