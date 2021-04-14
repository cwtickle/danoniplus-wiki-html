# オブジェクトリファレンス
- danoni_main.js で定義されており、cumtom側で制御できるオブジェクトを定義する。

## ライフゲージ

|変数名|規定値|内容|
|----|----|----|
|C_CLR_MAXLIFE|#440000|ライフゲージのライフがMAX時の色|
|C_CLR_CLEARLIFE|#004444|ノルマ以上のライフ時の色|
|C_CLR_DEFAULTLIFE|#444444|ノルマ未満のライフ時の色|
|C_CLR_BORDER|#555555|ノルマ位置を示す数字の背景色|
|C_CLR_BACKLIFE|#222222|ライフゲージの裏側の背景色|

## 判定許容フレーム数 (g_judgObj)

### arrowJ
- 矢印の許容フレーム数。  
左から「イイ」「シャキン」「マターリ」「ショボーン」の許容フレーム数、  
「ウワァン」の判定開始フレーム数を表す。  
```javascript
g_judgObj.arrowJ = [2, 4, 6, 8, 8];
```

### frzJ
- フリーズアローの許容フレーム数。  
左から「キター」「セフセフ」の許容フレーム数、  
「イクナイ」の判定開始フレーム数を表す。　※セフセフは未実装
```javascript
g_judgObj.frzJ = [2, 4, 8];
```

## ランク表示 (g_rankObj)

### rankMarks
```javascript
g_rankObj.rankMarks = ["SS", "S", "SA", "AAA", "AA", "A", "B"];
```
- ランク文字の定義。上位ランク順に記載する。
- PF, C, Fランクは別定義。

### rankRate
```javascript
g_rankObj.rankRate = [97, 90, 85, 80, 75, 70, 50];
```
- ランクの獲得条件(総スコアのパーセント表記)。数字必須。  
- rankMarksと同じ配列数とすること。  

### rankColor
```javascript
g_rankObj.rankColor = ["#00ccff", "#6600ff", "#ff9900", "#ff0000", "#00ff00", "#ff00ff", "#cc00ff"];
```
- ランクの色。カラーコード指定。  
- rankMarksと同じ配列数とすること。  


## function: setVal
- 変数の中身の型をチェックし、指定された型に変換する。
- 不適切な値の場合は、デフォルト値を返却する。
- undefinedやNaN、空白など、扱いにくい変数が入りそうなときに  
チェックを兼ねて使用する。

|引数|型|内容|
|----|----|----|
|_checkStr|string|型チェック対象の変数|
|_defaultStr|string|型チェックがNGの場合のデフォルト値|
|_type|string|チェックする型<br>("number":整数, "float":小数, "string":文字列)|

### 返却値
- _checkStrを指定された型に変換した値 (変換できない場合は _defaultStr を返却)

### 使用例
```javascript
const checkStr = "abc123";
const returnStr1 = setVal(checkStr, "a", "string");  // abc123
const returnStr2 = setVal(checkStr, 0, "number");    // 0
```

## function: createSprite
- 空のスプライト(オブジェクト)を作成する。  
- すでに同じ名前のスプライトが存在する場合は、作成済のスプライトを返却する。  
- 関数内でappendChild(子要素追加)を呼び出しているため、即画面反映される。  

|引数|型|内容|
|----|----|----|
|_parentObjName|string|親スプライト名|
|_newObjName|string|作成する子スプライト名|
|_x|number|作成するスプライトのx座標（親スプライト基準）|
|_y|number|作成するスプライトのy座標（親スプライト基準）|
|_width|number|作成するスプライトの幅|
|_height|number|作成するスプライトの高さ|

### 返却値
- _newObjNameで指定したスプライト(オブジェクト)

### 使用例
```javascript
// divRoot上の座標(x, y) = (100, 50)の位置に、400px × 300pxの空スプライト「mysprite」を作成する。
const mysprite = createSprite("divRoot", "mysprite", 100, 50, 400, 300);
```

## function: deleteChildspriteAll
- 親スプライト(オブジェクト)配下のスプライトを全削除する。  
- 親スプライト自体は削除されない。  

|引数|型|内容|
|----|----|----|
|_parentObjName|string|親スプライト名|

### 返却値
- 無し

### 使用例
```javascript
deleteChildspriteAll("mysprite");
```

## function: createButton
- 汎用ボタンを作成する。  
- ボタンを押したときの処理を記述できる。  
- オンマウス時のポインタ変更、ボタン色変更は関数の中で自動適用されている。  

|引数|型|内容|
|----|----|----|
|_obj|object|ボタンのスタイル設定|
|_func|function|ボタンを押したときの処理|

### _objで保持が必要なプロパティ

|プロパティ|型|内容|
|----|----|----|
|id|string|ボタンオブジェクト名|
|name|string|ボタンに表示するテキスト|
|x|number|作成先のx座標 (appendChildする親に対する位置)|
|y|number|作成先のy座標 (appendChildする親に対する位置)|
|width|number|ボタンの幅|
|height|number|ボタンの高さ|
|fontsize|number|文字サイズ|
|normalColor|string|通常時のボタンの背景色(カラーコード指定)|
|hoverColor|string|オンマウス時のボタンの背景色(カラーコード指定)|
|align|string|テキスト表示位置|

### 返却値
- ボタンオブジェクト

### 使用例
```javascript

// ボタン描画
const btnStart = createButton({
  id: "btnStart",
  name: "Click Here!!",
  x: 0,
  y: g_sHeight - 100,
  width: g_sWidth,
  height: C_BTN_HEIGHT,
  fontsize: C_LBL_TITLESIZE,
  normalColor: C_CLR_DEFAULT,
  hoverColor: C_CLR_DEFHOVER,
  align: C_ALIGN_CENTER
}, function () {
  // ボタン押下後の処理
  clearWindow();
  optionInit();
});

// ボタン作成後はappendChildが必須
divRoot.appendChild(btnStart);
```

## function: g_handler.addListener
- イベントハンドラの追加
- addEventListenerと異なり、リスナーキーを返却するためListenerの消し忘れに有効。   

|引数|型|内容|
|----|----|----|
|_target|object|対象スプライト|
|_type|string|対象のイベント名(click, touchstartなど)|
|_listener|function|イベントをトリガーとする処理|
|_capture|boolean|イベント伝播方法。addEventListenerのuseCaptureと同じ。|

### 返却値
- リスナーキー(number)

### 使用例
```javascript
// divオブジェクトに対してタップしたときのイベントを追加
const lsnrkeyTS = g_handler.addListener(div, "touchstart", function () {
  div.style.backgroundColor = _obj.hoverColor;
  div.style.cursor = "pointer";
}, false);

// イベントリスナー用のキーをセット
div.setAttribute("lsnrkeyTS", lsnrkeyTS);
```

## function: g_handler.removeListener
- イベントハンドラの削除   

|引数|型|内容|
|----|----|----|
|_key|number|リスナーキー|

### 返却値
- 無し

### 使用例
```javascript
// divRootの子要素のイベントハンドラを削除
while (divRoot.hasChildNodes()) {
  g_handler.removeListener(divRoot.firstChild.getAttribute("lsnrkeyTS"));
}
```