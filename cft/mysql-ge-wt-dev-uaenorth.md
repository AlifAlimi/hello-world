# mysql-ge-wt-dev-uaenorth

Display current date
```
C:\Program Files\MySQL\MySQL Server 8.0\bin>date
The current date is: Thu 05/20/2021
```

Connect to the Database Server
```
C:\Program Files\MySQL\MySQL Server 8.0\bin>mysql -u use_aadadmins@mysql-ge-wt-dev-uaenorth -hmysql-ge-wt-dev-uaenorth.mysql.database.azure.com -p
Enter password: ********
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 65141
Server version: 5.6.47.0 MySQL Community Server (GPL)

Copyright (c) 2000, 2021, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.
```

Check Database status
```
mysql> status
--------------
mysql  Ver 8.0.25 for Win64 on x86_64 (MySQL Community Server - GPL)

Connection id:          65141
Current database:
Current user:           use_aadadmins@183.171.76.146
SSL:                    Cipher in use is ECDHE-RSA-AES256-GCM-SHA384
Using delimiter:        ;
Server version:         5.6.47.0 MySQL Community Server (GPL)
Protocol version:       10
Connection:             mysql-ge-wt-dev-uaenorth.mysql.database.azure.com via TCP/IP
Server characterset:    latin1
Db     characterset:    latin1
Client characterset:    cp850
Conn.  characterset:    cp850
TCP port:               3306
Binary data as:         Hexadecimal
Uptime:                 64 days 6 hours 40 min 46 sec

Threads: 10  Questions: 1194191  Slow queries: 0  Opens: 35  Flush tables: 1  Open tables: 32  Queries per second avg: 0.215
--------------
```

Retrieve Database
```
mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
| sys                |
| wellnesstrace      |
+--------------------+
5 rows in set (0.16 sec)
```

Select databases and retrieve tables
```
mysql> use wellnesstrace;
Database changed
mysql> show tables;
Empty set (0.13 sec)
```