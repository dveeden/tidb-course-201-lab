# Best Practice: JDBC Batch Insert (Output)
```10
(flash) [scripts]: [master]$ ./10-demo-jdbc-batch-insert-01-show.sh
Connection established.
>>> Begin batch insert.
>>> End batch insert, ~!@rewriteBatchedStatements=true, elapsed: 452 (ms)@!~.
Connection established.
>>> Begin batch insert.
>>> End batch insert, ~!@rewriteBatchedStatements=false, elapsed: 20505 (ms)@!~.

/* Executing query: select count(*), max(name) from test.t1_batchtest; */
        Row#, ~!@count(*)@!~, max(name)
        1) ~!@20000@!~, 9999
Turn on autocommit.
Connection closed.
```