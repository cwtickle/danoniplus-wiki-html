[← 譜面ヘッダー仕様に戻る](dos_header.html)
## titlesize
[ver2.x以降]

### 使い方
```
|titlesize=40|
|titlesize=40,20|
|titlesize=40$20|
```
### 説明
デフォルトの曲名表示を使用した場合に、曲名のフォントサイズを指定します。  
指定しない場合は、曲名の文字数に合わせて自動でサイズが決定されます。  
ver3.5.0より曲名表示が最大2行となり、カンマ区切り(もしくは$区切り)で2行目が指定できるようになりました。  

### タイトル曲名文字(デフォルトデザイン)の設定箇所について
![dos-h0030-01.png](./wiki/dos-h0030-01.png)

### 関連項目
- [**musicTitle**](dos-h0001-musicTitle.html) (*, ★)  楽曲／楽曲クレジット
- [**customTitleUse**](dos-h0025-customTitleUse.html)  タイトルの曲名文字
- [customTitleArrowUse](dos-h0026-customTitleArrowUse.html)  タイトルの背景矢印
- [**titlefont**](dos-h0031-titlefont.html)  フォント
- [titlegrd / titlearrowgrd](dos-h0032-titlegrd.html)  グラデーション
- [titlepos](dos-h0033-titlepos.html)  X, Y座標位置
- [**titlelineheight**](dos-h0034-titlelineheight.html)  複数行の際の行間

### 更新履歴

|Version|変更内容|
|----|----|
|[v17.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.3.0)|曲名表示の2行対応で$区切りにも対応|
|[v3.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.5.0)|曲名表示の2行対応。<br>カンマ区切りでそれぞれの行サイズを指定できるように変更|
|[v2.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v2.1.0)|初回実装|