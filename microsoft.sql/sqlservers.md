##Backing up and restoring databases

###Recommended steps
SQL Database keeps replicas of your database so that you can recover from outages and user errors. This includes restoring a database to a previous point in time, restoring a deleted database, or recovering from a data center outage. Available options depend on the database service tier and options you chose. After the database is restored, make sure you go through the checklist of finalization tasks before you put a newly recovered Azure SQL Database back into production.

* Restore a database to a previous point in time.<br>
 Click "Restore" at the top of the resource blade for your selected SQL database to open the "Restore blade," and then fill in the necessary details.
* Restore an accidentally deleted database.<br>
  Click the "Deleted Databases" tile at the bottom of your SQL server resource blade under "Operations" to start the restore process.
* Restore as a new database from a geo-redundant backup, which is also called as Geo-restore.<br>
  Click "New," click "Data and Storage," click "SQL Database," and then select "Backup" in the source list.
* Complete finalization task checklist for a restored database<br>
  [Finalize your restored database](https://azure.microsoft.com/documentation/articles/sql-database-recovered-finalize/)
* Restore a single table from Azure database backup.
  [How to restore a single table from an Azure SQL Database backup](https://azure.microsoft.com/documentation/articles/sql-database-cloud-migrate-restore-single-table-azure-backup/)

###Recommended documents
[Restore a database to a previous point in time, restore a deleted database, or recover from a data center outage](https://azure.microsoft.com/documentation/articles/sql-database-troubleshoot-backup-and-restore/) <br>
[Business Continuity Overview](https://azure.microsoft.com/documentation/articles/sql-database-business-continuity/)

######metadata:sqldatabase

##How do I migrate

###Recommended documents
[Migrate your solution to SQL Data Warehouse](https://azure.microsoft.com/documentation/articles/sql-data-warehouse-overview-migrate/) 

######metadata:sqldatawarehouse

##My queries are slow

###Recommended documents
[My queries are running slow](https://azure.microsoft.com/documentation/articles/sql-data-warehouse-troubleshoot/) 

######metadata:sqldatawarehouse

##My database is slow

###Recommended steps
Missing indexes and poorly optimized queries are common reasons for poor database performance. First identify opportunities to fine tune these by using "Query Performance Insight" and "Index advisor tools" using the links below. If the problems persist, consider changing the service tier of a single database or increasing the eDTUs of an elastic database pool at any time to improve performance.

* Find the top consuming queries, and identify the ones that have to be fixed.<br>
  [Query Performance Insight](data-blade:SqlAzureExtension:QueryPerformanceBlade)
* Get Index recommendations and create indexes.<br>
  [Index Advisor](data-blade:SqlAzureExtension:DatabaseIndexBlade)
* Analyze the metrics shown on the SQL server resource blade to identify whether any resource is being overutilized or throttled. Mitigate resource issues by scaling up or out.<br>
  [Understand what's available in each service tier](https://azure.microsoft.com/documentation/articles/sql-database-service-tiers/)
* Complete finalization task checklist for a restored database<br>
  [Finalize your restored database](https://azure.microsoft.com/documentation/articles/sql-database-recovered-finalize/)
* For multiple databases, scale resources automatically with Elastic Database Pool.<br>
  [Understand elastic database pools](https://azure.microsoft.com/documentation/articles/sql-database-elastic-pool-guidance/)

###Recommended documents
[Troubleshoot Azure SQL Database performance](https://azure.microsoft.com/documentation/articles/sql-database-troubleshoot-backup-and-restore/)<br>
[Monitoring using DMVs](https://azure.microsoft.com/documentation/articles/sql-database-business-continuity/)<br>
[Extended Events](https://azure.microsoft.com/documentation/articles/sql-database-xevent-db-diff-from-svr/)<br>
[Benchmark overview](https://azure.microsoft.com/documentation/articles/sql-database-benchmark-overview/)

######metadata:sqldatabase

##My database is slow

###Recommended steps
Missing indexes and poorly optimized queries are common reasons for poor database performance. First identify opportunities to fine tune these by using "Query Performance Insight" and "Index advisor tools" using the links below. If the problems persist, consider changing the service tier of a single database or increasing the eDTUs of an elastic database pool at any time to improve performance.

* Find the top consuming queries, and identify the ones that have to be fixed.<br>
  [Query Performance Insight](https://azure.microsoft.com/documentation/articles/sql-database-query-performance/)
* Get Index recommendations and create indexes.<br>
  [Index Advisor](https://azure.microsoft.com/documentation/articles/sql-database-index-advisor/)
* Analyze the metrics shown on the SQL server resource blade to identify whether any resource is being overutilized or throttled. Mitigate resource issues by scaling up or out.<br>
  [Understand what's available in each service tier](https://azure.microsoft.com/documentation/articles/sql-database-service-tiers/)
* Complete finalization task checklist for a restored database<br>
  [Finalize your restored database](https://azure.microsoft.com/documentation/articles/sql-database-recovered-finalize/)
* For multiple databases, scale resources automatically with Elastic Database Pool.<br>
  [Understand elastic database pools](https://azure.microsoft.com/documentation/articles/sql-database-elastic-pool-guidance/)

###Recommended documents
[Troubleshoot Azure SQL Database performance](https://azure.microsoft.com/documentation/articles/sql-database-troubleshoot-backup-and-restore/)<br>
[Monitoring using DMVs](https://azure.microsoft.com/documentation/articles/sql-database-business-continuity/)<br>
[Extended Events](https://azure.microsoft.com/documentation/articles/sql-database-xevent-db-diff-from-svr/)<br>
[Benchmark overview](https://azure.microsoft.com/documentation/articles/sql-database-benchmark-overview/)

######metadata:sqlserver