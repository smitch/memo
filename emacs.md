
# frequently use key binding
  * C-M-p: go to previous (corresponding) parent
  * C-M-n: go to next (corresponding) parent
  * C-x 0: close window
  * M-x ffap: find file at point

# change inner
    * install by package-list
    * add below
(require 'ciel)
(global-set-key "\C-ci" 'ciel-ci)
(global-set-key "\C-co" 'ciel-co)

# sudo-edit
    * install from package-list
    * open file and run M-x sudo-edit

# reload file
    * run M-x revert-buffer

# [indent off](https://stackoverflow.com/questions/986592/any-emacs-command-like-paste-mode-in-vim)
```
M-x electric-indent-mode RET
```


# mg
- https://github.com/troglobit/mg


# packege install
-  [emacs起動時の自動パッケージインストール](https://riptutorial.com/ja/emacs/example/7979//emacs起動時の自動パッケージインストール)



# emacs-client
```
emacs --daemon
emacsclient -nw -a '' <fine name>
emacsclient -e '(kill-emacs)'
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTEyNzgyNTYwMl19
-->