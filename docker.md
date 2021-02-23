
# install
## centos
- https://docs.docker.com/install/linux/docker-ce/centos/#install-using-the-repository

```
sudo yum install -y yum-utils \
    device-mapper-persistent-data \
    lvm2
sudo yum-config-manager \
    --add-repo \
    https://download.docker.com/linux/centos/docker-ce.repo
sudo yum install docker-ce docker-ce-cli containerd.io
sudo systemctl start docker
sudo docker run hello-world
```
## ubuntu
- [Ansibleを使用してUbuntu 18.04にDockerをインストールおよびセットアップする方法](https://www.codeflow.site/ja/article/how-to-use-ansible-to-install-and-set-up-docker-on-ubuntu-18-04)
# copy directory from guest to host
- https://stackoverflow.com/questions/35787702/docker-cp-a-folder-with-a-relative-symlink-invalid-symlink


# shell in container
`docker exec -it <container id> /bin/bash`
- https://qiita.com/yosisa/items/a5670e4da3ff22e9411a

# microk8s

- docker disappeared #382
- https://github.com/ubuntu/microk8s/issues/382
`They have [replaced](https://github.com/ubuntu/microk8s/commit/7c3311a6d24a0eae482dc09e86471ead41aaa19e) docker daemon with containerd. `

- [MicroK8s バージョン 1.13.4 と 1.14.0の違い](https://qiita.com/ynott/items/490946a4622d96dda9cb)

- [containerdとrunCの比較](https://www.it-swarm-ja.tech/ja/docker/containerd%E3%81%A8runc%E3%81%AE%E6%AF%94%E8%BC%83/830485645/)

# host port access
> host.docker.internal

https://qiita.com/Asayu123/items/ccfe4ccfc417ce57f445

# security
- [owasp cheatsheet](https://cheatsheetseries.owasp.org/cheatsheets/Docker_Security_Cheat_Sheet.html#docker-security-cheat-sheet)


# env
- [Docker で環境変数をホストからコンテナに渡す方法（ホスト OS 側からゲスト OS に渡す方法各種）](https://qiita.com/KEINOS/items/518610bc2fdf5999acf2)

```
docker run --env-file [ ファイルパス ] [ その他のオプション ] <イメージ名> [ コマンド ]
```

# container log
## [How to clean Docker container logs?](https://stackoverflow.com/questions/41091634/how-to-clean-docker-container-logs)
```
docker logs --since 30s -f <container_name_or_id>
```
```
docker logs --tail 20 -f <container_name_or_id>
```
```
echo "" > $(docker inspect --format='{{.LogPath}}' <container_name_or_id>)
```

# port forwarding
https://stackoverflow.com/questions/19897743/exposing-a-port-on-a-live-docker-container
```
sudo docker ps 
sudo docker commit <containerid> <foo/live>
sudo docker run -i -p 22 -p 8000:80 -m /data:/data -t <foo/live> /bin/bash
```

# summary
command|description
-|-|-
`docker run -d --rm <image tag/id>`|
`docker build . -t <tag>`|
`docker exec -it <container name/id> /bin/bash`|
`docker logs -f <container name/id>`|
`docker ps [-a]`|
`docker images`|
`docker image rm <image tag/id>`|
`docker rm <container name/id>`|
`docker commit <container name/id> <new container name>`|

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTYwMzc0NTY4OSwxNjU3OTY2MTI1LC0zMz
E1MDU5MDcsOTM5MjI5MjEwLC04MzI1OTQ4NSwxNjM0NzQ2MzYs
LTczNzczOTE0MF19
-->