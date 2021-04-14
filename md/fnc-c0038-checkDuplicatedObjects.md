[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# checkDuplicatedObjects
### 概要
- 多重配列の存在をチェックし、存在しない場合は作成、  
存在する場合は重複を避けて配列を新規作成する関数。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_obj|array|*|配列データ|

### 返却値
- [配列データ, 配列長]

### 使用例
```javascript
spriteData[180] = [[1, 2]];
[spriteData[180], dataLength] = checkDuplicatedObjects(spriteData[180]); 
// spriteData[180] = [[1, 2], []]
// dataLength = 2
```
