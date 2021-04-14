[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# checkLightOrDark
### 概要
- 引数に渡されたカラーコードをRGB形式に分解し、それが明色か暗色かを区別する関数。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_colorStr|string|*|カラーコード|

### 返却値
- 真偽値 ( `true`: 明色, `false`: 暗色 )

### 関連項目
- [colorToHex (_color)](fnc-c0027-colorToHex.html)
- [colorNameToCode (_color)](fnc-c0040-colorNameToCode.html)

### 使用例
```javascript
console.log(checkLightOrDark(`#ffcccc`));  // true
console.log(checkLightOrDark(`#333366`));  // false
```

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.2.0)|・初回実装|