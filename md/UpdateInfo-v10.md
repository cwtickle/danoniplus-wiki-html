# 更新情報 (UpdateInfo-v10)

## 変更ファイル一式
- 多くのファイルで変更があります。
必要なファイルまで上書きしないよう注意してください。
- `danoni_custom.js`, `danoni_setting.js`の変更はありません。

|フォルダ名|状態|変更ファイル名|備考|
|----|----|----|----|
|js|変更|danoni_main.js|本体jsファイル|
|js/lib|追加|danoni_constants.js|定数管理用jsファイル<br>※v10.2.1以降|
|js/lib|追加|danoni_legacy_function.js|過去互換関数用jsファイル<br>※v10.2.1以降|
|css|変更|danoni_main.css|本体cssファイル|
|img|名称変更|aaShadow.png|アスキーアートの影部分画像|
|img|名称変更|arrow.png|矢印画像|
|img|名称変更|arrowShadow.png|矢印の影部分画像|
|img|名称変更|c.png|しぃ画像|
|img|名称変更|giko.png|ギコ画像|
|img|名称変更|iyo.png|ぃょぅ画像|
|img|名称変更|monar.png|モナー画像|
|img|名称変更|morara.png|モララー画像|
|img|名称変更|onigiri.png|おにぎり画像|
|skin|追加|danoni_skin_default.css|デフォルトスキン|
|skin|追加|danoni_skin_default.js|デフォルトスキン拡張|
|skin|追加|danoni_skin_light.css|白背景スキン|
|skin|追加|danoni_skin_light.js|白背景スキン拡張|
|skin|追加|danoni_skin_skyblue.css|スカイブルースキン|
|skin|追加|danoni_skin_skyblue.js|スカイブルースキン拡張|
|skin|追加|danoni_skin_background.css|背景用スキンテンプレート|
|skin|追加|danoni_skin_background.js|背景用スキン拡張テンプレート|
|skin|追加|danoni_skin_blank.css|スキン2つ目テンプレート|
|skin|追加|danoni_skin_blank.js|スキン2つ目拡張テンプレート|

※ jsファイルは任意です。無くても動作します。

## 新機能・変更点
## 1. スキンの実装
- スキンファイルを使って、全体的な色替えが行えるようになりました。

### ファイル構成
- スキンが実装され、スキン用のフォルダができました。
- danoni_skin_XXX.css (.js) の形で使用します。 XXX の部分はスキン名で、譜面ヘッダーより指定が可能です。

|フォルダ名|ファイル名|必須|役割|
|----|----|----|----|
|skin|danoni_skin_default.css|*|スキン指定が無い場合のデフォルトスキン。<br>v9までのデザインはこのファイルに移行されています。|
|skin|danoni_skin_default.js||デフォルトスキンのjs拡張。フォーマットのみ。無くても動作します。|
|skin|danoni_skin_light.css||白背景スキン。|
|skin|danoni_skin_light.js||白背景スキンのjs拡張。デフォルト色パターンを変更しています。|

### 使い方
- スキンをデフォルト以外に設定する場合、作品ページの**Canvasタグを取る**必要があります。  
canvasに対して画像を貼っている場合、注意してください。  
※ver10.1.0以降はスキンがデフォルト以外であれば入れていても問題ありません。  
```HTML
<div id="canvas-frame" style="width:600px;">
  <!-- Canvasタグは不要
    <canvas id="layer0" width="600" height="500"></canvas>
    <canvas id="layer1" width="600" height="500"></canvas>
   -->
</div>
```

- スキンは譜面ヘッダーの「skinType」より設定を行います。  
「light」と指定した場合は、「skin」フォルダに `danoni_skin_light.css` （、`danoni_skin_light.js`）が必要です。  
jsファイルは拡張のため、任意です。

```
|skinType=light|
```

- そのスキンが特定の作品専用の場合、  
作品ページと同一フォルダにスキンファイル(css, js)を配置させることができます。  
指定するスキン名の前に`(..)`を入れることで、作品ページと同一フォルダにあるスキンファイルを参照します。  
この場合は、作品ページと同じフォルダに `danoni_skin_original.css` があれば良いことになります。
```
|skinType=(..)original|
```

### スキンのカスタマイズ
- スキンは複製して名前を変えれば、カスタマイズすることができます。  
`danoni_skin_default.css`が暗背景、`danoni_skin_light.css`が明背景用です。
- 今後のバージョンアップにより、若干の項目追加が発生する可能性があります。

#### cssファイルの変更
- cssファイル側は基本的にカラーコード情報のみです。  
カラーコードを変更することで、画面の見た目を変えることができます。  
- 下記であれば、設定画面の`Difficulty`, `Speed`の先頭文字の色が変更できます。
```css
.settings_Difficulty::first-letter {
	color:#990000;
}
.settings_Speed::first-letter {
	color:#777700;
}
```

#### jsファイルの変更
- jsファイル側は基本フリーフォーマットです。
画面ごとに関数が分かれているため、画面毎に設定値を直接設定します。  
cssファイル側では設定が難しい、座標やサイズを変更することができます。

- 簡易に書けるように、`$id(変更したいラベルやボタンのid名)`で対象のスタイルが取れるようにしています。  
下記2つは同じ内容です。  
```javascript
$id(`lblArrow`).left = `0px`;
document.querySelector(`#lblArrow`).style.left = `0px`;
```

## 2. customjs, musicUrlのカレントディレクトリ設定
- 上記のスキンと同様に、ダンおに本体と同じフォルダ上にjsファイルを置いて読み込ませることが可能になりました。
```
|skinType=(..)light| 
 -> ダンおに本体フォルダから danoni_skin_light.css, danoni_skin_light.js をスキンファイルとして読込
|settingType=(..)tickle| 
 -> ダンおに本体フォルダから danoni_setting_tickle.js を共通設定として読込
|musicUrl=(..)music.mp3| 
 -> ダンおに本体フォルダからmusic.mp3を読込
|customjs=danoni_custom.js,(..)75.js| 
 -> jsフォルダからdanoni_custom.jsを、ダンおに本体フォルダから75.jsを読込
```

## 3. danoni_setting.jsのグルーピング設定
- danoni_setting.js以外のファイルを共通設定として指定することができます。  
指定できるファイルはこれまで通り1つのままです。  
下記を指定した場合、「danoni_setting_**tickle**.js」がその作品の共通設定ファイルとなります。
```
|settingType=tickle| 
```

## 4. 画像ファイルの自動プリロード設定
- word/mask_data などの背景・マスクモーションに(.bmp/.png/.gif/.jpg)の記述があれば、  
譜面ヘッダー `preloadImages`に記述をしなくても自動でプリロードされるようになる機能を追加しました。  
譜面ヘッダー `autoPreload` を設定するだけで設定完了です。
```
|autoPreload=true|
```

## 5. 関数名の変更 (customjs利用者向け)
- 多くの箇所でCSSクラスを参照することになったため、関数名が変わりました。  
従来の関数はそのまま利用できます。

|v9まで|v10以後|
|----|----|
|createButton|createCssButton|
|createDivLabel|createDivCssLabel|
|makeSettingLblButton|makeSettingLblCssButton|
|makeDifLblButton|makeDifLblCssButton|
|makeMiniButton|makeMiniCssButton|
|makeResultPlayData|makeCssResultPlayData|
|makeResultSymbol|makeCssResultSymbol|
|createArrowEffect<br>createColorObject|createColorObject (統一)|

## 6. danoni_custom.js, danoni_setting.js の任意化
- 外部ファイルの読み込み関数の仕様が変わり、  
エラー時でも続行可となったことで実現しました。
```javascript
/**
 * 外部jsファイルの読込
 * @param {string} _url 
 * @param {function} _callback 
 * @param {boolean} _requiredFlg (default : true / 読込必須)
 * @param {string} _charset (default : UTF-8)
 */
function loadScript(_url, _callback, _requiredFlg = true, _charset = `UTF-8`) {
	const script = document.createElement(`script`);
	script.type = `text/javascript`;
	script.src = _url;
	script.charset = _charset;
	script.onload = _ => _callback();
	script.onerror = _ => {
		if (_requiredFlg) {
			makeWarningWindow(C_MSG_E_0041.split(`{0}`).join(_url.split(`?`)[0]));
		} else {
			_callback();
		}
	};
	document.querySelector(`head`).appendChild(script);
}
```

## 7. customBackUse, customBackMainUse の無効化 (スキン利用時)
- スキン利用時（Canvas未使用時）は背景描画のON/OFF機能が無効化されます。
- 代わりに、スキンのjs側で必要に応じて設定します。`#divBack`が背景用オブジェクトです。

### 設定例
```javascript
    divBack.style.background = `linear-gradient(#000000, #222222)`;
```

## 8. 矢印オブジェクトのグループ化
- 矢印やおにぎり画像について、`g_imgObj`でまとめて定義するようになりました。  
これにより、`g_imgObj`の値を変更することでオブジェクトの変更が可能となります。

```javascript
const g_imgObj = {
	// 矢印及び塗りつぶし部分
	arrow: C_IMG_ARROW,
	arrowShadow: C_IMG_ARROWSD,
	onigiri: C_IMG_ONIGIRI,
	onigiriShadow: C_IMG_AASD,
	giko: C_IMG_GIKO,
	gikoShadow: C_IMG_AASD,
	iyo: C_IMG_GIKO,
	iyoShadow: C_IMG_AASD,
	c: C_IMG_C,
	cShadow: C_IMG_AASD,
	morara: C_IMG_MORARA,
	moraraShadow: C_IMG_AASD,
	monar: C_IMG_MONAR,
	monarShadow: C_IMG_AASD,

	// ステップゾーン
	arrowStep: C_IMG_ARROW,
	arrowShadowStep: C_IMG_ARROWSD,
	onigiriStep: C_IMG_ONIGIRI,
	onigiriShadowStep: C_IMG_AASD,
	gikoStep: C_IMG_GIKO,
	gikoShadowStep: C_IMG_AASD,
	iyoStep: C_IMG_GIKO,
	iyoShadowStep: C_IMG_AASD,
	cStep: C_IMG_C,
	cShadowStep: C_IMG_AASD,
	moraraStep: C_IMG_MORARA,
	moraraShadowStep: C_IMG_AASD,
	monarStep: C_IMG_MONAR,
	monarShadowStep: C_IMG_AASD,

	// ヒットゾーン
	arrowStepHit: C_IMG_ARROW,
	onigiriStepHit: C_IMG_ONIGIRI,
	gikoStepHit: C_IMG_GIKO,
	iyoStepHit: C_IMG_GIKO,
	cStepHit: C_IMG_C,
	moraraStepHit: C_IMG_MORARA,
	monarStepHit: C_IMG_MONAR,

	// カーソル、フリーズアローバー、ライフ用バー、ボーダー表示
	cursor: C_IMG_CURSOR,
	frzBar: C_IMG_FRZBAR,
	lifeBar: C_IMG_LIFEBAR,
	lifeBorder: C_IMG_LIFEBORDER,
};
```

## 9. スクロール拡張に伴う派生機能について（v10.2.1以降）
- これまで通り、スクロール拡張をON/OFFする譜面ヘッダーとして`scrollUse`を用意しています。
以下のように指定することで無効化が可能です。
```
|scrollUse=false|
```
- 歌詞表示・背景／マスクモーション用に、スクロール拡張版を用意しています。
`wordAlt_data`, `backAlt_data`, `maskAlt_data` の3つで、使い方はリバース版と同じです。
「Cross」「Split」「Flat」などが指定された場合に優先的に適用されます。

## 10. ステップゾーンのグループ化について（重要）（v10.2.1以降）
- ステップゾーン関係のオブジェクトが`stepRootX`で一律管理されるようになりました。
座標変更している作品は`stepX` -> `stepRootX` へ変更が必要です。
```javascript
    document.querySelector(`#step0`).style.left = `50px`;  // 変更前
    document.querySelector(`#stepRoot0`).style.left = `50px`;  // 変更後
```

- またステップゾーンに回転を加えている場合、
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

## 11. 特殊キーのスクロール拡張について（v10.2.1以降）
- 特殊キーについてもスクロール拡張が可能です。以下のように設定できます。  
複数パターンある場合は$区切りですべて指定してください。  
ただし、デフォルトの設定は不要です。  
```
|scroll6=Cross::1,1,-1,-1,1,1/Split::1,1,1,-1,-1,-1/Alternate::1,-1,1,-1,1,-1$Cross::1,1,-1,-1,1,1/Split::1,1,1,-1,-1,-1/Alternate::1,-1,1,-1,1,-1|
```
