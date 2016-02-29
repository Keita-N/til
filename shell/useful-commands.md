# linux commands
## 再帰的にディレクトリを作成する
```
$ mkdir -p src/{main,test}/{java,resouces,scala}
$ tree
.
└── src
    ├── main
    │   ├── java
    │   ├── resouces
    │   └── scala
    └── test
        ├── java
        ├── resouces
        └── scala
```
-p オプションで中間のフォルダも再帰的に作成する。

## tee コマンド

> 標準入力を標準出力とファイル同時ｎ出力する。

```
$ echo "hoge" | tee sample.txt

# -a file: fileに追記する
$ echo "hoge" | tee -a sample.txt

# 標準エラーもまとめてみる
$ ping 9999 2>&1 | tee result.txt
```
