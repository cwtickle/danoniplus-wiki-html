[← 譜面ヘッダー仕様に戻る](dos_header.html)  
[← 譜面エフェクト仕様に戻る](dos_effect.html)  
## グラデーション仕様（共通）

### 使い方
<pre>
|setColor=<b>#99ff66:#66ff99</b>,#9999ff,#ffffff,#ff9999,#ffff99|
|titlegrd=<b>#ffff99:#ff9999@radial-gradient</b>|
|color_data=
300,20,<b>45deg:#ffff99:#ffffff:#9999ff</b>
400,20,<b>#ffff99:#ffffff:#9999ff@radial-gradient</b>
500,20,<b>#ffff99:#ffffff:#9999ff@conic-gradient</b>
600,20,<b>blue:red</b>
700,20,<b>blue;100:orange;255:red;255</b>
|
</pre>

### 記述仕様
```
グラデーション記述(コロン区切りで記述)@グラデーションの種類
```
- グラデーション種類を省略した場合：linear-gradient が指定されます。
- linear-gradient でグラデーション方向を省略した場合：to rightが指定されます。
- 矢印色1種類を指定した場合：グラデーションのない単色になります。
（実際はlinear-gradientで開始色と終了色が同じ）

### 使用できるグラデーションの種類

|種類|グラデーションの方法・記述仕様|
|----|----|
|linear-<br>gradient|線形のグラデーション。指定が無い場合のデフォルトです。<br>`(グラデーション方向):(カラーコード1):(カラーコード2)...` のように指定します。<br>グラデーション方向は省略可能で、省略した場合は「to right」です。|
|radial-<br>gradient|放射グラデーション(中心から放射)。<br>`(カラーコード1):(カラーコード2)...` のように指定します。|
|conic-<br>gradient|放射グラデーション(中心点の周りを回りながら色が変化)。<br>`(カラーコード1):(カラーコード2)...` のように指定します。|

### 補足
- `linear-gradient`及び`repeating-linear-gradient`のグラデーションの方向を変えたい場合は、先頭に「45deg」「to top right」などをつけることで変更することができます。  
- カラーコード指定が原則です。色名指定も可能ですが、  
意図しない動きになることがありますのでご注意ください。  
   - ver14.1.0より、色名指定に対応しました。  
ただし、環境により色味が変わる可能性があるためご注意ください。
   - ver19.2.0より、色名に対して透明度を指定できるようになりました。  
`色名;透明度(0～255)`のように指定してください。

#### 参考：色名とカラーコードの対応表
https://www.colordic.org/  
https://www.webcreatorbox.com/webinfo/color-name

#### 参考：グラデーション詳細
- カンマになっている部分はコロンに置き換えてください。基本そのまま使用できます。  
現状、グラデーションの重ね合わせのみ未対応です。  

https://developer.mozilla.org/ja/docs/Web/CSS/linear-gradient()  
https://developer.mozilla.org/ja/docs/Web/CSS/CSS_Images/Using_CSS_gradients

### 関連項目
- [**setColor**](dos-h0003-setColor.html) (*, ★)  矢印色
- [**frzColor**](dos-h0004-frzColor.html) (*, ★)  フリーズアロー色
- [titlegrd / titlearrowgrd](dos-h0032-titlegrd.html)  グラデーション
- [色変化 (acolor_data, color_data)](dos-e0002-colorData.html)(★)  

### 更新履歴

|Version|変更内容|
|----|----|
|[v19.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.2.0)|・色名指定時、透明度を指定できるように変更|
|[v14.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v14.1.0)|・色名指定に対応|
|[v12.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.0.0)|・初期実装|
