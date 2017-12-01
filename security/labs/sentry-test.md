
<h3>Conjunto vacío</h3>

```
: jdbc:hive2://node2.gus.com:10000/default> SHOW TABLES;
INFO  : Compiling command(queryId=hive_20171130225252_b684dc10-e3af-47e4-a761-3108aa1ebfd7): SHOW TABLES
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20171130225252_b684dc10-e3af-47e4-a761-3108aa1ebfd7); Time taken: 0.628 seconds
INFO  : Executing command(queryId=hive_20171130225252_b684dc10-e3af-47e4-a761-3108aa1ebfd7): SHOW TABLES
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171130225252_b684dc10-e3af-47e4-a761-3108aa1ebfd7); Time taken: 0.288 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
+-----------+--+
No rows selected (2.271 seconds)
0: jdbc:hive2://node2.gus.com:10000/default>

```
# USUARIO  Ferdinand
```
INFO  : Compiling command(queryId=hive_20171201052424_cb121021-368e-4dff-a064-5f4d773d7917): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20171201052424_cb121021-368e-4dff-a064-5f4d773d7917); Time taken: 0.07 seconds
INFO  : Executing command(queryId=hive_20171201052424_cb121021-368e-4dff-a064-5f4d773d7917): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171201052424_cb121021-368e-4dff-a064-5f4d773d7917); Time taken: 0.113 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
| sample_07  |
+------------+--+
1 rows selected (0.187 seconds)
```

