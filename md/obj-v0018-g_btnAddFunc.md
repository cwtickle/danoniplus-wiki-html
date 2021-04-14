[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_btnAddFunc / g_cxtAddFunc

### 概要
- ボタンの処理拡張を管理するオブジェクト。
- `g_btnAddFunc`はボタン左クリック時、`g_cxtAddFunc`はボタン右クリック時の処理拡張を表す。
- `g_btnAddFunc.[ボタンid名]` もしくは `g_cxtAddFunc.[ボタンid名]`の形式で指定する。  
ボタンの既定処理が行われた後、これらの変数が指定されていれば実行される。
- ボタンの既定処理をやめたい場合、これと合わせて[**g_btnDeleteFlg** / **g_cxtDeleteFlg**](obj-v0019-g_btnDeleteFlg.html)を使用する。

```javascript
function customTitleInit() {
    g_btnAddFunc.btnStart = (_evt, _func, _resetFunc) => {
        _evt.target.style.background = `#9999ff`; // evt.targetでボタン本体に対する処理を記述できる
        commentInit(); // g_btnAddFunc.(ボタンID) に関数を定義することでその処理を後から挿入
    };

    g_cxtAddFunc.btnStart = evt => {
        commentInit(); // g_cxtAddFunc.(ボタンID) に関数を定義することでその処理を後から挿入
    };
}
```

### 引数仕様
- _func, _resetFuncはv20からの仕様。

|引数|型|必須|指定内容|
|----|----|----|----|
|_evt|object||イベントオブジェクト。<br>`_evt.target`でボタン本体を指定できる。|
|_func|function||ボタン本体の処理。<br>処理中に`_func(_evt);`と指定することで<br>任意の箇所でボタン本体処理が実行できる。<br>g_btnDeleteFlg / g_cxtDeleteFlg でボタン処理を無効にした上での利用を想定。<br>主にボタン本体の処理より前にカスタム処理を挟みたい場合に利用。|
|_resetFunc|function||ボタン本体の処理のうち、画面移動を伴う処理。<br>処理中に`_resetFunc(_evt);`と指定することで<br>ボタン本体処理が実行できる。<br>g_btnDeleteFlg / g_cxtDeleteFlg でボタン処理を無効にした上での利用を想定。<br>通常は一番最後に指定する。|

### 生成タイミング
- 初回起動時

### プロパティ
- (固定で指定されているものは初期では無し)

### 関連項目
- [createCss2Button](fnc-c0004-createCss2Button.html)
- [commonKeyDown](fnc-c0007-commonKeyDown.html)
- [**g_btnDeleteFlg** / **g_cxtDeleteFlg**](obj-v0019-g_btnDeleteFlg.html)