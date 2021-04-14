[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# loadScript
### 概要
- 外部jsファイルを読み込む関数。
読み込みが必須ではない場合は`_requireFlg`に`false`を指定することで  
その後の処理を続行できる。
- 読み込みに成功した場合、g_loadObj[ファイル名]に`true`を返し、失敗した場合は`false`を返す。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_url|string|*|読込対象のjsファイル|
|_callback|function|*|読込後に実行するコールバック関数|
|_requiredFlg|boolean||読込必須フラグ。デフォルトは`true`(必須)。<br>`true`の場合、読込失敗時に処理を止める。<br>`false`にした場合、読込に失敗してもコールバック関数を実行する。|
|_charset|string||_urlで指定したファイルの文字コード。デフォルトは`UTF-8`。|


### 返却値
- なし

### 使用例
```javascript
const filename = `test.js`;
const randTime = new Date().getTime();
loadScript(`${filename}?${randTime}`, _ => {
    // 読込後の処理
}, false);
```

### 関連項目
- [g_loadObj](obj-v0006-g_loadObj.html)
- [importCssFile](fnc-c0020-importCssFile.html)

### 更新履歴

|Version|変更内容|
|----|----|
|[v12.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.0.0)|・読込状態（g_loadObj）のフラグを追加|
|[v10.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v10.0.0)|・読込失敗時の継続処理を追加|
|[v1.0.0<br>(v0.40.x)](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|・初回実装|
