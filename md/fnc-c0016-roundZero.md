[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# roundZero
### 概要
- 0未満の数字に対して0に変換する関数。
- 0未満の数字に対して別の値を指定することもできる。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_num|number|*|数字|
|_init|number||_numが0未満のときに適用する値を指定。デフォルトは0。|

### 返却値
- 変換後の数字（0以上の場合は_numの値をそのまま返却する）

### 使用例
```javascript
console.log(roundZero(7));  // 7
console.log(roundZero(0));  // 0
console.log(roundZero(-5));  // 0
console.log(roundZero(-2, -1));  // -1
```
