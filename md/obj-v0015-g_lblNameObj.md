[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_lblNameObj / g_local_lblNameObj

### 概要
- ラベル全般を管理するオブジェクト。
- `g_local_lblNameObj`は`g_lblNameObj`のローカル版で、  
`g_local_lblNameObj`側のプロパティが優先される設定になっている。
- どこにマッピングされるかについては、[ID一覧](IdReferenceIndex.html)を参照。

### 生成タイミング
- 初回起動時

### プロパティ

#### ページタイトル
```javascript
{
    dancing: `DANCING`,
    star: `☆`,
    onigiri: `ONIGIRI`,
    settings: `SETTINGS`,
    display: `DISPLAY`,
    key: `KEY`,
    config: `CONFIG`,
    result: `RESULT`,
}
```

#### 補足メッセージ
```javascript
{
    kcDesc: `[{0}:スキップ / {1}:(代替キーのみ)キー無効化]`,
    sdDesc: `[クリックでON/OFFを切替、灰色でOFF]`,
    kcShortcutDesc: `プレイ中ショートカット：「{0}」タイトルバック / 「{1}」リトライ`,
    transKeyDesc: `別キーモードではハイスコア、キーコンフィグ等は保存されません`,
    sdShortcutDesc: `Hid+/Sud+時ショートカット：「pageUp」カバーを上へ / 「pageDown」下へ`,
}
```

#### 固定ボタン
```javascript
{
    maker: `Maker`,
    artist: `Artist`,

    dataReset: `Data Reset`,
    dataSave: `Data Save`,
    clickHere: `Click Here!!`,
    comment: `Comment`,
}
```

#### ロード時表示部分
```javascript
{
    nowLoading: `Now Loading...`,
    pleaseWait: `Please Wait...`,
}
```

#### 画面移動系ボタン
```javascript
{
    b_back: `Back`,
    b_keyConfig: `KeyConfig`,
    b_play: `PLAY!`,
    b_reset: `Reset`,
    b_settings: `To Settings`,
    b_copy: `CopyResult`,
    b_tweet: `Tweet`,
    b_gitter: `Gitter`,
    b_retry: `Retry`,
}
```

#### 設定画面（ラベル）
```javascript
{
    Difficulty: `Difficulty`,
    Speed: `Speed`,
    Motion: `Motion`,
    Scroll: `Scroll`,
    Reverse: `Reverse`,
    Shuffle: `Shuffle`,
    AutoPlay: `AutoPlay`,
    Gauge: `Gauge`,
    Adjustment: `Adjustment`,
    Fadein: `Fadein`,
    Volume: `Volume`,

    multi: `x`,
    percent: `%`,
}
```

#### 設定画面（ショートカット表示）
```javascript
{
    sc_speed: `←→`,
    sc_scroll: `↑/↓`,
    sc_adjustment: `- +`,
}
```

#### 設定画面（ゲージ詳細表示）
```javascript
{
    g_start: `Start`,
    g_border: `Border`,
    g_recovery: `Recovery`,
    g_damage: `Damage`,
}
```

#### 設定画面（速度・密度グラフ、ツール値表示）
```javascript
{
    s_speed: `Speed`,
    s_boost: `Boost`,
    s_apm: `APM`,
    s_time: `Time`,
    s_arrow: `Arrow`,
    s_frz: `Frz`,

    s_level: `Level`,
    s_douji: `同時補正`,
    s_tate: `縦連補正`,
    s_cnts: `All Arrows`,
    s_linecnts: `- 矢印 Arrow:<br><br>- 氷矢 Frz:<br><br>- 3つ押し位置 ({0}):`,
    s_print: `データ出力`,
    s_printTitle: `Dancing☆Onigiri レベル計算ツール+++`,
    s_printHeader: `難易度\t同時\t縦連\t総数\t矢印\t氷矢印\tAPM\t時間`,
}
```

#### 設定画面（Display画面）
```javascript
{
    d_StepZone: `StepZone`,
    d_Judgment: `Judgment`,
    d_FastSlow: `FastSlow`,
    d_LifeGauge: `LifeGauge`,
    d_Score: `Score`,
    d_MusicInfo: `MusicInfo`,
    d_FilterLine: `FilterLine`,
    d_Speed: `Speed`,
    d_Color: `Color`,
    d_Lyrics: `Lyrics`,
    d_Background: `Background`,
    d_ArrowEffect: `ArrowEffect`,
    d_Special: `Special`,

    Appearance: `Appearance`,
    Opacity: `Opacity`,
}
```

#### 各種設定項目
```javascript
{
    'u_x': `x`,
    'u_%': `%`,

    'u_OFF': `OFF`,
    'u_ON': `ON`,
    'u_Boost': `Boost`,
    'u_Brake': `Brake`,

    'u_Cross': `Cross`,
    'u_Split': `Split`,
    'u_Alternate': `Alternate`,
    'u_Twist': `Twist`,
    'u_Asymmetry': `Asymmetry`,
    'u_Flat': `Flat`,
    'u_R-': `R-`,
    'u_Reverse': `Reverse`,

    'u_Mirror': `Mirror`,
    'u_Random': `Random`,
    'u_Random+': `Random+`,
    'u_S-Random': `S-Random`,
    'u_S-Random+': `S-Random+`,

    'u_ALL': `ALL`,
    'u_Onigiri': `Onigiri`,
    'u_Left': `Left`,
    'u_Right': `Right`,

    'u_Original': `Original`,
    'u_Heavy': `Heavy`,
    'u_NoRecovery': `NoRecovery`,
    'u_SuddenDeath': `SuddenDeath`,
    'u_Practice': `Practice`,
    'u_Light': `Light`,

    'u_Normal': `Normal`,
    'u_Hard': `Hard`,
    'u_Easy': `Easy`,

    'u_Visible': `Visible`,
    'u_Hidden': `Hidden`,
    'u_Hidden+': `Hidden+`,
    'u_Sudden': `Sudden`,
    'u_Sudden+': `Sudden+`,
    'u_Hid&Sud+': `Hid&Sud+`,

    'u_Speed': `Speed`,
    'u_Density': `Density`,
    'u_ToolDif': `ToolDif`,

    'u_Main': `Main`,
    'u_Replaced': `Replaced`,

    'u_Default': `Default`,
    'u_Type0': `Type0`,
    'u_Type1': `Type1`,
    'u_Type2': `Type2`,
}
```

#### キーコンフィグ画面
```javascript
{
    ConfigType: `ConfigType`,
    ColorType: `ColorType`,
    KeyPattern: `KeyPattern`,
}
```

#### 判定キャラクタ、パーフェクト演出
```javascript
{
    j_ii: "(・∀・)ｲｲ!!",
    j_shakin: "(`・ω・)ｼｬｷﾝ",
    j_matari: "( ´∀`)ﾏﾀｰﾘ",
    j_shobon: "(´・ω・`)ｼｮﾎﾞｰﾝ",
    j_uwan: "( `Д´)ｳﾜｧﾝ!!",

    j_kita: "(ﾟ∀ﾟ)ｷﾀ-!!",
    j_iknai: "(・A・)ｲｸﾅｲ",

    j_maxCombo: `MaxCombo`,
    j_fmaxCombo: `FreezeCombo`,
    j_score: `Score`,

    j_fast: `Fast`,
    j_slow: `Slow`,

    allPerfect: `All Perfect!!`,
    perfect: `Perfect!!`,
    fullCombo: `FullCombo!`,
    cleared: `CLEARED!`,
    failed: `FAILED...`,
}
```

#### 結果画面（ラベル、略名表示）
```javascript
{
    rt_Music: `Music`,
    rt_Difficulty: `Difficulty`,
    rt_Style: `Playstyle`,
    rt_Display: `Display`,

    rd_StepZone: `Step`,
    rd_Judgment: `Judge`,
    rd_FastSlow: `FS`,
    rd_LifeGauge: `Life`,
    rd_Score: `Score`,
    rd_MusicInfo: `MusicInfo`,
    rd_FilterLine: `Filter`,
    rd_Speed: `Speed`,
    rd_Color: `Color`,
    rd_Lyrics: `Lyrics`,
    rd_Background: `Back`,
    rd_ArrowEffect: `Effect`,
    rd_Special: `SP`,
}
```

### 更新履歴

|Version|変更内容|
|----|----|
|[v20.3.1](https://github.com/cwtickle/danoniplus/releases/tag/v20.3.1)|・各種設定項目、結果画面（ラベル、略名表示）を追加|
|[v19.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.3.0)|・初回実装|