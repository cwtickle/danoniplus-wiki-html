[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# colorNameToCode
### 概要
- 色名やRGB形式(`rgb(225, 225, 225)`など)をカラーコードに変換する関数。
- Canvasに描画した色をカラーコードとして取得している。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_color|string|*|色名、RGB形式などの色|

### 返却値
- カラーコード

### 関連項目
- [colorToHex (_color)](fnc-c0027-colorToHex.html)
    - byteToHex (_num) ：透明度(10進)をカラーコード用の16進に変換
    - **colorNameToCode (_color)** ：Canvasに描画した色をカラーコードとして取得
- [checkLightOrDark (_colorStr)](fnc-c0041-checkLightOrDark.html)

### 使用例
```javascript
console.log(colorNameToCode(`red`));  // #ff0000
console.log(colorNameToCode(`rgb(0, 255, 0)`));  // #00ff00
```
