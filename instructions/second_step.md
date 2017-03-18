### 1. ファイルやディレクトリを削除する
* rm

```
$ rm /path/to/file or directory
```

|オプション|意味|
|:-|-:|
|-r|ディレクトリ以下を丸ごと削除|

### 2. 空のディレクトリを削除する
* rmdir

```
$ rmdir directory
```

### 3. ディレクトリを作成する
* mkdir

```
$ mkdir directoryname
```

### 4. ファイルやディレクトリを移動する・ファイル名やディレクトリ名を変更する
* mv

```
$ ls
originalfile

$ mv originalfail alteredfile

$ ls
alteredfile
```

### 5. ファイルやディレクトリをコピーする
* cp

```
$ ls
file

$ cp file copy_file

$ ls
file copy_file
```

### 6. Practice
1. 「osushi」というディレクトリを作成しよう。
2. 「osushi」ディレクトリの中に「ootoro.txt」というファイルを作成しよう。
3. 「ootoro.txt」ファイルを「chutoro.txt」という名前に変更しよう。
4. 「chutoro.txt」ファイルをコピーして「akami.txt」ファイルを作ろう。
5. 「chutoro.txt」ファイルを削除しよう。
6. 「osushi」ディレクトリを削除しよう。

### 7. Answers
1. 「osushi」というディレクトリを作成しよう。

```
$ pwd
fullpath/command-master

$ ls
README.md	collection	instructions

$ mkdir osushi

$ ls
README.md	collection	instructions	osushi
```

2. 「osushi」ディレクトリの中に「ootoro.txt」というファイルを作成しよう。

```
$ pwd
fullpath/command-master

$ cd osushi

$ vi ootoro.txt
エディタが開いたら
:wqで保存

$ ls
ootoro.txt
```

3. 「ootoro.txt」ファイルを「chutoro.txt」という名前に変更しよう。

```
$ ls
ootoro.txt

$ mv ootoro.txt chutoro.txt

$ ls
chutoro.txt
```

4. 「chutoro.txt」ファイルをコピーして「akami.txt」ファイルを作ろう。

```
$ ls
chutoro.txt

$ cp chutoro.txt akami.txt

$ ls
chutoro.txt akami.txt
```

5. 「chutoro.txt」ファイルを削除しよう。

```
$ ls
chutoro.txt akami.txt

$ rm chutoro.txt

$ ls
akami.txt
```

6. 「osushi」ディレクトリを削除しよう。

```
$ ls
osushi

$ rm -r osushi

$ls

```

[前のステップに戻る](https://github.com/imadashodai/command-master/blob/master/instructions/first_step.md)

[次のステップに進む](#)
