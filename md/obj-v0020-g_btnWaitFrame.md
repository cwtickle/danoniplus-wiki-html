[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_btnWaitFrame
### 概要
- ボタン及びショートカットキーが有効化するまでのフレーム数を管理するオブジェクト。
- 画面別にプロパティを持つ。
- 画面別プロパティは割り当てキー毎に、以下の項目を持っている。
  - `b_frame` : ボタンが有効化するまでのフレーム数
  - `s_frame` : ショートカットキーが有効化するまでのフレーム数
  - `initial` : `true`にすると2回目以降はすぐに利用できるようになる。  
`g_initialFlg`を利用しており、タイトル画面及び設定画面でのみ使用できる。

### 生成タイミング
- 初回起動時

### プロパティ
```javascript
const g_btnWaitFrame = {
    initial: { b_frame: 0, s_frame: 0 },
    title: { b_frame: 0, s_frame: 0 },
    option: { b_frame: 0, s_frame: 0, initial: true },
    settingsDisplay: { b_frame: 0, s_frame: 0 },
    keyConfig: { b_frame: 0, s_frame: 30 },
    loading: { b_frame: 0, s_frame: 0 },
    loadingIos: { b_frame: 0, s_frame: 0 },
    main: { b_frame: 0, s_frame: 0 },
    result: { b_frame: 0, s_frame: 120 },
};
```

### 利用例
- 以下のような使い方を想定しています。

1. 画面が完全に表示された後にボタンとショートカットキーを同時に有効化
```javascript
g_btnWaitFrame.title.b_frame = 200;
g_btnWaitFrame.title.s_frame = 200;
```

2. 設定画面に属するボタンで、通常と時間差をつけて有効化  
※カスタム側の方の有効化時間を通常より長くする必要があります。

実際には、既存グループ（通常）のボタンと同じタイミングでボタンが作成されますが、  
カスタムの方が有効化時間が長いため、その分使用できるまでの時間が掛かるようになります。
```javascript
// 既存グループ（通常）のボタン・ショートカットキーフレーム数を変更
g_btnWaitFrame.option = { b_frame: 100, s_frame: 100, initial : true };
// 新しいグループ名（カスタム）に対してボタン・ショートカットキーフレーム数を長めに指定
g_btnWaitFrame.optionNext = { b_frame: 200, s_frame: 200, initial : true };

// カスタムボタンの追加
multiAppend(optionsprite, 
    createCss2Button(`btnNew`, `NewButton`, _ => { /* ボタン処理 */ }, {
         /* ボタンの位置に関する設定 */
         groupName: `optionNext`, // 先ほどつけたグループ名を定義
    })
);
```

### 更新履歴

|Version|変更内容|
|----|----|
|[v20.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v20.4.0)|・keyConfig.s_frameの初期値変更(0->30)<br>・loadingIos項目を追加(iOS系専用開始待ち画面)|
|[v20.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v20.2.0)|・初回実装|