[← 譜面ヘッダー仕様に戻る](dos_header.html)
## titlefont
[ver2.x以降]

### 使い方
```
|titlefont=Century,Meiryo UI|
|titlefont=Century,Meiryo UI$Century Gothic,Meiryo UI|
```
### 説明
デフォルトの曲名表示を使用した場合に、曲名のフォントを指定します。  
カンマ区切りで複数のフォントを指定できます。前に設定したものが優先です。  
指定しない場合は、"メイリオ", sans-serifが自動指定されます。  
なおWebフォントを指定した場合、読込のラグで初回表示のみ、  
Webフォント以外のフォントが表示されます。  
（→ Ver3.2.0以降より、この事象は解消されました。）  

ver17.3.0より、$区切りで2行目限定のフォントが指定できるようになりました。

### タイトル曲名文字(デフォルトデザイン)の設定箇所について
![dos-h0030-01.png](./wiki/dos-h0030-01.png)

### 関連項目
- [**customFont**](dos-h0020-customFont.html)  画面全般のフォント
- [**titlesize**](dos-h0030-titlesize.html)  文字サイズ
- [titlegrd](dos-h0032-titlegrd.html)  グラデーション
- [titlepos](dos-h0033-titlepos.html)  X, Y座標位置
- [**titlelineheight**](dos-h0034-titlelineheight.html)  複数行の際の行間

### 更新履歴

|Version|変更内容|
|----|----|
|[v17.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.3.0)|・2行目のフォント設定を追加|
|[v2.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v2.1.0)|・初回実装|