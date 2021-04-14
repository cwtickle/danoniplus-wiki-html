[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# multiAppend
### 概要
  - 子div要素をまとめて追加する関数。
  - 現状は [ParentNode.append()](https://developer.mozilla.org/ja/docs/Web/API/ParentNode/append) のラップ関数になっている。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_baseObj|object|*|親div要素|
|...rest|array|*|子div要素 (カンマ区切り)|

### 返却値
- なし

### 使用例
- 親要素`divRoot`に、子要素`lblC`, `btnTweet`を追加する例
```javascript
multiAppend(divRoot,
	// 背景の矢印オブジェクトを表示
	createColorObject2(`lblC`, {
		x: g_sWidth / 2 - 300, y: 0, w: 100, h: 100, rotate: `onigiri`, opacity: 0.25,
		background: `#ffffff`,
	}),
	// Infoボタン描画
	createCss2Button(`btnInfo`, `Info`, _ => clearTimeout(g_timeoutEvtTitleId), {
		x: g_sWidth / 4 * 3, y: 340, w: g_sWidth / 4,
		resetFunc: _ => customCommentInit(),
	}, g_cssObj.button_Tweet)
);
```
