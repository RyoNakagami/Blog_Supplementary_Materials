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
#### (1) すでにpush済みのファイル名称の変更

> Syntax

```zsh
% git mv options <oldFilename> <newFilename>
```

- 追加で`git add`を実行する必要はありません

> 動作説明

`mv`コマンドを用いて,`git mv`と同じ動作をするコードを以下紹介します. 
そもそもですが,`mv`コマンドはファイル名を変更するのではありません. `<oldFilename>`を削除し、`<oldFilename>`と同じ内容を持つ新しいファイル`<newFilename>`を作成するものです. `git mv`も内部的には同じ動作をしています.

```zsh
% mv <oldFilename> <newFilename>
% git add <newFilename>
% git rm <oldFilename>
```

> Options

- `-f`: 移動または名前の変更操作を強制します. 同じ名前の別のファイルが存在する場合でも, ファイルを移動または名前変更します
- `-n`: 実際の操作を行わず, 何が起こるかを表示するだけ 
- `-k`: エラーを引き起こす可能性のある操作をスキップします
- `-v`: ファイル名を変更したり移動したりしたときに, そのファイル名を報告

#### (2) すでにpush済みのフォルダ名称の変更

> Syntax

```zsh
% git mv options <oldFoldername> <newFoldername>
```

> 動作説明

```zsh 
% mv oldfolder newfolder
% git add newfolder 
% git commit -m 'start rename'     
% git push origin main
% git rm -r oldfolder
% git commit -m 'rename complete' 
% git push origin main
```


## 参考
### オンラインマテリアル

- [stackoverflow > How to rename a directory/folder on GitHub website?](https://stackoverflow.com/questions/31861651/how-to-rename-a-directory-folder-on-github-website)
