[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# makeInfoWindow
### 概要
- 画面上部に一定時間(2.5秒)、常時手前表示のメッセージウィンドウを表示する関数。
- 2番目の引数にCSSに対応するアニメーション名を指定することができる。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_text|string|*|メッセージウィンドウに表示するテキスト|
|_animationName|string||CSSアニメーション名|


### 返却値
- なし

### 関数の依存関係
- makeInfoWindow
  - getTitleDivLabel
  - setWindowStyle

### 使用例
```javascript
// リザルトデータをクリップボードへコピー
createCss2Button(`btnCopy`, g_lblNameObj.b_copy, _ => {
	copyTextToClipboard(resultText);
	makeInfoWindow(g_msgInfoObj.I_0001, `leftToRightFade`);
}, {
	x: g_sWidth / 4,
	w: g_sWidth / 2,
	h: C_BTN_HEIGHT * 5 / 8, siz: 24,
	animationName: `smallToNormalY`,
}, g_cssObj.button_Setting),
```

### 関連項目
- [makeWarningWindow](fnc-c0013-makeWarningWindow.html)
- setWindowStyle

### 更新履歴

|Version|変更内容|
|----|----|
|[v16.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v16.1.0)|・初回実装|