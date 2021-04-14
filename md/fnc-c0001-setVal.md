[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# setVal

### 概要
- 変数の中身の型をチェックし、指定された型に変換する。
- 不適切な値の場合は、デフォルト値を返却する。
- undefinedやNaN、空白など、扱いにくい変数が入りそうなときにチェックを兼ねて使用する。

### 引数

|引数|型|内容|
|----|----|----|
|_checkStr|string|型チェック対象の変数|
|_default|string|型チェックがNGの場合のデフォルト値|
|_type|string|チェックする型|

### 返却値
- _checkStrを指定された型に変換した値 (変換できない場合は _defaultStr を返却)

### 使用例
```javascript
const checkStr = "abc123";
const returnStr1 = setVal(checkStr, "a", "string");  // abc123
const returnStr2 = setVal(checkStr, 0, "number");    // 0
```

### 関数詳細
#### チェック可能な型

|型|型名|備考|
|----|----|----|
|float|小数||
|number|整数||
|boolean|真偽値|false, true|
|switch|スイッチ|ON, OFF|
|calc|数式|数式として解釈した結果を計算|
|string|文字列||