[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# toCapitalize
### 概要
- 文字列の頭文字を英大文字に変換して返却する関数。
- 変数の多くがキャメル表記を行っている関係で、結合時に頭文字を英大文字にして結合することが多く、そのためにこの関数を使用している。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_str|string|*|任意の文字列|

### 返却値
- 頭文字を英大文字に変換した文字列

### 使用例
```javascript
console.log(toCapitalize(`option`));  // Option
console.log(toCapitalize(`keyConfig`));  // KeyConfig
```
