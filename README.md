# git-alias-template


One advantage of aliases over setting `help.autocorrect` is you can be sure your typos will be interpreted as you intended.

```
[alias]
  co = checkout
  ci = commit
  st = status
  br = branch
  hist = log --pretty=format:'%h %ad | %s%d [%an]' --graph --date=short
  type = cat-file -t
  dump = cat-file -p

  psuh = push
  puhs = push
  
```
