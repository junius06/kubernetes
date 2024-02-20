## MySQL ##
---

### Description
** Raw Datebase **




### How to show databases in a MySQL POD ###
** 1. Access in Pod **

```
kubectl exec -it mysql-0 -- /bin/sh
```


** 2. Access MySQL **
- No space between '-p' and 'ROOT_PASSWORD'

```
mysql -u root -p<ROOT_PASSWORD>
```


** 3. Show all databases **

```
show databases;
```


** 4. Show tables in database **

```
use <database>;
show tables;
```


** 5. Show information of a table **

```
desc <Table_Name>;
select * from <Table_Name>;
```


** 6. Show last updated block data **

```
select * from infos.last_updated_block;
```