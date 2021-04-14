[← 譜面ヘッダー仕様に戻る](dos_header.html)
## frzShadowColor
### 使い方
```
|frzShadowColor=Default$Default$Default$Default$Default|
|frzShadowColor=#ffcccc:#ffffff@radial-gradient,#9999ff$...|
|frzShadowColor2=#666666|
```
### 説明
フリーズアローの矢印内側の塗りつぶし色に関する設定です。  
未指定の場合は強制的に「黒色」になります。  
2つ1セット(カンマ区切り)で、フリーズアローの「通常時」「ヒット時」を表します。  
さらに、"$"を続けて4つずつ記載することで、「setColor(setShadowColor)」に  
対応した矢印レーンごとにフリーズアローの塗りつぶし色を変えることができます。  

## 補足：省略時の色補完について
基本的には`frzColor`の色補完方法と同じです。
- 未指定の場合：  
`setShadowColor`で指定されている色を「通常時」「ヒット時」に割り当てます。

### 関連項目
- [**setColor**](dos-h0003-setColor.html) (*, ★)  矢印色
- [**frzColor**](dos-h0004-frzColor.html) (*, ★)  フリーズアロー色
- [setShadowColor](dos-h0041-setShadowColor.html)  矢印の内側を塗りつぶす設定および色の設定
- [グラデーション仕様](dos-c0001-gradation.html) 

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.1.0)|・2譜面目以降の個別設定に対応（譜面分割＆譜面番号可変時）|
|[v21.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.0.0)|・2譜面目以降の個別設定に対応|
|[v13.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v13.0.0)|・初回実装|