[← 譜面ヘッダー仕様に戻る](dos_header.html)
## titlelineheight
[ver3.x以降]

### 使い方
```
|titlelineheight=50|
```
### 説明
デフォルトの曲名表示を使用した場合で曲名が2行になる場合、行間を指定します。  
デフォルトはタイトル1行目のフォントサイズ+10pxです。  
customTitleUseがfalseに設定されているとき、この値は無視されます。

### タイトル曲名文字(デフォルトデザイン)の設定箇所について
![dos-h0030-01.png](./wiki/dos-h0030-01.png)

### 関連項目
- [**titlesize**](dos-h0030-titlesize.html)  文字サイズ
- [**titlefont**](dos-h0031-titlefont.html)  フォント
- [titlepos](dos-h0033-titlepos.html)  X, Y座標位置

### 更新履歴

|Version|変更内容|
|----|----|
|[v3.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.2.0)|初回実装|