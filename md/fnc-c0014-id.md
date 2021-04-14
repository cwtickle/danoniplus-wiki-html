[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# $id
### 概要
- idのついているオブジェクトのCSSのstyleを返却する関数。
- これだけで何かをするのではなく、記述の簡易化のために使用する。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_id|*|オブジェクトのID名|


### 返却値
- オブジェクトのCSSのstyle

### 使用例
```javascript
g_stateObj.scoreDetail = `ToolDif`;
$id(`detail${g_stateObj.scoreDetail}`).visibility = `visible`;
```
