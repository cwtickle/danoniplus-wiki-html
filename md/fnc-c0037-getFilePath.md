[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# getFilePath
### 概要
- 譜面ヘッダーで指定されたファイルパスを、キーワードとディレクトリに分割する関数。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_fileName|string|*|ファイルパス|
|_directory|string||デフォルトディレクトリ。既定は`(空)`。|

### 返却値
- [ファイルキーワード, 参照するルートディレクトリ]

### 使用例
```javascript
// カスタムjsの場合
console.log(getFilePath(`file.txt`, `../js/`)); // [`file.txt`, `../js/`] => ../js/file.txt
console.log(getFilePath(`(..)file.txt`, `../js/`)); // [`file.txt`, ``] => file.txt

// スキンの場合
console.log(getFilePath(`(..)light`, `../skin/`)); // [`light`, ``] => danoni_skin_light.css
console.log(getFilePath(`sub/blue`, `../skin/`)); // [`light`, `../skin/sub/`] => ../skin/sub/danoni_skin_blue.css
```

### 関連項目
- [**customjs**](dos-h0019-customjs.html)  カスタムjsファイルの指定
- [**skinType**](dos-h0054-skinType.html)  スキン設定
- [settingType](dos-h0056-settingType.html)  共通設定名
