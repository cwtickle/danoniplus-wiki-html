[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# hasVal
### 概要
- 変数(オブジェクトプロパティ)が`undefined`もしくは空文字で無いかをチェックする関数。
- 定義済みの変数・オブジェクトを_dataに指定する。
- 定義されていない変数はこの関数ではチェックできない。  
`if(typeof 変数名 === C_TYP_STRING)`のような記述が必要になる。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_data|string, object|*|任意のデータ|

### 返却値
- `undefined`もしくは空文字の場合は`false`。それ以外は`true`。

### 使用例
```javascript
const obj = {
    data: [1, 2, 3],
};
console.log(hasVal(obj));  // true
console.log(hasVal(obj.data));  // true
console.log(hasVal(obj.data2));  // false
```
