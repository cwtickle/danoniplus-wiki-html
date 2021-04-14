[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# createColorObject2
### 概要
  - 座標、サイズ、色情報などを設定した色付きオブジェクト（矢印・フリーズアロー他）を作成する。
  - 従来の関数`createColorObject`で使用できる属性値に加え、CSSに対応した属性名に対応する設定が行える。
  - この関数を呼び出しただけではオブジェクトは作成されない。  
返却されたdiv要素を`(親div要素のid).append`や`multiAppend`関数などで追加する必要がある。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_id|string|*|色付きオブジェクトのID名|
|----|object||※下記のオブジェクト引数を参照|
|_classes|...any||CSSクラス名　※複数指定可|

### オブジェクト引数
- オブジェクト引数は全て任意。指定が無い場合はデフォルト値が採用される。

|引数|型|デフォルト|用途|
|----|----|----|----|
|x|number|0|オブジェクトのX座標|
|y|number|0|オブジェクトのY座標|
|w|number|50|オブジェクトの幅|
|h|number|50|オブジェクトの高さ|
|background|string|''|オブジェクト色|
|rotate|string|''|オブジェクトの回転量|
|styleName|string|''|オブジェクト名|
|`属性名`|string||(CSS属性に対する設定。CSS属性であれば指定可)|

### 使用例

```javascript

const step = createColorObject2(`step${j}`, {
  rotate: g_workObj.stepRtn[j], styleName: `Step`,
}, g_cssObj.main_stepDefault);
stepRoot.appendChild(step);

frzHit.appendChild(
  createColorObject2(`frzHitTop${j}`, {
    x: -8, y: -8, w: C_ARW_WIDTH + 16, h: C_ARW_WIDTH + 16,
    rotate: g_workObj.arrowRtn[j], styleName: `Shadow`,
  }, g_cssObj.main_frzHitTop)
);
```

### 更新履歴

|Version|変更内容|
|----|----|
|[v17.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.0.0)|・初回実装|