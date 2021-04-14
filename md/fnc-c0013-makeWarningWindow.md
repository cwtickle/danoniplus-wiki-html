[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# makeWarningWindow
### 概要
- 画面上部に常時手前表示の警告用メッセージウィンドウを表示する関数。
- [makeInfoWindow](fnc-c0012-makeInfoWindow.html)とは常時表示する点と複数追記ができる点が異なる。
- このメッセージウィンドウはver21.1.0までは画面切り替えを行った際（clearWindow呼び出し時）にリセットされる仕様だったが、
ver21.2.0以降は基本保持される仕様に変更された。  
メッセージは`g_errMsgObj`の画面別プロパティに格納される仕様になっている。  
第二引数の`resetFlg`を`true`にした場合、この画面別プロパティがクリアされる。（デフォルトは`false`）

#### 警告メッセージ格納イメージ
```html
<p>
お使いのブラウザは動作保証外です。<br>
Chrome/Opera/Vivaldiなど、WebKit系ブラウザの利用を推奨します。(W-0001)
</p>
<p>
fileスキームでの動作のため、内蔵の画像データを使用します。(W-0011)<br>
imgフォルダ以下の画像の変更は適用されません。
</p>
```

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_text|string|*|メッセージウィンドウに追記するテキスト|
|_resetFlg|boolean||メッセージをリセットするかどうかのフラグ (false:リセットしない / true:リセットする)|

### 返却値
- なし

### 関数の依存関係
- makeWarningWindow
  - getTitleDivLabel
  - setWindowStyle

### 使用例
- 下記の場合、該当する場合は`W_0001`, `W_0011`に対応するメッセージを同時に表示
```javascript
// 非推奨ブラウザに対して警告文を表示
// Firefoxはローカル環境時、Ver65以降矢印が表示されなくなるため非推奨表示
if (g_userAgent.indexOf(`msie`) !== -1 ||
	g_userAgent.indexOf(`trident`) !== -1 ||
	g_userAgent.indexOf(`edge`) !== -1 ||
	(g_userAgent.indexOf(`firefox`) !== -1 && location.href.match(`^file`))) {

	makeWarningWindow(g_msgInfoObj.W_0001);
}

if (location.href.match(/^file/)) {
	makeWarningWindow(g_msgInfoObj.W_0011);
}
```

### 関連項目
- [makeInfoWindow](fnc-c0012-makeInfoWindow.html)
- setWindowStyle

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.2.0)|・引数`resetFlg`を追加|
|[v16.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v16.1.0)|・makeInfoWindow関数との共通部をsetWindowStyle関数へ切り出し|
|[v1.0.0<br>(v0.59.x)](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|・初回実装|