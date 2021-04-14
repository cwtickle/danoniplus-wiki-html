[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_settings
### 概要
- 設定画面で選択できるオプション名(キー名)と、  
各設定のカーソル位置を設定項目別に管理するオブジェクト。  
- オプション名についてはこの名前がそのまま表示されるのではなく、  
`g_lblNameObj.u_(オプション名)`に対応した名前が表示される。  
ただし、`g_lblNameObj`内に`g_settings`内で指定したオプション名が存在しない場合は、  
そのオプション名がそのまま画面表示される。

### 生成タイミング
- 初回起動時。
- ただし、以下のプロパティは動的に生成される。

|プロパティ名|ベースとなる変数など|
|----|----|
|speeds (速度)|[maxSpeed](dos-h0016-maxSpeed.html), [minSpeed](dos-h0015-minSpeed.html) (譜面ヘッダー)|
|scrolls (スクロール)|[g_keyObj.scrollNameX, g_keyObj.scrollDirX_Y](keys.html)|
|gauges (ゲージ設定)|[customGauge](dos-h0053-customGauge.html), [gaugeX](dos-h0022-gaugeX.html) (譜面ヘッダー), <br>[g_gaugeOptionObj](obj-v0007-g_gaugeOptionObj.html)|
|autoPlays (オートプレイ)|[g_keyObj.assistNameX, g_keyObj.assistPosX_Y](keys.html)|

### プロパティ
```javascript
const g_settings = {
    speeds: [...Array((C_MAX_SPEED - C_MIN_SPEED) * 4 + 1).keys()].map(i => C_MIN_SPEED + i / 4),
    speedNum: 0,

    motions: [C_FLG_OFF, `Boost`, `Brake`],
    motionNum: 0,

    reverses: [C_FLG_OFF, C_FLG_ON],
    reverseNum: 0,

    scrolls: [],
    scrollNum: 0,

    shuffles: [C_FLG_OFF, `Mirror`, `Random`, `Random+`, `S-Random`, `S-Random+`],
    shuffleNum: 0,

    gauges: [],
    gaugeNum: 0,

    autoPlays: [C_FLG_OFF, C_FLG_ALL],
    autoPlayNum: 0,

    adjustments: [...Array(C_MAX_ADJUSTMENT * 2 + 1).keys()].map(i => i - C_MAX_ADJUSTMENT),
    adjustmentNum: C_MAX_ADJUSTMENT,

    volumes: [0, 0.5, 1, 2, 5, 10, 25, 50, 75, 100],

    appearances: [`Visible`, `Hidden`, `Hidden+`, `Sudden`, `Sudden+`, `Hid&Sud+`],
    appearanceNum: 0,

    opacitys: [10, 25, 50, 75, 100],

    scoreDetails: [`Speed`, `Density`, `ToolDif`],
    scoreDetailNum: 0,
};

g_settings.volumeNum = g_settings.volumes.length - 1;
g_settings.opacityNum = g_settings.opacitys.length - 1;

```
