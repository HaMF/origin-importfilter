# origin-importfilter

Add ("install") the OriginLab OriginPro import filters to your Origin installation by copying the _.oif_ files to the Filters subfolder of your origin user files folder. This is usually something like _"C:\Users\YOUR.USERNAME\Documents\OriginLab\2015\UserFiles\Filters\User Files"_. You can find more information on the Origin website http://www.originlab.de/doc/Origin-Help/UserFilesFolder.

If you have comments or questions on any of the filters or find and fix a bug, please let me know by filling an issue on github.

Origin, OriginLab, OriginPro are quite probably protected trade marks of OriginLab Corporation. Don't sue me, please. 

The import filters are licensed under _the Unlicense_ so go ahead, modify and share them. Return the favor, please.


## SQUID_RSO_ASCII.oif

This filter is intended to ease the import of M-H and M-T curves produced by a ??? SQUID magnetometer. The filter imports just the _Temperature_, _Field_ and _Long Moment_ rows from the measurement files and converts all data into SI units.

  * Associates with __*.rso.dat__ and __*.dc.dat__ files 
  * Imports the INFO variables _Temperature_, _Name_, _Weight_, _Area_, _Length_, _Shape_ and _Comment_ from the file
  * Adds a _volume_ user parameter to the worksheet that is used to volume normalize the data
  * Converts all units into SI
  * Fixes column names and units
