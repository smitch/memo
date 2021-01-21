# reset modification
git reset --hard <commit name>
<commit name>: HEAD or commmit hash value

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