[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_loadObj

### 概要
- 外部ファイルの読み込み状態を表すオブジェクト。  
譜面ファイル名をプロパティに持ち、  
`true`であればプロパティで指定した名前のファイルが読み込めていることを表す。  
`loadScript ()`でのみ使用。
```javascript
g_loadObj[`score.txt`] = true;
```

### 生成タイミング
- `loadScript ()`呼び出し時（ファイルの読み込み）

### プロパティと生成値
- main (boolean): true
