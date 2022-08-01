**Table of Contents**
<!-- START doctoc -->
<!-- END doctoc -->


## Git/GitHubチートシート
### git add編
#### (1) git addを取り消す（git init直後のみ)

```zsh
## 特定のファイルのgit addを取り消す
% git rm --cached -r <filename>

## すべてのファイルのgit addを取り消す
% git rm --cached -r ./*
```
#### (2) git addを取り消す（First Commit移行)

```zsh
###全てのファイルを取り消し
% git reset HEAD

###特定のファイルのみ取り消し
% git reset HEAD <filename>
```

### Respository上のフォルダ/ファイルの名前変更
#### (1) すでにcommit済みのファイル名称の変更

> Syntax

```zsh
% git mv options <oldFilename> <newFilename>
```

> 動作説明


> Options

- [`-f`]: 移動または名前の変更操作を強制します.同じ名前の別のファイルが存在する場合でも,ファイルを移動または名前変更します
- [`-n`]: 実際の操作を行わず,何が起こるかを表示するだけ.
- [`-k`]: Sエラーを引き起こす可能性のある操作をスキップします.
- [`-v`]: ファイル名を変更したり移動したりしたときに、そのファイル名を報告.







## 参考
### オンラインマテリアル

- [stackoverflow > How to rename a directory/folder on GitHub website?](https://stackoverflow.com/questions/31861651/how-to-rename-a-directory-folder-on-github-website)
