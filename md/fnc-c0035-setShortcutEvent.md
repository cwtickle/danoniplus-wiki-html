[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# setShortcutEvent
### 概要
- ショートカットキーを割り当て、実行を管理する関数。
- `document.onKeyDown`, `document.onKeyUp`の上書き処理を行う。  
上書き処理のタイミングは、[g_btnWaitFrame](obj-v0020-g_btnWaitFrame.html)を参照して、有効化時間経過後に反映する。  
反映するタイミングで画面の切り替えが発生した場合は、上書きしないようになっている。
- ショートカットキーに対応したボタン操作を定義するため、対象のボタンをこの関数が実行される前に定義しておく必要がある。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_displayName|string|*|画面名|
|_func|function||ショートカットキー処理後に実行するonKeyDown処理|

### 返却値
- なし

### 関数の依存関係
- **setShortcutEvent**
  - [createScTextCommon](fnc-c0034-createScTextCommon.html)
    - [createScText](fnc-c0008-createScText.html)
    - [g_btnPatterns](obj-v0021-g_btnPatterns.html)
  - [commonKeyDown](fnc-c0007-commonKeyDown.html)
    - [g_shortcutObj](obj-v0017-g_shortcutObj.html)
    - [keyIsDown](fnc-c0023-keyIsDown.html)
  - commonKeyUp

### 使用例
```javascript
setShortcutEvent(`title`);
```

### 関連項目
- [**g_shortcutObj**](obj-v0017-g_shortcutObj.html)
- [g_btnWaitFrame](obj-v0020-g_btnWaitFrame.html)
- [commonKeyDown](fnc-c0007-commonKeyDown.html)

### 更新履歴

|Version|変更内容|
|----|----|
|[v20.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v20.4.0)|・`createScTextCommon`関数を包含するよう変更|
|[v19.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.5.0)|・初回実装|