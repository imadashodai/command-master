### 1. ディレクトリ内の移動
* cd

```
$ cd /path/to/directory
```

### 2. 現在いるディレクトリの確認
* pwd

```
$ pwd
```

### 3. リスト表示
* ls

```
$ ls /path/to/directory
```

### 4. ファイルの内容を表示
* cat

|オプション|意味|
|:--|--:|
|-n|全ての行に行番号をつける|
|-s|空行を除く|
|-b|空行以外に行番号をつける|

```
$ cat [option] filename
```

### 5. Practice
1. cdコマンドでcollectionディレクトリに移動しよう。
2. pwdコマンドで現在いるディレクトリを確認しよう。
3. lsコマンドでcollectionディレクトリの中身を表示しよう。
4. catコマンドでusers.csvの中身を表示させよう。また、行番号をつけて表示させよう。

### 6. Answers
1. cdコマンドでcollectionディレクトリに移動しよう。

```
$ pwd
fullpath/command-master

$ cd collection
```

2. pwdコマンドで現在いるディレクトリを確認しよう。

```
$ pwd
fullpath/command-master/collection
```

3. lsコマンドでcollectionディレクトリの中身を表示しよう。

```
$ ls
users.csv       users.tsv
```

4. catコマンドでusers.csvの中身を表示させよう。また、行番号をつけて表示させよう。

```
$ cat users.csv
id,lname,sex,no
1,"hayashi","m","00010"
2,"takahashi","m","00044"
3,"suzuki","f","00009"
4,"nakamura","m","00048"
5,"satou","m","00024"
...

$ cat -n users.csv
1  id,lname,sex,no
2  1,"hayashi","m","00010"
3  2,"takahashi","m","00044"
4  3,"suzuki","f","00009"
5  4,"nakamura","m","00048"
...
```
