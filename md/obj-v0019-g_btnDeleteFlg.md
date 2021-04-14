[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_btnDeleteFlg / g_cxtDeleteFlg

### 概要
- ボタンの既定処理を削除するかどうかを管理するオブジェクト。
- `g_btnDeleteFlg`はボタン左クリック時、`g_cxtDeleteFlg`はボタン右クリック時を指す。  
- `g_btnDeleteFlg.[ボタンid名]` もしくは `g_cxtDeleteFlg.[ボタンid名]`の形式で指定する。
それぞれ、値を`true`にすることで既定処理が削除される。未指定時は`false`(既定処理有効)扱い。
- 通常、[**g_btnAddFunc** / **g_cxtAddFunc**](obj-v0018-g_btnAddFunc.html)とセットで使用することを想定している。

```javascript
function customTitleInit() {
    g_btnDeleteFlg.btnStart = true;  // g_btnDeleteFlg.(ボタンID) = true でボタンIDが行っている処理をやめる
    g_btnAddFunc.btnStart = evt => {
        evt.target.style.background = `#9999ff`; // evt.targetでボタン本体に対する処理を記述できる
        commentInit(); // g_btnAddFunc.(ボタンID) に関数を定義することでその処理を後から挿入
    };

    g_cxtDeleteFlg.btnStart = true;  // g_cxtDeleteFlg.(ボタンID) = true でボタンIDが行っている処理をやめる
    g_cxtAddFunc.btnStart = evt => {
        commentInit(); // g_cxtAddFunc.(ボタンID) に関数を定義することでその処理を後から挿入
    };
}
```

### 生成タイミング
- 初回起動時

### プロパティ
- (固定で指定されているものは初期では無し)

### 関連項目
- [createCss2Button](fnc-c0004-createCss2Button.html)
- [commonKeyDown](fnc-c0007-commonKeyDown.html)
- [**g_btnAddFunc** / **g_cxtAddFunc**](obj-v0018-g_btnAddFunc.html)
