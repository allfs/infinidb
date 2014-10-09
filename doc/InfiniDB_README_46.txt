/***********************************************************************
*
*   Copyright (C) 2013 InfiniDB Corp
*   All Rights Reserved
*
***********************************************************************/

July 7, 2014
Version 4.6


ENHANCEMENTS INCLUDED IN THIS RELEASE
-------------------------------------
Enh #   Short Description
1505	Implement temp file based LargeHashJoin for tuple joins	
3683	Allow function(column) = function(column) join	
5308	Improve performance of load data infile and insert into select from	


ISSUES RESOLVED IN THIS RELEASE
-------------------------------
Bug #   Short Description                                                                                                                                            

3858	While "load data infile" is in progress, PrimProc fails to read compressed chunk and retries for more than a minute
4295	CPimport Mode 2:  Should check for input files on all PMs before starting loading
4737	Distributed cpimport does not support a list of import files to a single table
4789	InfiniDB came up normally after encountering an critical sessionManager::rollback() error
5134	Source package:  After compilation and installation, InfiniDB reported lib not found error during startup
5140	second and subsequent load data infiles have 30 second delay with auto increment
5523	Mysql is resetting when running a query on a information_schema.table and an InfiniDB table.
5727	Improve logging around controllernode start up
5756	After a failed addModule command movePmDbrootConfig did not fail
5758	when amazon UM modules are removed, their associated EBS storages are not removed
5761	Support additional versions of Java for Hadoop installations
5762	Need a method to handle MySQL port conflict on a multi-server install
5773	Startsystem is failing when shutdown has not completed.
5847	IDB-2021 on query using multiple pseudo column functions against same column and aggregation
5848	No CP elimination from idbPartition(col) in the where clause
5865	ERROR 138 (HY000): IDB-1000: 'orders' and 'sub-query' are not joined on a query with an or condition and not in condition
5891	getsystemdisk reporting minus value
5894	Performance issue when inserting a value in an autoincrement column
5930	Not in group by error on query grouping by idbPm and idbDbRoot functions
5931	current builds do not support a non-root / hdfs install
5946	load data infile error: ERROR 122 (HY000): CAL0006:  Error verifying compression headers
5947	calonlinealter always creates non compressed columns
5950	getModuleHostNames command on AWS returned a segmentation fault error
5954	calpontSupport for Windows does not recognize options
5958	Query with a subselect is getting an assertion error
5963	configxml.sh fails to set CrossEngineSupport Password from the default setting
5978	crash with prepared statements
5987	hadoop test failed on install, hadoop not install where setenv was looking and not a parcel
5992	Bulk load fails on long schema name, long table name, and long column name combination.
5993	IDB-2016: Non supported item 'c2' on the GROUP BY list.
5996	Table reporting errors after a LDI
5997	standard mysql and infinidb mysql incorrectly starting/stopping each other
6000	New MySQL port test is insufficient
6001	cpimport performance improvement for tables with many dictionary columns
6005	addModule command failed to add an UM
6010	InfiniDB mysql replication doesn't work when UM mysql Port address is not 3306
6013	HW 2.1 testing with 4.5.1-2 - different JAVA_HOME's are setup
6017	Queries with "where date(col) in (select dtCol)" not finding rows
6026	Prevent potential infinite loops reading input in postConfigure
6027	post-install message for a non-root hadoop install is incorrect..
6029	when autocommit off, batchinsert set hwm of dictionary store file to 0
6041	When loading 4160825419 rows cpimport  reported as -134141877 rows
6044	'union all' query generates tupleconstantstep.cpp@731: assertion 'fRowConst.getSize() == fRowOut.getSize()' failed
6061	window function returned incorrect results
6066	query with alias is returning IDB-3009: Unknown column error.
6073	setenv scripts issues on Ubuntu
