# install: https://gitforwindows.org/

## zet vs code als editor voor de global git:
git config --global core.editor "code --wait"

## open git config:
git config --edit --global


### [alias]
-  ac = !git add -A && git commit -m
-  acp = !git add -A && git commit -m "quikfix-test" && git push
-  lg = !git log --pretty=format:\"%C(magenta)%h%Creset -%C(red)%d%Creset %s %C(dim green)(%cr) [%an]\" --abbrev-commit -10
-  lb = "!git for-each-ref --sort='-authordate' --format='%(authordate)%09%(objectname:short)%09%(refname)' refs/heads | sed -e 's-refs/heads/--'"
-  main = !git checkout main && git pull origin 
-  master = !git checkout master && git pull origin 
-  dev = !git checkout dev && git pull origin dev
