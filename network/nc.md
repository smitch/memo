# basics

## [ncコマンドの使い方](https://qiita.com/hana_shin/items/97e6c03ac5e5ed67ce38#0-nc%E3%82%B3%E3%83%9E%E3%83%B3%E3%83%89%E3%81%A8%E3%81%AF)

クライアント側
[root@client ~]#  nc server 11111
12345

サーバ側
[root@server ~]#  nc -kl 11111
12345

##  [netcatでHTTPリクエストを送ってみる](https://qiita.com/tags/http)
<!-- tag: http, netcat -->

```
nc example.com 80
GET / HTTP/1.1
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTExMzk0ODkxMF19
-->