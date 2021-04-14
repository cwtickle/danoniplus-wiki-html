[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_scViewObj
### 概要
- ショートカット表示部分のデフォルト位置に関するオブジェクト。
- 設定画面の各種設定変更ボタンに対応するショートカット表示部分の位置に関する設定をまとめて行う。
- formatはショートカット表示方法を指定。  
デフォルトは`{0})`で、`{0}`の部分が実際のショートカット表示に置き換わる。  
例えば割り当てキーが`F`の場合、`F)`と表示される。

### 生成タイミング
- 初回起動時

### 補足
- ショートカットキーを対応付ける場合は、`g_shortcutObj`で別途定義が必要。
- ショートカットに対応したキーを表示する関数は`createScText`で行っている。

### プロパティ
```javascript
const g_scViewObj = {
    x: 95,
    y: 0,
    w: 40,
    siz: 12,
    format: `{0})`,
};
```

### 関連項目
- [**g_shortcutObj**](obj-v0017-g_shortcutObj.html)
- [g_btnPatterns](obj-v0021-g_btnPatterns.html)

### 更新履歴

|Version|変更内容|
|----|----|
|[v20.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v20.2.1)|・初回実装|