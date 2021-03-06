### 1. 上から○行目までを表示する
* head

|オプション|意味|
|:--|--:|
|-n|行数を指定する(省略可)|
|-c|バイト数を指定する|

```
$ head users.tsv
```

### 2. 下から○行目までを表示する
* tail

オプションはheadコマンドと同様。

```
$tail users.tsv
```

### 3. 並び替え
* sort

|オプション|意味|
|:--|--:|
|-r|逆順に並べる|
|-n|数値の昇順に並べる|
|-k|何列目かを指定する|
|-t|区切り文字のを指定する|

```
$ sort -r users.csv
```

### 4. 文字列を検索する
* grep [オプション] [引数] [ファイル名]

|オプション|意味|
|:--|--:|
|-c|引数を含む行数|
```
$ grep 'takahashi' users.csv
```

### 5. ディレクトリやファイルを検索
* find [ディレクトリ] [検索条件]

|オプション|意味|
|:--|--:|
|-name|ファイル名を指定|
|-empty|空のファイル|
|-type f|ファイルを検索|
|-type d|ディレクトリを検索|

```
$ find instructions -name '*step.md'
```

### 6. Practice
1. users.csvの上から5行目までを出力しよう。
2. users.tsvの下から3行目までを出力しよう。
3. users.csvを"no"の昇順に並べよう。
4. users.tsvに"tanaka"が何人いるか調べよう。
5. collectionディレクトリの中に「user」がつくファイルがいくつあるか調べよう。

### 7. Answer
1. users.csvの上から5行目までを出力しよう。

```
$ head -5 users.csv

id,lname,sex,no
1,"hayashi","m","00010"
2,"takahashi","m","00044"
```
2. users.tsvの下から3行目までを出力しよう。

```
$ tail -3 users.tsv

48	"tanaka"	"m"	"00050"
49	"takahashi"	"f"	"00013"
50	"shimizu"	"f"	"00025"
```
3. users.csvを"no"の昇順に並べよう。

```
$ sort -t ',' -k4 users.csv

16,"inoue","f","00001"
45,"yoshida","m","00002"
36,"yamaguchi","m","00003"
22,"katou","m","00004"
44,"yamada","f","00005"
...
```
4. users.tsvに"tanaka"が何人いるか調べよう。

```
$ grep 'tanaka' users.tsv | wc -l

2
```
※最後に登場したwcは行数や文字数を数えるコマンド

5. collectionディレクトリの中に「user」がつくファイルがいくつあるか調べよう。

```
$ find collection -name 'user*' | wc -l

2
```

[前のステップに戻る](https://github.com/imadashodai/command-master/blob/master/instructions/second_step.md)

[次のステップに進む](#)
