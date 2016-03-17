# sudo で開き忘れたとき

> E45: 'readonly' option is set (add ! to override)

となったときは、

```vim
:w !sudo tee > /dev/null %

or

:w !sudo tee % > /dev/null
```
- % は現在開いているファイル
- !は外部コマンド実行
- :w でバッファの内容が!sudo tee に標準入力としてパイプされて、
- tee {file} は標準入力を{file}に出力すると同時に標準出力へ出力する
- > /dev/null だから、標準出力は捨てられて、% 現在開いているファイルにsudo権限で書き出される。

という仕組み。


