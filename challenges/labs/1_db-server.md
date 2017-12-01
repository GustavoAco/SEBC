# Name Bd host
 SHOW VARIABLES WHERE Variable_name IN ('hostname','port');
+---------------+-------+
| Variable_name | Value |
+---------------+-------+
| hostname      | nodo1 |
| port          | 3306  |
+---------------+-------+
2 rows in set (0.00 sec)

# VErsion
mysql> SELECT version();
+-----------+
| version() |
+-----------+
| 5.7.20    |
+-----------+
1 row in set (0.00 sec)
# Databases

mysql> show databases
    -> ;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive               |
| hue                |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sys                |
+--------------------+
9 rows in set (0.00 sec)
