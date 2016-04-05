# Split Window
---
|command||
|---|---|
|\<C-w>s|水平分割|
|\<C-w>v|垂直分割|

## Change forcus
|command||
|---|---|
|\<C-w>w|フォーカスを順次移動|
|\<C-w>h|左のウインドウにフォーカス|
|\<C-w>j|下のウインドウにフォーカス|
|\<C-w>k|上のウインドウにフォーカス|
|\<C-w>l|右のウインドウにフォーカス|


### 後で整理
- reload .vimrc
 
```
:source ~/.vimrc
```

- ステータスラインを表示する

```
<Ctrl> + g
```

- スクロール

|command||
|---|---|
|\<Ctrl> + u | 上方スクロール |
|\<Ctrl> + d | 下方スクロール |

- Scrolling relative to cursor (:h scroll-cursor)

カーソル行を固定してスクロール

```
# カーソル行をコンソール先頭に移動
z<CR> or zt 

# カーソル行をコンソール中央に移動
zz or z.

# カーソル行をコンソール最下に移動
z- or zb 

# コンソールの高さを{height}行分に変更
z{height}<CR>

```

- 大文字、小文字変換

| command ||
|---|---|
| g~~ | 現在行全体の大文字小文字を反転させる|
| vU | 現在行の先頭を大文字にする|
| vu | 現在行の先頭を小文字にする|
| v~ | 現在行の先頭の大文字小文字を反転させる|
| gu{motion} | {motion}を小文字にする (:h gu)|
| gugu, guu | 現在行を小文字にする |
| gU{motion} | {motion}を大文字にする (:h gU) |
| gUgU, gUU | 現在行を大文字にする |
| g~{motion}, g~g~, g~~ | (省略) 大文字小文字反転|
