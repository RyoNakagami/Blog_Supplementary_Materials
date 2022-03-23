**Table of Contents**
<!-- START doctoc -->
<!-- END doctoc -->


## Git/GitHubチートシート
### (1) git addを取り消す（git init直後のみ)

```zsh
## 特定のファイルのgit addを取り消す
% git rm --cached -r <filename>

## すべてのファイルのgit addを取り消す
% git rm --cached -r ./*
```
### (2) git addを取り消す（First Commit移行)

```zsh
###全てのファイルを取り消し
% git reset HEAD

###特定のファイルのみ取り消し
% git reset HEAD <filename>
```
