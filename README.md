# docker-image-mssql-tools
A docker image for mssql-tools on Linux

See more @ https://hub.docker.com/r/beardedfoo/mssql-tools/

Use this image:
```bash
$ docker run beardedfoo/mssql-tools sqlcmd -?
Microsoft (R) SQL Server Command Line Tool
Version 13.1.0007.0 Linux
Copyright (c) 2012 Microsoft. All rights reserved.

usage: sqlcmd            [-U login id]          [-P password]
  [-S server or Dsn if -D is provided]
  [-H hostname]          [-E trusted connection]
  [-N Encrypt Connection][-C Trust Server Certificate]
  [-d use database name] [-l login timeout]     [-t query timeout]
  [-h headers]           [-s colseparator]      [-w screen width]
  [-a packetsize]        [-e echo input]        [-I Enable Quoted Identifiers]
  [-c cmdend]
  [-q "cmdline query"]   [-Q "cmdline query" and exit]
  [-m errorlevel]        [-V severitylevel]     [-W remove trailing spaces]
  [-u unicode output]    [-r[0|1] msgs to stderr]
  [-i inputfile]         [-o outputfile]
  [-k[1|2] remove[replace] control characters]
  [-y variable length type display width]
  [-Y fixed length type display width]
  [-p[1] print statistics[colon format]]
  [-R use client regional setting]
  [-K application intent]
  [-M multisubnet failover]
  [-b On error batch abort]
  [-D Dsn flag, indicate -S is Dsn]
  [-X[1] disable commands, startup script, environment variables [and exit]]
  [-x disable variable substitution]
  [-? show syntax summary]
$ docker run beardedfoo/mssql-tools bcp -?
usage: bcp {dbtable | query} {in | out | queryout | format} datafile
  [-m maxerrors]            [-f formatfile]          [-e errfile]
  [-F firstrow]             [-L lastrow]             [-b batchsize]
  [-n native type]          [-c character type]      [-w wide character type]
  [-N keep non-text native] [-q quoted identifier]
  [-t field terminator]     [-r row terminator]
  [-a packetsize]           [-K application intent]
  [-S server name or DSN if -D provided]             [-D treat -S as DSN]
  [-U username]             [-P password]
  [-T trusted connection]   [-v version]             [-R regional enable]
  [-k keep null values]     [-E keep identity values]
  [-h "load hints"]         [-d database name]
```
