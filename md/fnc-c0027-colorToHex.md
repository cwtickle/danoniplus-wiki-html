[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# colorToHex
### 概要
- 色名をカラーコードに変換する関数。
- `色名_位置;透明度` (例: red 20%;255) の形式のように色名以外の指定の仕方も可能。
- すでにカラーコードであったり、色名と関係のない値が入ってきた場合はそのままの値を返す。  
対象外のリストは `g_cssCheckStr` (danoni_constants.js)にて定義している。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_color|string|*|色名、もしくは`色名_位置;透明度`の形式指定|

### 返却値
- カラーコード（及び透明度、位置）

### 関連項目
- **colorToHex (_color)**
    - byteToHex (_num) ：透明度(10進)をカラーコード用の16進に変換
    - [colorNameToCode (_color)](fnc-c0040-colorNameToCode.html) ：Canvasに描画した色をカラーコードとして取得
- [checkLightOrDark (_colorStr)](fnc-c0041-checkLightOrDark.html)

### 使用例
```javascript
console.log(colorToHex(`red`));  // #ff0000
console.log(colorToHex(`red;128`));  // #ff000080
console.log(colorToHex(`red 20%;128`));  // #ff000080 20%
```
