[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# copyTextToClipboard
### 概要
- 引数に渡された文字列をクリップボードへコピーする関数。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_textVal|string|*|任意の文字列|

### 返却値
- コピーコマンドを実行した結果

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
