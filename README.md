# trino_container

## Start the Trino container

```
[xxx@xxx trino_container]$ docker-compose down && docker-compose up -d --build
Creating trino_trino-coordinator_1 ... done
```

## Enter the Trino container

```
[xxx@xxx]$ docker exec -ti trino_container-trino-coordinator-1 bash
```

## Run the Trino CLI

```
[trino@trino-coordinator /]$ /usr/bin/trino
trino> show catalogs;
 Catalog
---------
 hive
 iceberg
 memory
 system
 tpcds
 tpch
(6 rows)

Query 20241112_184611_00007_za7wd, FINISHED, 1 node
Splits: 7 total, 7 done (100.00%)
0.18 [0 rows, 0B] [0 rows/s, 0B/s]
```
