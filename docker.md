
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

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTgzMjU5NDg1LDE2MzQ3NDYzNiwtNzM3Nz
M5MTQwXX0=
-->