# アップグレードガイド / Migration Guide
- 最新の情報は[Release](https://github.com/cwtickle/danoniplus/releases)をご覧ください。
- 更新情報の概要については[更新情報(UpdateInfo)](UpdateInfo.html)もご覧ください。

## ⭐ v20 -> v21
ReleasesのFiles Changedの項目を参照してください。 

### 1. 一部関数の見直し
- 一部関数について廃止もしくは引数の見直しを行っています。

|関数|変更内容|
|----|----|
|resetCursor|引数カット|
|resetCursorMain|廃止|
|resetCursorReplaced|廃止|
|resetCursorALL|廃止|
|setKeyConfigCursor|引数カット|

#### 🛠 修正事項
- カスタムJs等で利用している場合は注意してください。

### 2. danoni_legacy_function.js へ移動した関数について
- 現行ソースで未使用の以下の関数を「danoni_legacy_function.js」へ移動しました。  
対象：checkArrayVal, getStrLength, paddingLeft, createDivCustomLabel  

#### 🛠 修正事項
- 今後も利用する場合は、lib/danoni_legacy_function.js をサーバーへアップロードしてください。

## ⭐ v19 -> v20
ReleasesのFiles Changedの項目を参照してください。 

### 1. 変数名の変更
- 現行ソースで未使用、もしくは今後の機能拡張上支障が出る変数群に対して  
変数名の見直しを行いました。

<details>
<summary>変更対象の変数一覧（クリックして開閉）</summary>

#### 判定キャラクタ

|旧変数|新変数|デフォルト値|
|----|----|----|
|C_JCR_II|g_lblNameObj.j_ii|"(・∀・)ｲｲ!!"|
|C_JCR_SHAKIN|g_lblNameObj.j_shakin|"(`・ω・)ｼｬｷﾝ"|
|C_JCR_MATARI|g_lblNameObj.j_matari|"( ´∀`)ﾏﾀｰﾘ"|
|C_JCR_SHOBON|g_lblNameObj.j_shobon|"(´・ω・`)ｼｮﾎﾞｰﾝ"|
|C_JCR_UWAN|g_lblNameObj.j_uwan|"( `Д´)ｳﾜｧﾝ!!"|
|C_JCR_KITA|g_lblNameObj.j_kita|"(ﾟ∀ﾟ)ｷﾀ-!!"|
|C_JCR_IKNAI|g_lblNameObj.j_iknai|"(・A・)ｲｸﾅｲ"|

#### 判定領域 g_judgObj の位置

|旧変数|新変数|デフォルト値|
|----|----|----|
|C_JDG_II|g_judgPosObj.ii|0|
|C_JDG_SHAKIN|g_judgPosObj.shakin|1|
|C_JDG_MATARI|g_judgPosObj.matari|2|
|C_JDG_SHOBON|g_judgPosObj.shobon|3|
|C_JDG_UWAN|g_judgPosObj.uwan|4|
|C_JDG_KITA|g_judgPosObj.kita|0|
|C_JDG_SFSF|g_judgPosObj.sfsf|1|
|C_JDG_IKNAI|g_judgPosObj.iknai|2|

#### 設定系変数群

|旧変数|新変数|
|----|----|
|g_speeds|g_settings.speeds|
|g_speedNum|g_settings.speedNum|
|g_motions|g_settings.motions|
|g_motionNum|g_settings.motionNum|
|g_scrolls|g_settings.scrolls|
|g_scrollNum|g_settings.scrollNum|
|g_reverses|g_settings.reverses|
|g_reverseNum|g_settings.reverseNum|
|g_shuffles|g_settings.shuffles|
|g_shuffleNum|g_settings.shuffleNum|
|g_autoPlays|g_settings.autoPlays|
|g_autoPlayNum|g_settings.autoPlayNum|
|g_gauges|g_settings.gauges|
|g_gaugeNum|g_settings.gaugeNum|
|g_adjustments|g_settings.adjustments|
|g_adjustmentNum|g_settings.adjustmentNum|
|g_volumes|g_settings.volumes|
|g_volumeNum|g_settings.volumeNum|
|g_appearances|g_settings.appearances|
|g_appearanceNum|g_settings.appearanceNum|
|g_opacitys|g_settings.opacitys|
|g_opacityNum|g_settings.opacityNum|
|g_scoreDetails|g_settings.scoreDetails|
|g_scoreDetailNum|g_settings.scoreDetailNum|

#### 前/次の設定に進めるボタンの表示位置

|旧変数|新変数|
|----|----|
|C_LBL_SETMINIL|g_settingBtnObj.chara.L|
|C_LBL_SETMINILL|g_settingBtnObj.chara.LL|
|C_LBL_SETMINIR|g_settingBtnObj.chara.R|
|C_LBL_SETMINIRR|g_settingBtnObj.chara.RR|
|C_LBL_SETMINIL_LEFT|g_settingBtnObj.pos.L|
|C_LBL_SETMINILL_LEFT|g_settingBtnObj.pos.LL|
|C_LBL_SETMINIR_LEFT|g_settingBtnObj.pos.R|
|C_LBL_SETMINIRR_LEFT|g_settingBtnObj.pos.RR|

</details>

#### 🛠 修正事項
- 該当する変数群をカスタムしている場合は、新変数に変更してください。

### 2. danoni_legacy_function.js へ移動した関数について
- 現行ソースで未使用の以下の関数を「danoni_legacy_function.js」へ移動しました。  
対象：createLabel  

#### 🛠 修正事項
- 今後も利用する場合は、lib/danoni_legacy_function.js をサーバーへアップロードしてください。

### 3. g_resultMsgObj の廃止 (ver19.5.1以降)
- FULL COMBOやPerfectの表示部分のhtml部分を管理する`g_resultMsgObj`が廃止になっています。

#### 🛠 修正事項
- 利用している場合は、代替関数 `resultViewText` の利用を検討してください。

### 4. Display画面からSettings画面へ戻るボタンの位置変更
- Settings画面からDisplay画面へ移動するボタンと統一しました。  
ID名は従来のままのため、個別の設定は可能です。

#### 🛠 修正事項
- 当該ボタンをカスタムしている場合、念のため見た目に影響が無いか確認してください。

### 5. ステップゾーン位置を表す旧変数の削除
- 従来、ステップゾーン位置を表していた `g_stepY`や`g_distY`などについて、  
正式に g_posObj へ移行しました。

|旧変数|新変数|
|----|----|
|g_stepY|g_posObj.stepY|
|g_stepYR|g_posObj.stepYR|
|g_distY|g_posObj.distY|
|g_reverseStepY|g_posObj.reverseStepY|

#### 🛠 修正事項
- v20以降、旧変数は使えなくなります。  
カスタム側で使用している場合は変数を置き換えてください。

## ⭐ v18 -> v19
ReleasesのFiles Changedの項目を参照してください。 

### 1. danoni_legacy_function.js へ移動した関数について
- 現行ソースで未使用の以下の関数を「danoni_legacy_function.js」へ移動しました。  
対象：createDivCssLabel, createCssButton, createColorObject  

#### 🛠 修正事項
- 今後も利用する場合は、lib/danoni_legacy_function.js をサーバーへアップロードしてください。

### 2. gaugeXの初期値補完について
- gaugeX (gaugeEasy, gaugeHardなど)について、2譜面目以降の設定を省略した場合、  
1譜面目のgaugeXの設定が引き継がれるようになりました。

#### 🛠 修正事項
- 基本的に影響は無いはずですが、gaugeXを中途半端に設定していた場合、  
設定の引継ぎにより設定値が変わる可能性があります。  
必要に応じて、gaugeXの設定値を見直してください。  

### 3. 初期表示時のclearWindow関数内包
- titleInit / optionInit / settingsDisplayInit / loadMusic / MainInit / resultInit の処理の先頭に  
clearWindow() 処理を追加しています。

#### 🛠 修正事項
- 上記関数呼び出し時のclearWindow関数の呼び出しが不要になります。  
基本的に影響は無いと思いますが、カスタムで処理をさせている場合はご注意ください。  
- clearWindow関数を上記関数前に指定している場合、2回呼び出されることになりますが影響はありません。

## ⭐ v17 -> v18
ReleasesのFiles Changedの項目を参照してください。  

### 1. 矢印・フリーズアローの個別属性の変更について
- 直接使用する機会は無いかもしれませんが、矢印・フリーズアローの個別属性の仕様が変わりました。
カスタムjsで使用している場合、修正が必要です。

#### 🛠 修正事項
- [主要オブジェクトのプロパティ](objectMainRef.html)に記載の変数を使用している場合、修正が必要です。

変更前
```javascript
const boostSpd = parseFloat(document.querySelector(`#arrow${_j}_${_k}`).getAttribute(`boostSpd`));
```

変更後
```javascript
const boostSpd = g_attrObj[`arrow${_j}_${_k}`].boostSpd;
```

### 2. タイトルアニメーションの仕様変更 (ver18.5.0以降)  
- タイトル文字のアニメーションを譜面ヘッダー：[titleanimation](dos-h0077-titleanimation.html) にて設定できるようになりました。

#### 🛠 修正事項
- 今後、`#lblmusicTitle` にてCSSを直接変更した場合、両方の設定が反映されます。ご注意ください。
- 従来の設定を維持したい場合は、`danoni_main.css`を**変更せず**、
`danoni_setting.js`にてg_presetCustomDesignUse の titleAnimation を `true`に変更してください。

#### 従来の指定方法
```css
#lblmusicTitle {
    animation-name: upToDown;
    animation-duration: 2.0s;
}
```

#### 今後の指定方法
```
|titleanimation=upToDown,120,0|
```

### 3. Gitterボタン、操作方法リンクの追加 (ver18.8.0以降)
- Gitter（結果画面）、操作方法（タイトル画面）へリンクするボタンが追加されました。  
ID名はそれぞれ「btnGitter」「btnHelp」です。  

#### 🛠 修正事項
- 結果画面、タイトル画面のデザインを変更している場合は修正が必要となります。

## ⭐ v16 -> v17
ReleasesのFiles Changedの項目を参照してください。  

### 1. strictモードの再有効化 (ver17.4.0より)
- v2～v17.3まで、strictモードが有効になっていませんでした。  
ver17.4.0より再度有効化しています。  
カスタムjsにて予約語を利用していたり、変数を初期化していない場合動作しないことがあります。

#### 🛠 修正事項
- カスタムjsにて変数を初期化していること、予約語を使用していないことを確認してください。  
以下は予約語のため、変数に使用できません。
  - implements、interface、let、package、private、protected、public、static、yield
- 参考：https://developer.mozilla.org/ja/docs/Web/JavaScript/Reference/Strict_mode

### 2. ラベル・ボタン・色付きオブジェクト作成用関数の変更
- それぞれ次の関数に移行しています。

|変更前関数|変更後関数|概要|
|----|----|----|
|createDivCssLabel|createDivCss2Label|ラベル作成用関数|
|createCssButton|createCss2Button|ボタン作成用関数|
|createColorObject|createColorObject2|色付きオブジェクト作成用関数|

#### 🛠 修正事項
- 変更前関数は残しているのでそのままでも問題はありませんが、  
今後`danoni_legacy_function.js`へ移動となる可能性があります。  
customjsで指定している場合はご注意ください。

## ⭐ v15 -> v16
ReleasesのFiles Changedの項目を参照してください。  

### 1. CopyResultボタンの追加 (ver16.1.0より)
- リザルトデータをクリップボードへコピーするボタンが追加されました。  
ID名は「btnCopy」です。  

#### 🛠 修正事項
- 結果画面デザインを変更している場合は修正が必要となります。

## ⭐ v14 -> v15
ReleasesのFiles Changedの項目を参照してください。

### 1. 設定画面内の設定別スプライト変数名変更
- 設定別のスプライト変数名を変更しています。
なお、ID名は変更していません。

|変数変更前|変数変更後|
|----|----|
|difficultySprite|spriteList.difficulty|
|speedSprite|spriteList.speed|
|motionSprite|spriteList.motion|
|shuffleSprite|spriteList.shuffle|
|scrollSprite|spriteList.scroll|
|reverseSprite|spriteList.reverse|
|autoPlaySprite|spriteList.autoPlay|
|gaugeSprite|spriteList.gauge|
|adjustmentSprite|spriteList.adjustment|
|fadeinSprite|spriteList.fadein|
|volumeSprite|spriteList.volume|
|appearanceSprite|spriteList.appearance|
|opacitySprite|spriteList.opacity|

#### 🛠 修正事項
- 設定別スプライト変数名をそのまま使用している場合は、変更が必要です。  
ID名参照（例：`querySelector('#difficultySprite')`など）の場合は変更不要です。

## ⭐️ v13 -> v14
ReleasesのFiles Changedの項目を参照してください。

### 1. スキンファイル(css)の更新
- Opacityオプションの追加、Displayオプションの無効化ボタン背景色追加による変更です。 

#### 🛠 修正事項（必須）
- デフォルトスキンを利用している方は、Files Changedの項目を参考に入れ替えてください。
- 独自スキンを利用している方は、以下の項目を足してください。
```css
/* opacityオプション用：ver13.5.1以降。ver13.4.0以前からの変更のみ追加 */
.settings_Opacity::first-letter {
	color:#999999;
}

/* ステップゾーン用の影矢印色：ver14.1.0以降 */
.main_objStepShadow {
	background-color: #000000;
}

/* ボタン：ON/OFF 無効化ボタン用 */
.button_DisabledOFF {
	color: #999999;
	background-color: #333333;
}
.button_DisabledON {
	color: #ffffff;
	background-color: #009999;
}
```

## ⭐️ v12 -> v13
ReleasesのFiles Changedの項目を参照してください。

### 1. スキンファイル(css)の更新
- Opacityオプションの追加、Displayオプションの無効化ボタン背景色追加による変更です。 

#### 🛠 修正事項（必須）
- デフォルトスキンを利用している方は、Files Changedの項目を参考に入れ替えてください。
- 独自スキンを利用している方は、以下の項目を足してください。
```css
/* opacityオプション用：ver13.5.1以降 */
.settings_Opacity::first-letter {
	color:#999999;
}
```

## ⭐️ v11 -> v12
### 1. danoni_contents.jsの更新
- 譜面詳細画面の追加に伴う変更です。  

#### 🛠 修正事項（必須）
- danoni_contents.js を入れ替えてください。（./js/lib にあります）

## ⭐️ v10 -> v11
### 1. danoni_contents.jsの更新
- キーコンフィグの見直しを行っています。

#### 🛠 修正事項（必須）
- danoni_contents.js を入れ替えてください。（./js/lib にあります）

### 2. danoni_skin_default(light, skyblue).css の更新（v10.1.1以前からの更新のみ）
- v10.2.1より、Reverse / Scroll の色設定を追加しています。  

#### 🛠 修正事項
- v10.1.1以前からの更新の場合、skinフォルダにある以下のファイルを入れ替えてください。
  - danoni_skin_default.css
  - danoni_skin_light.css
  - danoni_skin_skyblue.css

### 3. word/back/mask_dataのCross/Split対応（v10.1.1以前からの更新のみ）
- v10.2.1より、Cross/Split等のスクロール拡張オプションが追加されています。  
スクロール方向により、演出系に影響がある場合は独自に対応するか、  
Cross/Split等の実行時は演出OFFにするといった対応が必要です。

#### 🛠 修正事項
- Cross/Split等のword/back/mask_dataとして、  
`wordAlt_data`, `backAlt_data`, `maskAlt_data`が使用できます。  
取り急ぎCross/Split等の実行時は演出OFFにする場合、  
下記を譜面に追加することで対応可能です。  
```
|wordAlt_data=|backAlt_data=|maskAlt_data=|
```

## ⭐️ v9 -> v10
### 1. スキンファイル追加・画像ファイル名変更
- [更新情報(UpdateInfo-v10)](UpdateInfo-v10.html)にも追記していますが、  
スキン実装によりファイルが追加・変更されています。

#### 🛠 修正事項 (必須)
- cssフォルダ、imgフォルダを v10 のものに入れ替えてください。  
また、skinフォルダをcss, imgフォルダと同じ階層に置いてください。  
※danoni_custom.js, danoni_setting.jsの入れ替えは不要です。

### 2. 設定画面のoptionsprite位置変更
- 設定画面の各項目を覆うoptionspriteについて、背景色を塗ったときに欠けが起こらないよう、位置を調整しました。

#### 🛠 修正事項
- optionsprite上に別オブジェクトを配置している場合、X方向に25px, Y方向に20pxを足してください。

### 3. ステップゾーンのグループ化
- ステップゾーン関係のオブジェクトが`stepRootX`で一律管理されるようになりました。

#### 🛠 修正事項
1. 座標変更している作品は`stepX` -> `stepRootX` へ変更が必要です。
```javascript
    document.querySelector(`#step0`).style.left = `50px`;  // 変更前
    document.querySelector(`#stepRoot0`).style.left = `50px`;  // 変更後
```

2. またステップゾーンに回転を加えている場合、
指定するオブジェクトにより指定する回転数が異なります。
（既存作品については、手間でも構成オブジェクト個々に回転数を指定した方が無難です。）
    - `stepRootX` (ステップゾーンルート)：
生成時点からの**相対値** (最初が60度、移動後が90度なら指定する値は30度)
    - `stepX`, `stepDivX`, `stepHitX` (ステップゾーン構成オブジェクト)：
指定した**絶対値**そのまま (移動後が90度なら、指定する値は最初によらず90度固定)
```javascript
    document.querySelector(`#step0`).style.transform = `rotate(180deg)`; 
    document.querySelector(`#stepHit0`).style.transform = `rotate(180deg)`; 
    document.querySelector(`#stepDiv0`).style.transform = `rotate(180deg)`;   // 新たに追加
```

## ⭐️ v8 -> v9
### 1. 矢印・フリーズアローのオブジェクトルート変更
- 以下のように変更しました。arrowSprite0/1は、mainSpriteの子要素です。

|オブジェクト|v8まで|v9以降|
|----|----|----|
|ステップゾーン|mainSprite|mainSprite|
|矢印・フリーズアロー|mainSprite|arrowSprite0 (スクロール方向が上向き)<br>arrowSprite1 (スクロール方向が下向き)|

#### 🛠 修正事項
- 通常は変更不要です。  
矢印・フリーズアローを作成・削除する処理を外部から行っている場合、変更が必要です。  

### 2. danoni_main.cssの更新（v9.4.3にて更新あり）
- Appearance用のクリッピングマスクとして、CSSクラスを追加しています。
- 設定画面のGaugeオプションの詳細表示で、新たにCSSクラスを追加しています。

#### 🛠 修正事項（必須）
- danoni_main.css を入れ替えてください。

### 3. danoni_setting.jsの更新（v9.4.2にて更新あり）
- カスタムゲージ実装によりデフォルト設定以外のゲージの再設定が必要なため、一部追加が必要です。

#### 🛠 修正事項（カスタムゲージ利用時必須）
- danoni_setting.js のg_presetGaugeCustom を、以下のように変更してください。  
SuddenDeath以外の各数値は必要に応じて変更して問題ありません。

```javascript
// ゲージ設定（デフォルト以外）
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

## ⭐️ v7 -> v8
### 1. リザルトモーションの音楽同期化
- リザルトモーション（backresult_data 他）について、  
音楽に同期したフレーム制御になりました。（メイン画面と同様）

#### 🛠 修正事項
- 通常は変更不要です。  
リザルトモーションと音楽を同期させる演出を行っている場合、フレーム数の修正が必要になる場合があります。  

### 2. 速度変化 (speed_data/change) の統一
- 途中変速で使用する速度変化 (speed_data, speed_change) がキーの種類に関係なくどちらでも使えるようになりました。  
どちらも指定した場合は、speed_change側が優先されます。

|B/A|概要|
|----|----|
|変更前|5key: speed_data / 5key以外: speed_change|
|変更後|speed_data もしくは speed_change (キーの種類によらず)|

#### 🛠 修正事項
- 通常は変更不要です。  
同一譜面でどちらも指定していた場合のみ、どちらかに合わせることを推奨します。  

## ⭐️ v6 -> v7
### 1. 個別色変化(フリーズアローヒット時)のタイミング変更
- [個別色変化(color_data)](dos-e0002-colorData.html)においてフリーズアローヒット時の色のタイミングが変わりました。  

|B/A|概要|
|----|----|
|変更前|対象のフリーズアローが出現したタイミングで色変更<br>※逆算されるため、実際に使用するタイミングより値を大きくする必要がある|
|変更後|対象のフリーズアローがヒット時に変わる(ステップゾーン到達)タイミングで色変更<br>※実際に使用するタイミングと同一|

#### 🛠 修正事項
- フリーズアローヒット時の色変更を`color_data`で行っていた場合、  
値の見直しを行うか、譜面ヘッダーで以下を指定してください。
```
|colorDataType=v6|
```
### 2. 楽曲の終了判定タイミングの変更（秒単位からフレーム単位へ）
- 楽曲の終了判定タイミングがフレーム単位に変わりました。

#### 🛠 修正事項
- ほとんど問題はありませんが、譜面ヘッダー：endFrameなどで終了タイミングを指定していない場合、
楽曲の終了位置が若干変わる可能性があります。  
必要に応じて、譜面ヘッダー：endFrameを指定して終了位置を調整してください。

### 3. danoni_main.cssの更新
- 誤爆抑止用のボタンアニメの実装のために、CSSモーションを追加しています。

#### 🛠 修正事項（必須）
- danoni_main.css を入れ替えてください。

## ⭐️ v5 -> v6
### 1. ライフゲージ（初期）の値変更
- ライフ上限値を可変にしたため、ライフゲージ（初期）の値(lifeInit)の取り方が変わりました。

|B/A|概要|
|----|----|
|変更前|ライフ上限：1000に対して実際の初期ライフ値を設定（デフォルト：250）|
|変更後|上限値に関係なく、全体の何％を初期ライフ値にするかを設定（デフォルト：25）|

#### 🛠 修正事項
- 通常はありませんが、カスタム側で強制的に`lifeInit`を変更する処理を入れていた場合、  
値の見直し（数値を10で割る）が必要です。

## ⭐️ v4 -> v5
### 1. 変数名の変更
- コード集約により、変数名の一部が変わりました。

|変更前|変更後|
|----|----|
|g_stateObj.auto|g_stateObj.autoPlay|
|g_stateObj.lifeId|g_gaugeNum|
|g_stateObj.lifeSetName|g_stateObj.gauge|

#### 🛠 修正事項
- カスタム側でこれらの変数（変更前）を使用していた場合、  
変更後の変数へ置き換えが必要です。

### 2. danoni_main.cssの更新
- 歌詞表示のフェードイン・アウト用のCSSモーションを追加しています。

#### 🛠 修正事項（必須）
- danoni_main.css を入れ替えてください。

## ⭐️ v3 -> v4
- 特にありません。
- v4.x以降、[ローカルストレージ保存](LocalStorage.html)機能が有効となり、  
ハイスコア等のデータが保存されるようになります。

## ⭐️ v2 -> v3
### 1. 設定ファイル (danoni_setting.js)の追加
- 作品群全体の設定ファイル(danoni_setting.js)が追加されました。

#### 🛠 修正事項（必須）
- jsフォルダ配下に、`danoni_setting.js`を追加する必要があります。

### 2. danoni_main.cssの更新
- タイトル文字用のCSSモーションを追加しています。

#### 🛠 修正事項（必須）
- danoni_main.css を入れ替えてください。

### 3. 歌詞表示(word_data)のセット毎改行区切りに対応
- 1セット1行としている場合に限り、行末のカンマが不要になりました。
※色変化についてもセット毎改行区切りに対応しました。
```
|word_data=
300,0,[fadein]
350,0,歌詞テスト
400,0,[fadeout]
|
```
#### 🛠 修正事項
- 特になし。  
ただし今後、改行を使わない歌詞表示(word_data)については非推奨となる可能性があります。

### 4. 設定画面のレイアウト変更
- Shuffle機能追加に伴い、画面レイアウトが変わりました。

#### 🛠 修正事項
- 設定画面の上からカスタムでデザインを変えている場合、位置調整が必要です。  

## ⭐️ v1 -> v2
### 1. danoni_custom.jsの見直し
- 従来のcustomファイルより、共通部分がdanoni_main.jsへ移動しました。

#### 🛠 修正事項（必須）
- [ver2.1.0への移行について](for_ver2.1.0)をご覧ください。
