[← 譜面ヘッダー仕様に戻る](dos_header.html)
## frzColor (*)

### 使い方
```
|frzColor=#00ffff,#6600ff,#ffff66,#ffff66$#ff00ff,#ff6600,#ffff66,#ffff66|
|frzColor=#00ffff:#00ff00,#6600ff:#9900ff,#ffff66:#ffff99,#ffff66$#ff00ff,#ff6600,#ffff66,#ffff66|
|frzColor2=#00ffff,#6666ff,#ffffcc,#ffffcc$#ff00ff,#ff6600,#ffff66,#ffff66|
```
### 説明
フリーズアロー色を指定します。指定の仕方は、「#ffffff」もしくは「0xffffff」の形式です。  
4つ1セット(カンマ区切り)で、フリーズアローの「矢印(通常時)」「帯(通常時)」「矢印(ヒット時)」「帯(ヒット時)」を表します。  
さらに、"$"を続けて4つずつ記載することで、「setColor」に対応した矢印レーンごとに  
フリーズアロー色を変えることができます。  

ParaFlaではこういう場合、基本的には矢印色変化を行う必要がありましたが、  
「frzColor」で最初からある程度制御できるようになりました。 

また、ver12以降[コロン(:)区切りによるグラデーション](dos-c0001-gradation.html)に対応しています。 

### 補足1：省略時の色補完について
ver13より、[defaultFrzColorUse](dos-h0063-defaultFrzColorUse.html) を`false`に設定した場合は下記のように色補完を行います。  
デフォルトはこれまで通り、既定のフリーズアローセットから補完します。  

- 未指定の場合：  
`setColor`で指定されている色を「矢印(通常時)」「帯(通常時)」「矢印(ヒット時)」「帯(ヒット時)」に割り当てます。
- 部分省略した場合：  
先頭を省略した場合は`setColor`, 後続(ヒット部)を省略した場合は前2つを補完します。
```
|setColor=#9999ff|
|frzColor=,,#ffff33,#ffff99| -> #9999ff,#9999ff,#ffff33,#ffff99
|frzColor=#66ffff,#8888ff|   -> #66ffff,#8888ff,#66ffff,#8888ff
```

### 補足2：2譜面目以降の個別設定について
- ver21より2譜面目以降の個別設定が行えるようになりました。  
frzColor2, frzColor3, ... のように指定します。使い方はfrzColorと同じです。  
未指定時はこれまで通り、frzColorの値が採用されます。

### 関連項目
- [colorCdPaddingUse](dos-h0047-colorCdPaddingUse.html)  初期矢印色/フリーズアロー色のゼロパディング有無設定
- [**setColor**](dos-h0003-setColor.html) (*, ★)  矢印色
- [setShadowColor](dos-h0041-setShadowColor.html)  矢印の内側を塗りつぶす設定および色の設定
- [frzShadowColor](dos-h0062-frzShadowColor.html)  フリーズアローの矢印内側を塗りつぶす設定および色の設定
- [defaultColorgrd](dos-h0061-defaultColorgrd.html)  自動グラデーション設定
- [defaultFrzColorUse](dos-h0063-defaultFrzColorUse.html)  フリーズアロー初期色(frzColor)が未指定時の適用方法
- [titlegrd / titlearrowgrd](dos-h0032-titlegrd.html)  タイトルグラデーション
- [色変化 (acolor_data, color_data)](dos-e0002-colorData.html)(★)  
- [グラデーション仕様](dos-c0001-gradation.html) 

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.1.0)|・2譜面目以降の個別設定に対応（譜面分割＆譜面番号可変時）|
|[v21.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.0.0)|・2譜面目以降の個別設定に対応|
|[v13.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v13.0.0)|・省略時、setColorから色補完する仕様を追加|
|[v12.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.0.0)|・グラデーション記述に対応|
|[v1.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|・初回実装|