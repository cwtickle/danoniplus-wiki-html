[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# createScText
### 概要
  - ショートカットキーの画面表示を行う関数。
  - [g_shortcutObj](obj-v0017-g_shortcutObj.html)よりボタンに対応するショートカットキーが存在すれば、  
そのキーを指定した親オブジェクト（ボタンも指定可）の左上に表示する。
  - ショートカットキーが存在しない場合は何も表示しない。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_obj|object|*|ショートカット表示を行う対象の親オブジェクト|
|_settingLabel|string|*|ラベルに指定する任意の名前|
|----|object||※下記のオブジェクト引数を参照|

### オブジェクト引数
- オブジェクト引数は全て任意。指定が無い場合はデフォルト値が採用される。

|引数|型|デフォルト|用途|
|----|----|----|----|
|displayName|string|option|画面名|
|dfLabel|string||ショートカットキー表示に使用する代替文字列。<br>未指定の場合はg_shortcutObjに対応するキー名を表示する。<br>複数キーの組み合わせの場合、対応するキー名が取得できないため、この項目がある。|
|targetLabel|string|`lnk${_settingLabel}R`|ショートカットキーを検索するボタンのID名。<br>通常は_objと同じ名前のIDになるが、設定画面の各項目では右回り・左回りで複数のボタンがあるため、この項目がある。|
|x|number|95|ショートカットキー表示位置のX座標|

### 返却値
- なし

### 使用例
```javascript
createScText(spriteList.difficulty, `Difficulty`);
createScText(lnkScoreDetail, `ScoreDetail`, { targetLabel: `lnkScoreDetail`, x: -10 })
```

### 補足
- 親オブジェクトの子要素にテキストを表示するため、  
親オブジェクトがボタンの場合でそのボタンのテキスト表示が変わってしまうような場合は注意が必要。
```javascript
// ショートカット表示作成用関数を定義
const viewScText = _ => createScText(lnkScoreDetail, `ScoreDetail`, { targetLabel: `lnkScoreDetail`, x: -10 });

// ボタン作成処理
multiAppend(scoreDetail,
    /* 省略 */
    makeSettingLblCssButton(`lnkScoreDetail`, `${g_stateObj.scoreDetail}`, 0, _ => {
        /* 省略 */
        // クリックすると値が書き換わるため、再度ショートカット表示作成用関数を呼び出して追記
        setSetting(1, `scoreDetail`);
        viewScText();
        /* 省略 */
    }, {
        x: 10, w: 100, borderStyle: `solid`,
    }, g_cssObj.button_RevON),
);

// ボタン作成後初回表示
viewScText();
```

### 関連項目
- [**g_shortcutObj**](obj-v0017-g_shortcutObj.html)
- [createScTextCommon](fnc-c0034-createScTextCommon.html)

### 更新履歴

|Version|変更内容|
|----|----|
|[v19.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.5.0)|・初回実装|