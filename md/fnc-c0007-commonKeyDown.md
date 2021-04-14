[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# commonKeyDown
### 概要
  - キーを押したときの動作を定義。
  - [g_shortcutObj](obj-v0017-g_shortcutObj.html)より対象画面のショートカットリストを取得し、  
対象キーに合致していれば、その処理を実行する。
  - ショートカット処理とは別に実行したい内容を`_func`内で定義することも可能。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_evt|object|*|イベントオブジェクト|
|_displayName|string|*|画面名(`g_shortcutObj`で定義したプロパティ名)|
|_func|function||後続処理（任意）|

### 返却値
- イベントの真偽値 (イベント実行時は`true`, キャンセルする場合は`false`)

### 使用例
```javascript
// この部分の既定値は danoni_constants.js で定義
// 拡張が必要な場合、danoni_settings.js などで定義することもできる
const g_shortcutObj = {
    keyConfig: {
        Escape: { id: `btnBack` },
    },
};

// この場合は g_shortcutObj.keyConfig が対象
// Escapeキーが押されたら、id: btnBackのボタンを実行する
document.onkeydown = evt => commonKeyDown(evt, `keyConfig`, setCode => {
  // ショートカット以外の独自処理
};
```

### 関連項目
- [createCss2Button](fnc-c0004-createCss2Button.html)
- [**g_btnAddFunc** / **g_cxtAddFunc**](obj-v0018-g_btnAddFunc.html)
- [**g_btnDeleteFlg** / **g_cxtDeleteFlg**](obj-v0019-g_btnDeleteFlg.html)

### 更新履歴

|Version|変更内容|
|----|----|
|[v19.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.5.0)|・初回実装|