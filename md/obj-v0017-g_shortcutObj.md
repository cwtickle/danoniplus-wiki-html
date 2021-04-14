[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_shortcutObj

### 概要
- ショートカットキーを管理するオブジェクト。
- ショートカットキーの割り当ては画面により異なるため、画面別にプロパティを持つ。
- 画面別プロパティは割り当てキー毎に、以下の項目を持っている。
  - プロパティ名 : `KeyBoardEvent.code`に従ったコードを指定。  
複数キーを組み合わせる場合は`_`で区切る。
  - id : 実行するボタンのID名を指定。
  - reset (任意) : 実行前にキーを押した状態を解除する場合は`true`を指定。
他のサイトへ移動する場合、onkeyupイベントが動かないためこの項目を設定している。

### 生成タイミング
- 初回起動時

### プロパティ
```javascript
const g_shortcutObj = {
    title: {
        Enter: { id: `btnStart` },
        Slash: { id: `btnHelp`, reset: true },
        F1: { id: `btnHelp`, reset: true },
        KeyC: { id: `btnComment` },
    },
    option: {
        ShiftLeft_KeyD: { id: `lnkDifficultyL` },
        KeyD: { id: `lnkDifficultyR` },
        ShiftLeft_ArrowRight: { id: `lnkSpeedR` },
        ArrowRight: { id: `lnkSpeedRR` },
        ShiftLeft_ArrowLeft: { id: `lnkSpeedL` },
        ArrowLeft: { id: `lnkSpeedLL` },
        KeyL: { id: `lnkDifficulty` },

        ShiftLeft_KeyM: { id: `lnkMotionL` },
        KeyM: { id: `lnkMotionR` },
        ArrowUp: { id: `btnReverse` },
        ShiftLeft_ArrowDown: { id: `lnkScrollL` },
        ArrowDown: { id: `lnkScrollR` },
        KeyR: { id: `lnkReverseR` },

        ShiftLeft_KeyS: { id: `lnkShuffleL` },
        KeyS: { id: `lnkShuffleR` },
        ShiftLeft_KeyA: { id: `lnkAutoPlayL` },
        KeyA: { id: `lnkAutoPlayR` },
        ShiftLeft_KeyG: { id: `lnkGaugeL` },
        KeyG: { id: `lnkGaugeR` },

        ShiftLeft_Semicolon: { id: `lnkAdjustmentR` },
        Semicolon: { id: `lnkAdjustmentRR` },
        ShiftLeft_Minus: { id: `lnkAdjustmentL` },
        Minus: { id: `lnkAdjustmentLL` },

        ShiftLeft_NumpadAdd: { id: `lnkAdjustmentR` },
        NumpadAdd: { id: `lnkAdjustmentRR` },
        ShiftLeft_NumpadSubtract: { id: `lnkAdjustmentL` },
        NumpadSubtract: { id: `lnkAdjustmentLL` },

        ShiftLeft_KeyV: { id: `lnkVolumeL` },
        KeyV: { id: `lnkVolumeR` },

        KeyI: { id: `btnGraph` },
        KeyQ: { id: `lnkScoreDetail` },
        KeyP: { id: `lnkDifInfo` },
        KeyZ: { id: `btnSave` },

        Escape: { id: `btnBack` },
        Space: { id: `btnKeyConfig` },
        Enter: { id: `btnPlay` },
        ShiftLeft_Tab: { id: `btnBack` },
        Tab: { id: `btnDisplay` },
    },
    difSelector: {
        ShiftLeft_KeyD: { id: `lnkDifficultyL` },
        KeyD: { id: `lnkDifficultyR` },
        KeyR: { id: `difRandom` },
        KeyL: { id: `lnkDifficulty` },
        ArrowDown: { id: `btnDifD` },
        ArrowUp: { id: `btnDifU` },

        Escape: { id: `btnBack` },
        Space: { id: `btnKeyConfig` },
        Enter: { id: `lnkDifficulty` },
        ShiftLeft_Tab: { id: `btnBack` },
        Tab: { id: `btnDisplay` },
    },
    settingsDisplay: {
        ShiftLeft_KeyA: { id: `lnkAppearanceL` },
        KeyA: { id: `lnkAppearanceR` },
        ShiftLeft_KeyO: { id: `lnkOpacityL` },
        KeyO: { id: `lnkOpacityR` },

        Digit1: { id: `lnkstepZone` },
        Digit2: { id: `lnkjudgment` },
        Digit3: { id: `lnkfastSlow` },
        Digit4: { id: `lnklifeGauge` },
        Digit5: { id: `lnkscore` },
        Digit6: { id: `lnkmusicInfo` },
        Digit7: { id: `lnkfilterLine` },
        Digit8: { id: `lnkspeed` },
        Digit9: { id: `lnkcolor` },
        Digit0: { id: `lnklyrics` },
        Semicolon: { id: `lnkbackground` },
        Minus: { id: `lnkarrowEffect` },
        Slash: { id: `lnkspecial` },

        Numpad1: { id: `lnkstepZone` },
        Numpad2: { id: `lnkjudgment` },
        Numpad3: { id: `lnkfastSlow` },
        Numpad4: { id: `lnklifeGauge` },
        Numpad5: { id: `lnkscore` },
        Numpad6: { id: `lnkmusicInfo` },
        Numpad7: { id: `lnkfilterLine` },
        Numpad8: { id: `lnkspeed` },
        Numpad9: { id: `lnkcolor` },
        Numpad0: { id: `lnklyrics` },
        NumpadAdd: { id: `lnkbackground` },
        NumpadSubtract: { id: `lnkarrowEffect` },
        NumpadDivide: { id: `lnkspecial` },

        Escape: { id: `btnBack` },
        Space: { id: `btnKeyConfig` },
        Enter: { id: `btnPlay` },
        ShiftLeft_Tab: { id: `btnBack` },
        Tab: { id: `btnSettings` },
    },
    keyConfig: {
        Escape: { id: `btnBack` },
    },
    loadingIos: {
        Enter: { id: `btnPlay` },
    },
    result: {
        Escape: { id: `btnBack` },
        ShiftLeft_Tab: { id: `btnBack` },
        KeyC: { id: `btnCopy`, reset: true },
        KeyT: { id: `btnTweet`, reset: true },
        KeyG: { id: `btnGitter`, reset: true },
        Backspace: { id: `btnRetry` },
    },
};
```

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.0.0)|・譜面セレクター（子画面）のショートカットキーを割り当て|
|[v20.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v20.4.0)|・タイトル画面のヘルプ、コメント画面開閉ボタンに対応するキーを割り当て<br>・loadingIos項目を追加(iOS系専用開始待ち画面)|
|[v20.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v20.2.0)|・キーコンフィグ画面以外の戻るボタンにShift+Tabを追加で割り当て|
|[v20.1.2](https://github.com/cwtickle/danoniplus/releases/tag/v20.1.2)|・Adjustment設定にテンキーの「+」「-」を追加で割り当て|
|[v19.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.5.0)|・初回実装|