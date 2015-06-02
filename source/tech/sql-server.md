## About sql-server

Microsoft SQL Server is a relational database management system. Use this tag for all SQL Server editions including Compact, Express, Azure, Fast-track and PDW. Do not use this tag for other types of DBMS (MySQL, PostgreSQL, etc.).

[Microsoft's SQL Server](http://www.microsoft.com/sqlserver) is a suite of **_relational database management system_** (RDBMS) products providing multi-user database access functionality. It originated from the Sybase SQL Server 4.x codebase and _Transact-SQL dialect_ (T-SQL), but it has forked significantly since then.

SQL Server is available in multiple versions, typically identified by release year, and versions are subdivided into _editions_ to distinguish between product functionality. The latest released version is [SQL Server 2014](http://www.microsoft.com/sqlserver/en/us/editions.aspx).

The SQL Server product range is split broadly into five categories:

1.  **SQL Server** is the main suite of enterprise and developer server products. Primary differences are licensing costs, capacities, and components included in the product, with some minor differences supported language features. Standard components include database language and storage server, developer tools, [ETL](http://en.wikipedia.org/wiki/Extract,_transform,_load) tools, schedulers, and replication. Other components include OLAP, reporting, and parallel computation. Components runs as NT Services.

2.  **SQL Server Express** is free for use and distribution but has reduced engine performance, functionality and capacity than found in its other server siblings. It is focused on small deployments and runs as an NT Service.

3.  **SQL Server Compact** is an embeddable subset of SQL Server. Like the Express edition it has a reduced language, functionality and capacity, but it is free to distribute. It's focused on small installations and desktop applications where its small footprint and no-management-required features are a great advantage.

4.  **SQL Azure** is a completely managed, hosted, high-availability instance of SQL Server 2005 with some language syntax support for federated queries, operated in [Microsoft Azure](http://www.microsoft.com/windowsazure/) datacenters.

5.  **SQL Server Parallel Data Warehouse** is a pre-built DataWarehouse appliance that offers massively parallel processing for SQL Server, allowing support for many hundreds of terabytes.

**SQL Server Release History**

    Version     Year  Release Name             Codename
    1.0 (OS/2)  1989  SQL Server 1.0 (16 bit)   Ashton-Tate 
    1.1 (OS/2)  1991  SQL Server 1.1 (16 bit)    -
    4.21(WinNT) 1993  SQL Server 4.21           SQLNT
    6.0         1995  SQL Server 6.0            SQL95
    6.5         1996  SQL Server 6.5            Hydra
    7.0         1998  SQL Server 7.0            Sphinx
     -          1999  SQL Server 7.0 OLAP Tools Palato mania
    8.0         2000  SQL Server 2000           Shiloh
    8.0         2003  SQL Server 2000 x64       Liberty
    9.0         2005  SQL Server 2005           Yukon
    10.0        2008  SQL Server 2008           Katmai
    10.25       2010  SQL Azure DB              CloudDatabase
    10.5        2010  SQL Server 2008 R2        Kilimanjaro (aka KJ)
    11.0        2012  SQL Server 2012           Denali
    12.0        2014  SQL Server 2014           Hekaton

**References**

*   [MSDN SQL Server 2005 Transact-SQL Reference](http://msdn.microsoft.com/en-us/library/ms189826.aspx)
*   [MSDN SQL Server 2008 R2 Transact-SQL Reference](http://msdn.microsoft.com/en-us/library/bb510741(v=sql.105))
*   [MSDN SQL Server 2012 Transact-SQL Reference](http://msdn.microsoft.com/en-us/library/bb510741(v=sql.110))
*   [MSDN SQL Server 2014 Transact-SQL Reference](http://msdn.microsoft.com/en-us/library/bb510741)
*   [SQL Server Wikipedia Article](http://en.wikipedia.org/wiki/Microsoft_SQL_Server)
*   [SQL Azure Stack-Overflow Tag](http://stackoverflow.com/tags/sql-azure/info)
*   [MSDN SQL Server DevCenter](http://msdn.microsoft.com/en-in/sqlserver/aa336270.aspx)
*   [SQL Server Best Practices](http://msdn.microsoft.com/en-us/sqlserver/bb671430)

**Tagging recommendation:**

There are several version specific tags. It is recommended to use the [sql-server](http://stackoverflow.com/questions/tagged/sql-server "show questions tagged 'sql-server'") tag together with the version specific tag, e.g. [sql-server-2005-express](http://stackoverflow.com/questions/tagged/sql-server-2005-express "show questions tagged 'sql-server-2005-express'").Do not use this tag for other types of DBMS ([mysql](http://stackoverflow.com/questions/tagged/mysql "show questions tagged 'mysql'"), [postgresql](http://stackoverflow.com/questions/tagged/postgresql "show questions tagged 'postgresql'"), etc.).

Code Language (used for [syntax highlighting](http://google-code-prettify.googlecode.com/svn/trunk/README.html)): lang-sql

  lang-sql