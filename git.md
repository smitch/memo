
# push tags to remote
git push origin --tags

# push branch to remote
git push origin <branch name>

# show and get file from another branch
git show <branch name>:<file name>
git checkout <branch name> -- <file name>

# track only designated directory in repository
cd path/to/git/clone/repository
git config core.sparsecheckout true
echo "path/to/include/only/this/directory" > .git/info/sparse-checkout
git read-tree -m -u HEAD

# color setting
git config --global color.ui true

# first setting
git config --global user.name "my name"
git config --global user.email "my email@address"

# config url setting
url = ssh://git@github.com/<my account>/<my repository>

# private git
useradd git
echo "Match User git" >> /etc/ssh/sshd_config
echo "PasswordAuthentication no" >> /etc/ssh/sshd_config

change login shell to git-shell
/etc/passwd
git ... /bin/bash -> git ... /usr/bin/git-shell

make keys

# repository list
```
curl -sSa "https://api.github.com/users/<user_name>/repos?per_page=100" | grep '"name"' | cut -d '"' -f4
```

# resetting
git resed --hard <commit_id>

git revert <commit_id>

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTA0MDU0NzQ4MCwtNjA2MTYzNzA4XX0=
-->