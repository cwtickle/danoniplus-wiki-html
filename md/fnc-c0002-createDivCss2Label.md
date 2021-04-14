[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# createDivCss2Label
### 概要
  - 座標、サイズ、フォントなどを設定したラベル用div要素を作成する。
  - 従来の関数`createDivCssLabel`で使用できる属性値に加え、CSSに対応した属性名に対応する設定が行える。
  - この関数を呼び出しただけではラベルは作成されない。  
返却されたdiv要素を`(親div要素のid).append`や`multiAppend`関数などで追加する必要がある。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_id|string|*|ラベルのID名|
|_text|string|*|表示する文字列|
|----|object||※下記のオブジェクト引数を参照|
|_classes|...any||CSSクラス名　※複数指定可|

### オブジェクト引数
- オブジェクト引数は全て任意。指定が無い場合はデフォルト値が採用される。

|引数|型|デフォルト|用途|
|----|----|----|----|
|x|number|0|ラベルのX座標|
|y|number|0|ラベルのY座標|
|w|number|210|ラベルの幅|
|h|number|23|ラベルの高さ|
|siz|number|17|ラベル文字のフォントサイズ|
|align|string|center|ラベル文字の位置|
|`属性名`|string||(CSS属性に対する設定。CSS属性であれば指定可)|

### 返却値
- この関数で作成したラベルdiv要素

### 使用例
```javascript
createDivCss2Label(`lblComment`, tmpComment, {
    x: 0, y: 70, w: g_sWidth, h: g_sHeight - 180, siz: C_SIZ_DIFSELECTOR, align: C_ALIGN_LEFT,
    overflow: `auto`, background: `#222222`, color: `#cccccc`, display: C_DIS_NONE,
});
```
上記記述と同じ定義を旧関数で行った場合：
```javascript
const lblComment = createDivCssLabel(`lblComment`, 0, 70, g_sWidth, g_sHeight - 180, C_SIZ_DIFSELECTOR, tmpComment);
lblComment.style.textAlign = C_ALIGN_LEFT;
lblComment.style.overflow = `auto`;
lblComment.style.background = `#222222`;
lblComment.style.color = `#cccccc`;
lblComment.style.display = C_DIS_NONE;
```

### 更新履歴

|Version|変更内容|
|----|----|
|[v17.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.0.0)|・初回実装|