
# starter-kit
## sassc
- https://thr3a.hatenablog.com/entry/20180308/1520506843
```bash
git clone https://github.com/sass/sassc.git
. sassc/script/bootstrap
make -C sassc -j4
PREFIX="~/local" make -C sassc install
```

## install
```bash
git clone https://github.com/cockpit-project/starter-kit
cd starter-kit
make
mkdir -p ~/.local/share/cockpit
ln -s `pwd`/dist ~/.local/share/cockpit/starter-kit
```

# cockpit-podman
## install
```
git clone https://github.com/cockpit-project/cockpit-podman.git 
cd cockpit-podman
make
ln -s `pwd`/dist ~/.local/share/cockpit/cockpit-podman
```
## run podman service
```bash
systemctl --user start podman
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE0MzUxNTg4MTUsLTE0NjYwOTIwMjJdfQ
==
-->