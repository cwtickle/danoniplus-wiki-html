[← 譜面ヘッダー仕様に戻る](dos_header.html)
## titlegrd / titlearrowgrd

### 使い方
```
|titlegrd=#ff0000,#ff4500,#ffff00,#008000,#00ffff,#0000ff,#800080|
|titlegrd=to top right,#DDDD99,#ffff00|
|titlegrd=45deg,#DDDD99,#ffff00|
|titlegrd=0xffff99,0xffffff|
|titlegrd=180deg,#9999ff,#ffffff$180deg,#ffff66,#888888,#ff9999|
|titlegrd=90deg:#ffff99:#ffffff|
|titlearrowgrd=#ffff99:#ffffff@radial-gradient|
```
### 説明

|譜面ヘッダー|内容|
|----|----|
|titlegrd|曲名文字のグラデーション|
|titlearrowgrd|背景矢印のグラデーション|

デフォルトの曲名表示を使用した場合に、  
タイトル文字(背景矢印)のグラデーションを設定できます。  
カンマ区切りでいくつでも指定可能です。  
ver5.1以降は、$区切りで2行目のグラデーションを指定できます。  
ver12以降、[コロン(:)区切りによるグラデーション](dos-c0001-gradation.html)に対応しています。

指定がない場合は、これまで通りsetColorの1番目・3番目の値が適用されます。  
1つだけ色指定した場合、2つ目の色として#ffffffが自動補完されます。  

グラデーションの方向を変えたい場合は、先頭に「45deg」「to top right」などをつけることで  
変更することができます。  
カラーコード指定が原則です。色名指定も可能ですが、意図しない動きになることがありますのでご注意ください。  
(参考：Pull Request [#223](https://github.com/cwtickle/danoniplus/pull/223) )  

customTitleUseがfalseに設定されているとき、この値は無視されます。  

### タイトル曲名文字(デフォルトデザイン)の設定箇所について
![dos-h0030-01.png](./wiki/dos-h0030-01.png)

### 関連項目
- [**musicTitle**](dos-h0001-musicTitle.html) (*, ★)  楽曲／楽曲クレジット
- [defaultColorgrd](dos-h0061-defaultColorgrd.html)  自動グラデーション設定
- [**titlesize**](dos-h0030-titlesize.html)  文字サイズ
- [**titlefont**](dos-h0031-titlefont.html)  フォント
- [titlepos](dos-h0033-titlepos.html)  X, Y座標位置
- [**titlelineheight**](dos-h0034-titlelineheight.html)  複数行の際の行間
- [titleanimation](dos-h0077-titleanimation.html)  アニメーション設定
- [グラデーション仕様](dos-c0001-gradation.html) 

### 更新履歴

|Version|変更内容|
|----|----|
|[v19.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.2.0)|・titlearrowgrdについてRGBAのカラーコードに対応|
|[v12.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.0.0)|・グラデーション記述に対応|
|[v5.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v5.1.0)|・曲名表示の2行対応。<br>　"$"区切りでそれぞれのグラデーションを指定できるように変更|
|[v3.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.2.0)|・初回実装|