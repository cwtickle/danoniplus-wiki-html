[← 譜面ヘッダー仕様に戻る](dos_header.html)
## setColor (*)

### 使い方
```
|setColor=#9999ff,#ccffff,#ffffff,#ffff99,#ff9966|
|setColor=#ffcccc:#ffffff@radial-gradient,#ff9999:#ffff99@conic-gradient,#ffffff,#ffff99,#ff9966|
|setColor2=#ff9999,#ccffff,#ffffff,#ffff99,#ff9966| // 2譜面目
|setColor3=#ff9999,#ccffff,#ffffff,#ffff99,#ff9966| // 3譜面目
```
### 説明
矢印色を指定します。指定の仕方は、「#ffffff」もしくは「0xffffff」の形式です。  
カンマ区切りで5つの色を指定すると、キー数によって自動で色を振り分けてくれます。  
(ランダムではなく、キー数によって決まっています)  
また、ver12以降[コロン(:)区切りによるグラデーション](dos-c0001-gradation.html)に対応しています。

### 補足1：省略時の色補完について
- ver13より下記のように色補完を行います。
```
|setColor=#ff9999|                   (1)のみ     ⇒ すべて(1)で埋める
   -> #ffff99,#ffff99,#ffff99,#ffff99,#ffff99
|setColor=#ff3333,#99ffff|           (1),(2)     ⇒ (1),(2)の繰り返し
   -> #ff3333,#99ffff,#ff3333,#99ffff,#ff3333
|setColor=#ff3333,#99ffff,#ffffff|   (1),(2),(3) ⇒ (1),(2),(3)の繰り返し
   -> #ff3333,#99ffff,#ffffff,#ff3333,#99ffff
```

### 補足2：2譜面目以降の個別設定について
- ver21より2譜面目以降の個別設定が行えるようになりました。  
setColor2, setColor3, ... のように指定します。使い方はsetColorと同じです。  
未指定時はこれまで通り、setColorの値が採用されます。

### 参考：setColorで割り当てられた色について
- 割り当て色は、キーコンフィグ画面で確認できます。

![dos-h0003-01.png](./wiki/dos-h0003-01.png)

### 関連項目
- [colorCdPaddingUse](dos-h0047-colorCdPaddingUse.html)  初期矢印色/フリーズアロー色のゼロパディング有無設定
- [**frzColor**](dos-h0004-frzColor.html) (*, ★)  フリーズアロー色
- [setShadowColor](dos-h0041-setShadowColor.html)  矢印の内側を塗りつぶす設定および色の設定
- [defaultColorgrd](dos-h0061-defaultColorgrd.html)  自動グラデーション設定
- [titlegrd / titlearrowgrd](dos-h0032-titlegrd.html)  タイトルグラデーション
- [色変化 (acolor_data, color_data)](dos-e0002-colorData.html)(★)  
- [グラデーション仕様](dos-c0001-gradation.html) 

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.1.0)|・2譜面目以降の個別設定に対応（譜面分割＆譜面番号可変時）|
|[v21.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.0.0)|・2譜面目以降の個別設定に対応|
|[v13.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v13.0.0)|・省略時の色補完仕様を変更|
|[v12.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.0.0)|・グラデーション記述に対応|
|[v1.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|・初回実装|