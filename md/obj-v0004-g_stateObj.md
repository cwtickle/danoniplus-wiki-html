[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_stateObj

### 概要
- 各種設定の状態を管理するオブジェクト。初期化時に作成される。  
- 設定画面やDisplay画面で表示される設定の変更と連動して、g_stateObjも変化する。
```javascript
g_stateObj.speed = 7;
g_stateObj.motion = `Brake`;
```

### 生成タイミング
- 初期に生成される。  
ただし、設定を変更するとそれに応じて値が変わる。

### プロパティと初期値
- scoreLockFlg (boolean): false
- scoreId (number): 0
- dummyId (string): ``
- speed (float): 3.5
- motion (string): `OFF`
- reverse (switch): `OFF`
- scroll (string): `---`
- shuffle (string): `OFF`
- autoPlay (string): `OFF`
- autoAll (switch): `OFF`
- gauge (string): `Normal`
- adjustment (number): 0
- fadein (number): 0
- volume (number): 100
- lifeRcv (float): 2
- lifeDmg (float): 7
- lifeMode (string): `Border`
- lifeBorder (float): 70
- lifeInit (float): 25
- lifeVariable (switch): `OFF`
- extraKeyFlg (boolean): false
- dataSaveFlg (boolean): true
- scoreDetailViewFlg (boolean): false
- scoreDetail (string): `Speed`
- d_stepzone (switch): `ON`
- d_judgment (switch): `ON`
- d_fastslow (switch): `ON`
- d_lifegauge (switch): `ON`
- d_musicinfo (switch): `ON`
- d_score (switch): `ON`
- d_filterline (switch): `ON`
- d_color (switch): `ON`
- d_speed (switch): `ON`
- d_arroweffect (switch): `ON`
- d_lyrics (switch): `ON`
- d_background (switch): `ON`
- d_special (switch): `ON`
- appearance (string): `Visible`
- opacity (number): 100
- realAdjustment (number) ※初期定義なし