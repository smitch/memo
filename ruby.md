# install rbenv
```
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
cd ~/.rbenv
src/configure
make -C src
PATH="~/.rbenv/shims:~/.rbenv/bin:$PATH"
git clone https://github.com/sstephenson/ruby-build.git ~/.rbenv/plugins/ruby-build

renv install -l
renv install <ruby version>
renv versions
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTk2MjM0MjI2XX0=
-->