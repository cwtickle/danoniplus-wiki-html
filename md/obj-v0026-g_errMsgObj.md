[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_errMsgObj

### 概要
- 警告/メッセージウィンドウに表示するメッセージを画面ごとに管理するオブジェクト。
- 表示メッセージを配列で管理している。
- [makeWarningWindow](fnc-c0013-makeWarningWindow.html) にて利用される。

### 生成タイミング
- 初回起動時

### 格納イメージ
```javascript
g_errMsgObj.title = [
`お使いのブラウザは動作保証外です。<br>
 Chrome/Opera/Vivaldiなど、WebKit系ブラウザの利用を推奨します。(W-0001)`,
`fileスキームでの動作のため、内蔵の画像データを使用します。(W-0011)<br>
 imgフォルダ以下の画像の変更は適用されません。`
];
```

### プロパティ
```javascript
const g_errMsgObj = {
    title: [],
    option: [],
    settingsDisplay: [],
    loading: [],
    main: [],
    result: [],
};
```

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.3.0)|・プロパティ毎に配列化|
|[v21.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.2.0)|・初回実装|
