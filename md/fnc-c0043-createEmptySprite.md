[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# createEmptySprite
### 概要
- 空のスプライトを作成する関数。すでにある場合はCSS属性を適用後、すでにあるスプライトを返却する。
- `(親div要素のid).appendChild`が含まれているため、特別に追加しなくても画面上に反映される。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_parentObj|object|*|親div要素のオブジェクト|
|_newObjId|string|*|子スプライト(div要素)の名前|
|----|object||※下記のオブジェクト引数を参照|
|_classes|...any||CSSクラス名　※複数指定可|

### オブジェクト引数
- オブジェクト引数は全て任意。指定が無い場合はデフォルト値が採用される。

|引数|型|デフォルト|用途|
|----|----|----|----|
|x|number|0|子スプライトのX座標|
|y|number|0|子スプライトのY座標|
|w|number|g_sWidth|子スプライトの幅|
|h|number|g_sHeight|子スプライトの高さ|
|title|string||子スプライトのオンマウステキスト|
|`属性名`|string||(CSS属性に対する設定。CSS属性であれば指定可)|

### 返却値
- この関数で作成した子スプライト（div要素）

### 使用例
```javascript
const difList = createEmptySprite(optionsprite, `difList`, { x: 165, y: 65, w: 280, h: 255, overflow: `auto` }, g_cssObj.settings_DifSelector);
const difCover = createEmptySprite(optionsprite, `difCover`, {
	x: 25, y: 65, w: 140, h: 255, overflow: `auto`, opacity: 0.95
}, g_cssObj.settings_DifSelector);
```

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.3.0)|・初回実装|