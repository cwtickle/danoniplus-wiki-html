# 共通設定ファイル仕様
- 作品の共通設定については`danoni_setting.js`で設定することができます。
- グループごとに共通設定を分けることが可能です。詳細は譜面ヘッダー：[settingType](dos-h0056-settingType.html)をご覧ください。
- 対応する譜面ヘッダーがある場合は、譜面ヘッダーの値が優先されます。

## 設定可能項目
### 譜面製作者名 (g_presetTuning)
⇒ 指定があった場合に優先される譜面ヘッダー：[tuning](dos-h0017-tuning.html)
- デフォルトの制作者名に指定する値を設定します。  
下記の譜面製作者URLと合わせて設定しておくと、譜面ヘッダー：[tuning](dos-h0017-tuning.html)を省略できます。
```javascript
const g_presetTuning = `name`;
```

### 譜面製作者URL (g_presetTuningUrl)
⇒ 指定があった場合に優先される譜面ヘッダー：[tuning](dos-h0017-tuning.html)
- デフォルトの制作者名URLを設定します。 
```javascript
const g_presetTuningUrl = `https://www.google.co.jp/`;
```

### デフォルトスキン (g_presetSkinType)
⇒ 指定があった場合に優先される譜面ヘッダー：[skinType](dos-h0054-skinType.html)
- デフォルトスキンを**1つ**設定できます。譜面ヘッダーが指定された場合は上書きされます。  
カレントディレクトリ指定などの方法は譜面ヘッダーと同じです。
```javascript
const g_presetSkinType = `light`;
```

### デフォルトカスタムJs (g_presetCustomJs)
⇒ 指定があった場合に優先される譜面ヘッダー：[customjs](dos-h0019-customjs.html)
- デフォルトのカスタムJsを**1つ**設定できます。譜面ヘッダーが指定された場合は上書きされます。  
カレントディレクトリ指定などの方法は譜面ヘッダーと同じです。
```javascript
const g_presetCustomJs = `mainCustom.js`;
```

### デフォルトのゲージ設定 (g_presetGauge)
⇒ 指定があった場合に優先される譜面ヘッダー：[difData](dos-h0002-difData.html), [gaugeX](dos-h0022-gaugeX.html)
- 未指定時のデフォルトのゲージ設定を指定します。  
- 初期状態では未指定で、この場合はソース本体の初期値が適用されます。
```javascript
const g_presetGauge = {
	//	Border: 70,  // ノルマ制でのボーダーライン、ライフ制にしたい場合は `x` を指定
	//	Recovery: 2, // 回復量
	//	Damage: 7,   // ダメージ量
	//	Init: 25,    // 初期値
};
```

### デフォルト以外のゲージ値の初期設定 (g_presetGaugeCustom)
⇒ 指定があった場合に優先される譜面ヘッダー：[gaugeX](dos-h0022-gaugeX.html)
- ゲージ設定の各ゲージ値の初期値を設定別に設定できます。  
`SuddenDeath`は変更すると1ミスFailedにならなくなるため、変更非推奨です。
```javascript
const g_presetGaugeCustom = {
	Easy: {
		Border: 70,
		Recovery: 4,
		Damage: 7,
		Init: 25,
	},
	Hard: {
		Border: `x`,
		Recovery: 1,
		Damage: 50,
		Init: 100,
	},
	NoRecovery: {
		Border: `x`,
		Recovery: 0,
		Damage: 50,
		Init: 100,
	},
	SuddenDeath: {
		Border: `x`,
		Recovery: 0,
		Damage: setVal(g_rootObj.maxLifeVal, C_VAL_MAXLIFE, C_TYP_FLOAT),
		Init: 100,
	},
	Practice: {
		Border: `x`,
		Recovery: 0,
		Damage: 0,
		Init: 50,
	}
};
```

### カスタムゲージリスト (g_presetGaugeList)
⇒ 指定があった場合に優先される譜面ヘッダー：[customGauge](dos-h0053-customGauge.html)
- カスタムゲージでデフォルトで使用するリストを指定します。
この指定がある場合、デフォルトで用意されているゲージ設定のリストは無視されます。

```javascript
// カスタムゲージ設定(デフォルト)
// 'ゲージ名': `回復・ダメージ量設定`　の形式で指定します。
// (F : 矢印数によらず固定, V: 矢印数により変動)
const g_presetGaugeList = {
	'Original': `F`,
	'Normal': `V`,
	'Hard': `V`,
};
```

### フリーズアローのデフォルト色セットの利用有無 (g_presetFrzColors)
⇒ 指定があった場合に優先される譜面ヘッダー：[defaultFrzColorUse](dos-h0063-defaultFrzColorUse.html)
- フリーズアローの矢印色が未指定の場合、色セットをどこから指定するかを設定します。
- `true`: デフォルト色セットから使用 / `false`: 矢印色(setColor)に合わせて変更 となっており、  
未指定の場合は`true`となります。
```javascript
const g_presetFrzColors = true;
```

### デフォルトデザインの使用有無設定 (g_presetCustomDesignUse)
⇒ 指定があった場合に優先される譜面ヘッダー：[customTitleUse](dos-h0025-customTitleUse.html), [customTitleArrowUse](dos-h0026-customTitleArrowUse.html), [customTitleAnimationUse](dos-h0078-customTitleAnimationUse.html), [customBackUse](dos-h0027-customBackUse.html), [customBackMainUse](dos-h0028-customBackMainUse.html), [customReadyUse](dos-h0029-customReadyUse.html)
- タイトルで表示される曲名、背景矢印、背景などを使用するかどうかを指定します。  
使用せず独自のものを使用する場合は`true`にします。デフォルトはいずれも`false`となっています。
```javascript
const g_presetCustomDesignUse = {
	title: `false`,           // タイトル曲名
	titleArrow: `false`,      // タイトルの背景矢印
	titleAnimation: `false`,  // タイトルのアニメーション
	back: `false`,            // メイン画面以外の背景
	backMain: `false`,        // メイン画面の背景
	ready: `false`,           // メイン開始時の「Ready」表示
}
```

### オプション有効化設定 (g_presetSettingUse)
⇒ 指定があった場合に優先される譜面ヘッダー：[settingUse](dos-h0035-settingUse.html), [displayUse](dos-h0057-displayUse.html)
- オプションをデフォルト無効化する設定を行います。  
オプション名を指定し、`false`で無効化します。  
Displayオプションの場合は、`(無効化の設定),(初期値)`の順に指定します。  
使い方は譜面ヘッダー：[settingUse](dos-h0035-settingUse.html)や[displayUse](dos-h0057-displayUse.html)をご確認ください。
```javascript
const g_presetSettingUse = {
	motion: `true`,
	scroll: `true`,
	shuffle: `true`,
	autoPlay: `true`,
	gauge: `true`,
	appearance: `true`,

	stepZone: `true`,
	judgment: `true`,
	fastSlow: `true`,
	lifeGauge: `true,OFF`, // 複数指定の場合はこのようにカンマを入れて繋げる
	score: `true`,
	musicInfo: `false,ON`, // 複数指定の場合はこのようにカンマを入れて繋げる
	filterLine: `true`,
	speed: `true`,
	color: `true`,
	lyrics: `true`,
	background: `true`,
	arrowEffect: `true`,
	special: `true`,
};
```

### フリーズアローの始点判定設定 (g_presetFrzStartjdgUse)
⇒ 指定があった場合に優先される譜面ヘッダー：[frzStartjdgUse](dos-h0037-frzStartjdgUse.html)
- フリーズアローの始点で通常矢印の判定を行うかを設定します。  
判定させる場合は `true` を指定します。
```javascript
const g_presetFrzStartjdgUse = `false`;
```

### デフォルト画像の拡張子設定 (g_presetOverrideExtension)
⇒ 指定があった場合に優先される譜面ヘッダー：なし
- 矢印、おにぎり等のデフォルト画像（独自で追加している画像は除きます）について、  
svg画像を使用するか、他の拡張子（png画像など）を使用するかを設定します。  
- 未指定の場合のデフォルトは`svg`画像です。  
独自のデフォルト画像を使用している場合で  
それが`svg`形式以外の場合は下記設定にて拡張子を設定します。
```javascript
const g_presetOverrideExtension = `svg`;
```

### Reverse時の歌詞の自動反転制御設定 (g_presetWordAutoReverse)
⇒ 指定があった場合に優先される譜面ヘッダー：[wordAutoReverse](dos-h0069-wordAutoReverse.html)
- 通常は以下の条件でReverseが指定された場合、歌詞表示を反転します。  
この設定をどのように制御するか設定します。
  - 上下スクロールを挟まないキーに限定（5key, 7key, 7ikey, 9A/9Bkeyなど）
  - リバース・スクロール拡張用の歌詞表示（wordRev_data / wordAlt_data）が設定されていない作品
  - SETTINGS 画面で Reverse：ON、Scroll：--- (指定なし) を指定してプレイ開始した場合
  - 歌詞表示がすべて1段表示の場合

- 設定可能な値は以下の通りです。  
（譜面ヘッダー：[wordAutoReverse](dos-h0069-wordAutoReverse.html)と同じ）

|値|既定|内容|
|----|----|----|
|auto|*|Reverse時に歌詞表示を条件付きで反転する|
|OFF||Reverse時に歌詞表示を反転しない|
|ON||Reverse時に条件を満たさなくても歌詞を反転する　※|

※スクロール拡張（Cross, Splitなど）を設定している場合や、  
　wordRev_dataが含まれている場合は反転しません。  
　11keyなど本来適用しないキーや、歌詞が2段になっているケースが反転可能です。 

```javascript
const g_presetWordAutoReverse = `auto`;
```

### リザルトデータのフォーマット設定 (g_presetResultFormat)
⇒ 指定があった場合に優先される譜面ヘッダー：[resultFormat](dos-h0072-resultFormat.html)
- リザルトデータ（Twitter貼り付け用データ）のフォーマット変更を行います。  
使い方は [resultFormat](dos-h0072-resultFormat.html) をご覧ください。  
カスタム変数については、`g_presetResultVals`にて定義可能です。

```javascript
const g_presetResultFormat = `【#danoni[hashTag]】[musicTitle]([keyLabel]) /[maker] /Rank:[rank]/Score:[score]/Playstyle:[playStyle]/[arrowJdg]/[frzJdg]/[maxCombo] [url]`;
```

### リザルトデータ用のカスタム変数群 (g_presetResultVals)
⇒ 指定があった場合に優先される譜面ヘッダー：なし
- プロパティ名(左側)を定義すると、リザルトフォーマット上で  
`[プロパティ名]`というフォーマットを使用できます。  
右側に定義する値は、g_resultObj配下にカスタムjsを利用して定義する必要があります。

- 例えば、下記の場合はリザルトフォーマットに`[exScore]`と指定すると  
実際には`g_resultObj.exScores`に置き換えられます。
```javascript
const g_presetResultVals = {
	exScore: `exScores`,
};
```

- customjs上の定義
```javascript
g_resultObj.exScores = 300;  // [exScore]は`300`に置き換えられる
```

### ラベルテキスト設定 (g_local_lblNameObj)
⇒ 指定があった場合に優先される譜面ヘッダー：なし
- danoni_constants.jsにある [g_lblNameObj](obj-v0015-g_lblNameObj.html) を上書きする設定を定義できます。  
上書きするプロパティに対して、適用したい値を指定してください。変更したい分だけ追加が可能です。  
この設定は、カスタムjsやスキンjsでも利用可能です。
```javascript
const g_local_lblNameObj = {
    settings: `オプション`,
};
```
<details>
<summary>g_lblNameObj で定義されているプロパティ一覧</summary>

- ここで定義されているプロパティを、`g_local_lblNameObj`で上書きできます。  
※下記は一例です。詳細は [g_lblNameObj](obj-v0015-g_lblNameObj.html) をご覧ください。

```javascript
const g_lblNameObj = {
    dancing: `DANCING`,
    star: `☆`,
    onigiri: `ONIGIRI`,
    settings: `SETTINGS`,
    display: `DISPLAY`,
    key: `KEY`,
    config: `CONFIG`,
    result: `RESULT`,

    b_back: `Back`,
    b_keyConfig: `KeyConfig`,
    b_play: `PLAY!`,
    b_reset: `Reset`,
    b_settings: `To Settings`,
    b_copy: `CopyResult`,
    b_tweet: `Tweet`,
    b_gitter: `Gitter`,
    b_retry: `Retry`,

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

    ConfigType: `ConfigType`,
    ColorType: `ColorType`,
    KeyPattern: `KeyPattern`,

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
};
```
</details>

### オンマウステキスト、確認メッセージ定義設定 (g_local_msgObj)
⇒ 指定があった場合に優先される譜面ヘッダー：なし
- danoni_constants.jsにある [g_msgObj](obj-v0016-g_msgObj.html) を上書きする設定を定義できます。  
この設定は、カスタムjsやスキンjsでも利用可能です。
```javascript
const g_local_msgObj = {
    reload: `ページを再読込します。`,
};
```
<details>
<summary>g_msgObj で定義されているプロパティ一覧</summary>

- ここで定義されているプロパティを、`g_local_msgObj`で上書きできます。  
※下記は一例です。詳細は [g_msgObj](obj-v0016-g_msgObj.html) をご覧ください。

```javascript
const g_msgObj = {

    reload: `ページを再読込します。`,
    howto: `ゲーム画面の見方や設定の詳細についてのページへ移動します（GitHub Wiki）。`,
    dataReset: `この作品で保存されているハイスコアや\nAdjustment情報等をリセットします。`,
    github: `Dancing☆Onigiri (CW Edition)のGitHubページへ移動します。`,
    security: `Dancing☆Onigiri (CW Edition)のサポート情報ページへ移動します。`,

    dataResetConfirm: `この作品のローカル設定をクリアします。よろしいですか？\n(ハイスコアやAdjustment等のデータがクリアされます)`,
    keyResetConfirm: `キーを初期配置に戻します。よろしいですか？`,

    difficulty: `譜面を選択します。`,
    speed: `矢印の流れる速度を設定します。`,
    motion: `矢印の速度を一定ではなく、\n変動させるモーションをつけるか設定します。`,
    reverse: `矢印の流れる向きを設定します。`,
    scroll: `各レーンのスクロール方向をパターンに沿って設定します。`,
    shuffle: `譜面を左右反転したり、ランダムにします。\nランダムにした場合は別譜面扱いとなり、ハイスコアは保存されません。`,
    autoPlay: `オートプレイや一部キーを自動で打たせる設定を行います。\nオートプレイ時はハイスコアを保存しません。`,
    gauge: `クリア条件を設定します。`,
    adjustment: `タイミングにズレを感じる場合、\n数値を変えることでズレを直すことができます。`,
    fadein: `譜面を途中から再生します。\n途中から開始した場合はハイスコアを保存しません。`,
    volume: `ゲーム内の音量を設定します。`,

    graph: `速度変化や譜面密度状況、\n譜面の難易度など譜面の詳細情報を表示します。`,
    dataSave: `ハイスコア、リバース設定、\nキーコンフィグの保存の有無を設定します。`,
    toDisplay: `プレイ画面上のオブジェクトの\n表示・非表示（一部透明度）を設定します。`,
    toSettings: `SETTINGS画面へ戻ります。`,

    d_stepzone: `ステップゾーンの表示`,
    d_judgment: `判定キャラクタ・コンボの表示`,
    d_fastslow: `Fast/Slow表示`,
    d_lifegauge: `ライフゲージの表示`,
    d_score: `現時点の判定数を表示`,
    d_musicinfo: `音楽情報（時間表示含む）`,
    d_filterline: `Hidden+, Sudden+使用時のフィルターの境界線表示`,
    d_speed: `途中変速、個別加速の有効化設定`,
    d_color: `色変化の有効化設定`,
    d_lyrics: `歌詞表示の有効化設定`,
    d_background: `背景・マスクモーションの有効化設定`,
    d_arroweffect: `矢印・フリーズアローモーションの有効化設定`,
    d_special: `作品固有の特殊演出の有効化設定`,

    appearance: `流れる矢印の見え方を制御します。`,
    opacity: `判定キャラクタ、コンボ数、Fast/Slow、Hidden+/Sudden+の\n境界線表示の透明度を設定します。`,

};
```

</details>

### 設定名の上書き可否設定 (g_lblRenames)
⇒ 指定があった場合に優先される譜面ヘッダー：なし
- [g_lblNameObj / g_local_lblNameObj](obj-v0015-g_lblNameObj.html) のうち、  
プロパティ名が`u_`で始まるプロパティを設定した値で置き換えるかを画面別に設定します。 
- デフォルトはすべて`true`で、設定した値で書き換えるようになっています。 `false`にすると書き換えません。
- `u_`で始まらないプロパティは無条件で置き換えます。  
`u_`で始まるプロパティは画面をまたがって設定する項目のため、  
画面によってはそのままにしたい場合に使用します。

```javascript
const g_lblRenames = {
	option: true,
	settingsDisplay: true,
	keyConfig: true,
	result: true,
};
```

#### `u_`で始まるプロパティの例
- 設定画面の設定名が主に該当します。[g_lblNameObj / g_local_lblNameObj](obj-v0015-g_lblNameObj.html) もご覧ください。

```javascript
{
    'u_Cross': `Cross`,
    'u_Split': `Split`,
    'u_Alternate': `Alternate`,
    'u_Twist': `Twist`,
    'u_Asymmetry': `Asymmetry`,
    'u_Flat': `Flat`,
    'u_R-': `R-`,
    'u_Reverse': `Reverse`,
}
```

## 更新履歴

|Version|変更内容|
|----|----|
|[v20.3.1](https://github.com/cwtickle/danoniplus/releases/tag/v20.3.1)|・設定名の上書き可否設定 (g_lblRenames)を実装|
|[v19.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.3.0)|・ラベルテキスト、オンマウステキスト、確認メッセージ定義設定<br>　 (g_local_lblNameObj, g_local_msgObj)を実装<br>・デフォルトスキン／カスタムJs (g_presetSkinType, g_presetCustomJs)を実装|
|[v19.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.1.0)|・カスタムゲージリスト (g_presetGaugeList)を実装|
|[v18.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.5.0)|・タイトル文字のアニメーション設定 (g_presetCustomDesignUse.titleAnimation)を実装|
|[v16.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v16.2.1)|・リザルトデータのフォーマット設定 (g_presetResultFormat, g_presetResultVals)を実装|
|[v15.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.4.0)|・Reverse時の歌詞の自動反転制御設定 (g_presetWordAutoReverse)を実装|
|[v15.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.1.0)|・デフォルト画像の拡張子設定 (g_presetOverrideExtension)を実装|
|[v14.0.2](https://github.com/cwtickle/danoniplus/releases/tag/v14.0.2)|・オプション有効化設定 (g_presetSettingUse)のDisplayオプションについて、<br>　デフォルトOFF設定及び有効/無効化設定を実装|
|[v13.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v13.4.0)|・オプション有効化設定 (g_presetSettingUse)について<br>　Displayオプションも指定できるように変更|
|[v10.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v10.0.0)|・共通設定ファイルの変更、分割設定（-> [settingType](dos-h0056-settingType.html)）の実装|
|[v9.4.2](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.2)|・デフォルト以外のゲージ値の初期設定 (g_presetGaugeCustom)の内容更新<br>　(カスタムゲージ実装によるライフ上限値可変に伴い)|
|[v9.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.0)|・デフォルト以外のゲージ値の初期設定 (g_presetGaugeCustom)を実装|
|[v9.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v9.0.0)|・オプション有効化設定 (g_presetSettingUse)についてAppearanceの設定有無を追加|
|[v5.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v5.7.0)|・フリーズアローの始点判定設定 (g_presetFrzStartjdgUse)を実装|
|[v3.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.6.0)|・デフォルトデザインの使用有無設定 (g_presetCustomDesignUse)を実装|
|[v3.1.1](https://github.com/cwtickle/danoniplus/releases/tag/v3.1.1)|・オプション有効化設定 (g_presetSettingUse)についてGaugeの設定有無を追加|
|[v3.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.1.0)|・オプション有効化設定 (g_presetSettingUse)を実装|
|[v3.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.0.0)|・初期実装|