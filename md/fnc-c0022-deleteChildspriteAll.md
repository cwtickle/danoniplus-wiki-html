[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# deleteChildspriteAll
### 概要
- 引数に指定したオブジェクトID配下の子オブジェクト、並びにボタンに付属しているListenerを削除する関数。
- 引数に指定したオブジェクト自体は削除の起点となるだけで、削除はされない。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_parentObjName|string|*|削除起点のオブジェクト|

### 返却値
- なし

### 使用例
```javascript
/**
 * 譜面変更セレクターの削除
 */
const resetDifWindow = _ => {
	if (document.querySelector(`#difList`) !== null) {
		deleteChildspriteAll(`difList`);
		optionsprite.removeChild(document.querySelector(`#difList`));
		optionsprite.removeChild(document.querySelector(`#difCover`));
	}
};
```
