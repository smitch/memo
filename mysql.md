

# load data infile
```
optin: --local-infile
```
- [ csvをLOAD DATA INFILEするときよく発行するクエリ](https://qiita.com/hdtkkj/items/ab4a66237dc8d1c2f1e1)

```sql
LOAD DATA INFILE '/data/mysql_backup/filename.csv' INTO TABLE event_hisotry 
  FIELDS TERMINATED BY ',' ENCLOSED BY '"' (member_id, event_id, `created_at`);
```
- [mysqlのテーブルに大量のcsvファイルをインポートしたい](https://detail.chiebukuro.yahoo.co.jp/qa/question_detail/q1469942604)

```sql
LOAD DATA local INFILE 'filename' ignore INTO TABLE `tbl_name` (`column1`,`column2`,`column3` ) SET `col_name` = '2011-09-01' ;
```

# copy database
```sql
$ mysqldump -u user_name -p from_db > from_db.dump.sql  
$ mysqladmin -u user_name -p create dest_db  
$ mysql -u user_name -p dest_db < from_db.dump.sql`
``` 
- https://weblabo.oscasierra.net/mysql-database-copy/
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTc4NjAxMjI3OV19
-->