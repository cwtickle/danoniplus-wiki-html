[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# createCss2Button
### 概要
  - 座標、サイズ、フォントなどを設定したボタンを作成する。
  - 従来の関数`createCssButton`で使用できる属性値に加え、CSSに対応した属性名に対応する設定が行える。
  - この関数を呼び出しただけではボタンは作成されない。  
返却されたdiv要素を`(親div要素のid).append`や`multiAppend`関数などで追加する必要がある。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_id|string|*|ボタンのID名|
|_text|string|*|表示する文字列|
|_func|function|*|ボタンを押したときの処理|
|----|object||※下記のオブジェクト引数を参照|
|_classes|...any||CSSクラス名　※複数指定可|

### オブジェクト引数
- オブジェクト引数は全て任意。指定が無い場合はデフォルト値が採用される。
- CSS属性名については、div要素で使えるCSS属性が一通り使用できる。  
下記の例ではリストに無い`borderStyle`が指定されているが、CSS属性には存在するため指定が可能。  
他にも、`opacity`や`pointerEvents`, `display`といった項目が利用できる。
```javascript
spriteList.scroll.appendChild(
    createCss2Button(`btnReverse`, `${g_lblNameObj.Reverse}:${g_stateObj.reverse}`, evt => setReverse(evt.target), {
        x: 160, y: 0, w: 90, h: 21, siz: C_SIZ_DIFSELECTOR,
        borderStyle: `solid`,
        cxtFunc: evt => setReverse(evt.target),
    }, g_cssObj.button_Default, g_cssObj[`button_Rev${g_stateObj.reverse}`])
);
```

|引数|型|デフォルト|用途|
|----|----|----|----|
|x|number|0|ボタンのX座標|
|y|number|g_sHeight - 100|ボタンのY座標|
|w|number|g_sWidth / 3|ボタンの幅|
|h|number|50|ボタンの高さ|
|siz|number|28|ボタン文字のフォントサイズ|
|align|string|center|ボタン文字の位置|
|title|string||オンマウス時の説明表示文|
|groupName|string|g_currentPage|ボタンが所属するグループ。<br>既定はそのボタンが置かれている画面名。<br>ボタンの有効化までにかかる時間で利用。|
|initDisabledFlg|boolean|true|初期利用不可フラグ。<br>既定は利用不可で、指定時間後に利用可の設定。<br>ただし、`g_btnWaitFrame[グループ名].initial = true`となっている場合のみ、2回目以降は指定時間ゼロで使用できる。<br><br>※g_initialFlgを利用するため、事前に`g_initialFlg = false;`と`g_initialFlg = true;`を設定しておく必要がある。|
|resetFunc|function||左クリック時に実行する画面移動を伴う関数|
|cxtFunc|function||右クリック時に実行する関数|
|`属性名`|string||(CSS属性に対する設定。CSS属性であれば指定可)|

### 返却値
- この関数で作成したボタン（div要素）

### 使用例
- _obj内の要素については未指定の場合、デフォルトの値が適用される。
```javascript
divRoot.appendChild(
    createCss2Button(`btnKeyConfig`, `KeyConfig`, _ => {
        // ボタン処理エリア
        g_kcType = `Main`;
        clearWindow();
        keyConfigInit();
    }, {
        // CSSデザイン系変更エリア
        x: g_sWidth / 3,
    }, g_cssObj.button_Setting)   // CSSクラス
);

spriteList.scroll.appendChild(
    createCss2Button(`btnReverse`, `Reverse:${g_stateObj.reverse}`, evt => {
        setReverse(evt.target);
    }, {
        x: 160, y: 0,
        w: 90, h: 21, siz: C_SIZ_DIFSELECTOR,
        borderStyle: `solid`,
        cxtFunc: evt => setReverse(evt.target),
    }, g_cssObj.button_Default, g_cssObj[`button_Rev${g_stateObj.reverse}`])
);
```

### 関連項目
- [commonKeyDown](fnc-c0007-commonKeyDown.html)
- [**g_btnAddFunc** / **g_cxtAddFunc**](obj-v0018-g_btnAddFunc.html)
- [**g_btnDeleteFlg** / **g_cxtDeleteFlg**](obj-v0019-g_btnDeleteFlg.html)
- [**g_btnWaitFrame**](obj-v0020-g_btnWaitFrame.html)

### 更新履歴

|Version|変更内容|
|----|----|
|[v20.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v20.2.0)|・オブジェクト引数`groupName`, `initDisabledFlg`を実装|
|[v20.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v20.0.0)|・オブジェクト引数`resetFunc`を実装|
|[v17.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.5.0)|・オブジェクト引数`cxtFunc`を実装|
|[v17.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.0.0)|・初回実装|