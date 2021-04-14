[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# getQueryParamVal
### 概要
- 現在URLのクエリパラメータから指定したキーに合致する値を取得する関数。  
取得できない場合は`null`を返す。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_name|string|*|指定したキー|

### 返却値
- 現在URLのクエリパラメータから引数に指定したキーに合致する値を返却する。  
取得できない場合は`null`を返す。

### 使用例
```javascript
// URLに ?dos=XXXX もしくは &dos=XXXX のような値が入っているかをチェック
if (getQueryParamVal(`dos`) !== null) {
    const queryDos = `dos/${getQueryParamVal('dos')}.txt`;
}
```
