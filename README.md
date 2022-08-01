**Table of Contents**
<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Git/GitHubチートシート](#gitgithub%E3%83%81%E3%83%BC%E3%83%88%E3%82%B7%E3%83%BC%E3%83%88)
  - [git add編](#git-add%E7%B7%A8)
    - [(1) git addを取り消す（git init直後のみ)](#1-git-add%E3%82%92%E5%8F%96%E3%82%8A%E6%B6%88%E3%81%99git-init%E7%9B%B4%E5%BE%8C%E3%81%AE%E3%81%BF)
    - [(2) git addを取り消す（First Commit移行)](#2-git-add%E3%82%92%E5%8F%96%E3%82%8A%E6%B6%88%E3%81%99first-commit%E7%A7%BB%E8%A1%8C)
  - [ファイルのstagedからの削除](#%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%81%AEstaged%E3%81%8B%E3%82%89%E3%81%AE%E5%89%8A%E9%99%A4)
    - [(非推奨)stageされた特定のファイルを一括除外したい場合](#%E9%9D%9E%E6%8E%A8%E5%A5%A8stage%E3%81%95%E3%82%8C%E3%81%9F%E7%89%B9%E5%AE%9A%E3%81%AE%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%82%92%E4%B8%80%E6%8B%AC%E9%99%A4%E5%A4%96%E3%81%97%E3%81%9F%E3%81%84%E5%A0%B4%E5%90%88)
    - [stagedされたファイルを.gitignore経由で一括除外したい場合](#staged%E3%81%95%E3%82%8C%E3%81%9F%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%82%92gitignore%E7%B5%8C%E7%94%B1%E3%81%A7%E4%B8%80%E6%8B%AC%E9%99%A4%E5%A4%96%E3%81%97%E3%81%9F%E3%81%84%E5%A0%B4%E5%90%88)
  - [Respository上のフォルダ/ファイルの名前変更](#respository%E4%B8%8A%E3%81%AE%E3%83%95%E3%82%A9%E3%83%AB%E3%83%80%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%81%AE%E5%90%8D%E5%89%8D%E5%A4%89%E6%9B%B4)
    - [(1) すでにpush済みのファイル名称の変更](#1-%E3%81%99%E3%81%A7%E3%81%ABpush%E6%B8%88%E3%81%BF%E3%81%AE%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E5%90%8D%E7%A7%B0%E3%81%AE%E5%A4%89%E6%9B%B4)
    - [(2) すでにpush済みのフォルダ名称の変更](#2-%E3%81%99%E3%81%A7%E3%81%ABpush%E6%B8%88%E3%81%BF%E3%81%AE%E3%83%95%E3%82%A9%E3%83%AB%E3%83%80%E5%90%8D%E7%A7%B0%E3%81%AE%E5%A4%89%E6%9B%B4)
  - [ファイルの表示](#%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%81%AE%E8%A1%A8%E7%A4%BA)
    - [(1) 更新されたファイルの表示](#1-%E6%9B%B4%E6%96%B0%E3%81%95%E3%82%8C%E3%81%9F%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%81%AE%E8%A1%A8%E7%A4%BA)
    - [(2) マージされていないファイルの表示](#2-%E3%83%9E%E3%83%BC%E3%82%B8%E3%81%95%E3%82%8C%E3%81%A6%E3%81%84%E3%81%AA%E3%81%84%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%81%AE%E8%A1%A8%E7%A4%BA)
    - [(3) ファイルをカレントディレクトリからのパスで表示](#3-%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%82%92%E3%82%AB%E3%83%AC%E3%83%B3%E3%83%88%E3%83%87%E3%82%A3%E3%83%AC%E3%82%AF%E3%83%88%E3%83%AA%E3%81%8B%E3%82%89%E3%81%AE%E3%83%91%E3%82%B9%E3%81%A7%E8%A1%A8%E7%A4%BA)
    - [(4) gitignoreの対象ファイルの表示](#4-gitignore%E3%81%AE%E5%AF%BE%E8%B1%A1%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%81%AE%E8%A1%A8%E7%A4%BA)
- [参考](#%E5%8F%82%E8%80%83)
  - [オンラインマテリアル](#%E3%82%AA%E3%83%B3%E3%83%A9%E3%82%A4%E3%83%B3%E3%83%9E%E3%83%86%E3%83%AA%E3%82%A2%E3%83%AB)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


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

### ファイルのstagedからの削除
#### (非推奨)stageされた特定のファイルを一括除外したい場合

git管理されているディレクトリにて,`.DS_Store`をサブディレクトリ下に存在するもの含めてすべて削除したいとします.
この場合,再帰的に`git rm`を実行する必要があるので

```zsh
% git rm --cached -r .DS_Store
```

- この方法は非推奨です
- [stagedされたファイルを.gitignore経由で一括除外したい場合](#staged%E3%81%95%E3%82%8C%E3%81%9F%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%82%92gitignore%E7%B5%8C%E7%94%B1%E3%81%A7%E4%B8%80%E6%8B%AC%E9%99%A4%E5%A4%96%E3%81%97%E3%81%9F%E3%81%84%E5%A0%B4%E5%90%88)を参考に実行してください


#### stagedされたファイルを.gitignore経由で一括除外したい場合

```zsh
% git rm --cached `git ls-files --full-name -ic --exclude-standard` 
```

- `--cached` オプションを付けることにより,ファイルを残したまま管理対象から外す
- `--cached` オプションを付与しない場合はファイルごと削除
- `git ls-files -c`はインデックスされている(=git 管理下)ファイルの一覧を表示
- `git ls-files -i`はステージングエリアに存在する無視されるファイルのみを表示（無視のルールは` --exclude-standard`で指定=`.gitignore`対象ファイル）

> 動作説明

基本的には,インデックスされているがステージングエリアに存在する無視されるべきファイルのみを表示し、それら対象に`git rm --cached`を実行する


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

### ファイルの表示
#### (1) 更新されたファイルの表示

```zsh
% git ls-files -m
```

#### (2) マージされていないファイルの表示

```zsh
% git ls-files -u
```

#### (3) ファイルをカレントディレクトリからのパスで表示

```zsh
% git ls-files --full-name
```

#### (4) gitignoreの対象ファイルの表示

```zsh
% git ls-files -io --exclude-standard
```

- `-i`オプションで無視ファイル(ignore)のみを表示
- `-o`オプションを渡すことで管理対象外のファイルを表示
- `--exclude-standard` オプションは `.gitignore` 等で無視されているファイルを除外するオプション

## 参考
### オンラインマテリアル

- [GitHub Docs > 機密データをリポジトリから削除する](https://docs.github.com/ja/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository#avoiding-accidental-commits-in-the-future)
- [stackoverflow > How to rename a directory/folder on GitHub website?](https://stackoverflow.com/questions/31861651/how-to-rename-a-directory-folder-on-github-website)
