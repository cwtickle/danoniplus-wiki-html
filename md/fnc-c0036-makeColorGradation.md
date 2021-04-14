[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# makeColorGradation
### 概要
- グラデーション指定されたカラーコードとパラメータを元に、  
CSSが認識できるグラデーション表記に変換する関数。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_colorStr|string|*|グラデーション指定されたカラーコード|
|----|object||※下記のオブジェクト引数を参照|

### オブジェクト引数
- オブジェクト引数は全て任意。指定が無い場合はデフォルト値が採用される。

|引数|型|デフォルト|用途|
|----|----|----|----|
|_defaultColorgrd|boolean|g_headerObj. defaultColorgrd|デフォルトグラデーション設定|
|_colorCdPaddingUse|boolean|false|カラーコードの前パディング可否|
|_objType|string|normal|オブジェクトの種類<br>(normal: 汎用, titleMusic: タイトル曲名, titleArrow: タイトル矢印)|
|_shadowFlg|boolean|false|デフォルト透明化するかどうかのフラグ|

### 返却値
- CSSが認識できるグラデーション表記

### 使用例
```javascript
console.log(makeColorGradation(`#6666ff:#9999ff`)); // linear-gradient(to right #6666ff #9999ff)
console.log(makeColorGradation(`#6666ff:#9999ff@conic-gradient`)); // conic-gradient(#6666ff #9999ff)
```

### 関連項目
- [グラデーション仕様](dos-c0001-gradation.html)
