<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->



<!-- END doctoc generated TOC please keep comment here to allow auto update -->

[# 任意のログをlogrotateを使って管理する](https://qiita.com/Esfahan/items/a8058f1eb593170855a1)
```
# logrotate -dv /etc/logrotate.conf
```
実際に実行するにはこちら
```
# /usr/sbin/logrotate /etc/logrotate.conf
```
ローテートする条件を満たしていなくても強制的に実行する場合は`-f`を付ける
```
# logrotate -f /etc/logrotate.conf
```
最後にローテーションされたログファイルの日付を確認する
```
# cat /var/lib/logrotate.status
…
logrotate state -- version 2
"/var/log/yum.log" 2017-1-13
"/var/log/dracut.log" 2017-1-13
"/var/lib/mysql/mysqld.log" 2017-1-13
(略)
```

[# rsyslogdがログファイルを掴んで離さない](https://iww.hateblo.jp/entry/20181026/rsyslog)
```
/var/log/hoge/piyo.log {
    daily
    missingok
    rotate 5
    compress

#   rsyslog経由なので、ログを更新させる
    sharedscripts
    postrotate
        invoke-rc.d rsyslog rotate > /dev/null
    endscript
}
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4NTgwMDIwNTNdfQ==
-->