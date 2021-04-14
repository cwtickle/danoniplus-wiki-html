[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_btnPatterns
### 概要
- ボタンに対するショートカットキーの表示場所を管理するオブジェクト。
- 画面別にプロパティを持つ。また、画面別のプロパティではさらに以下のプロパティを持つ。  
下記プロパティに対応するボタンのdiv要素の子要素に、ショートカットに対応したキーを左上に表示する。
    - プロパティ名 : ID名の`btnXXX`の`XXX`の部分を指定。
    - 値 : `X`座標の補正値

### 生成タイミング
- 初回起動時

### 補足
- ショートカットキーを対応付ける場合は、`g_shortcutObj`で別途定義が必要。
- ショートカットに対応したキーを表示する関数は [createScTextCommon](fnc-c0034-createScTextCommon.html) で行っている。

### プロパティ
```javascript
const g_btnPatterns = {
    title: { Start: 0 },
    option: { Back: 0, KeyConfig: 0, Play: 0, Display: -5, Save: -10, Graph: -25 },
    difSelector: {},
    settingsDisplay: { Back: 0, KeyConfig: 0, Play: 0, Save: -10, Settings: -5 },
    keyConfig: { Back: -3 },
    loadingIos: { Play: 0 },
    result: { Back: -5, Copy: -5, Tweet: -5, Gitter: -5, Retry: 0 },
};
```

### 関連項目
- [**g_shortcutObj**](obj-v0017-g_shortcutObj.html)
- [createScTextCommon](fnc-c0034-createScTextCommon.html)

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.2.0)|・Display画面にSave切替ボタンを追加|
|[v21.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.0.0)|・譜面セレクター表示時のプロパティを追加|
|[v20.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v20.4.0)|・loadingIos項目を追加(iOS系専用開始待ち画面)|
|[v19.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.5.0)|・初回実装|