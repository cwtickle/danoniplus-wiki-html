[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_gaugeOptionObj

### 概要
- ゲージ設定の初期値を管理するオブジェクト。   
譜面ヘッダーで指定するゲージの値に合わせて、`headerConvert ()`(一部は`loadDos()`)にて設定する。  
なおここで設定する値は基準値であり、danoni_setting.js や 譜面ヘッダーの値とマージされて決定される。
```javascript
const g_gaugeOptionObj = {
    survival: [`Original`, `Heavy`, `NoRecovery`, `SuddenDeath`, `Practice`, `Light`],
    border: [`Normal`, `Hard`, `SuddenDeath`, `Easy`],
    custom: [],
    customDefault: [],
    customFulls: {},

    initSurvival: [25, 50, 100, 100, 50, 25],
    rcvSurvival: [6, 2, 0, 0, 0, 12],
    dmgSurvival: [40, 50, 50, C_LFE_MAXLIFE, 0, 40],
    typeSurvival: [C_LFE_SURVIVAL, C_LFE_SURVIVAL, C_LFE_SURVIVAL, C_LFE_SURVIVAL, C_LFE_SURVIVAL, C_LFE_SURVIVAL],
    varSurvival: [C_FLG_OFF, C_FLG_OFF, C_FLG_OFF, C_FLG_OFF, C_FLG_OFF, C_FLG_OFF],
    clearSurvival: [0, 0, 0, 0, 0, 0],

    initBorder: [25, 100, 100, 25],
    rcvBorder: [2, 1, 0, 4],
    dmgBorder: [7, 50, C_LFE_MAXLIFE, 7],
    typeBorder: [C_LFE_BORDER, C_LFE_BORDER, C_LFE_SURVIVAL, C_LFE_BORDER],
    varBorder: [C_FLG_ON, C_FLG_ON, C_FLG_OFF, C_FLG_ON],
    clearBorder: [70, 0, 0, 70],

    varCustom: [],
    varCustomDefault: [],
    defaultList: [`survival`, `border`],
    defaultPlusList: [`survival`, `border`, `customDefault`],
};
```

### 生成タイミング
- 初回起動時、及び getGaugeSetting() 呼び出し時 (`headerConvert ()`, `loadDos()`内)

### プロパティ
#### ライフ制/ノルマ制/カスタムのゲージ設定種別
- survival (array)
- border (array)
- custom (array)
- customDefault (array) ※共通設定ファイルで`g_presetGaugeList`を指定した場合のリスト 
- customX (array) ※[customGauge](dos-h0053-customGauge.html)指定時、譜面毎に作成

#### 初期ライフ値、回復量、ダメージ量
- initSurvival (array)
- initBorder (array)
- rcvSurvival (array)
- rcvBorder (array)
- dmgSurvival (array)
- dmgBorder (array)

#### ライフ制/ノルマ制の設定別の区分
- typeSurvival (array)
- typeBorder (array)
- typeCustomX (array)  
※譜面ヘッダー：|[customGauge](dos-h0053-customGauge.html)X=survival|もしくは|[customGauge](dos-h0053-customGauge.html)X=border|指定時のみ作成

#### 回復・ダメージ量を矢印数依存とするかどうかの設定
- varSurvival (array)
- varBorder (array)
- varCustom (array)
- varCustomDefault (array) ※共通設定ファイルで`g_presetGaugeList`を指定した場合のリスト 
- varCustomX (array) ※[customGauge](dos-h0053-customGauge.html)指定時、譜面毎に作成

#### クリアするためのボーダーライン
- clearSurvival (array)
- clearBorder (array)

#### デフォルトゲージリスト
- defaultList (array) ※survival, border
- defaultPlusList (array) ※survival, border, customDefault

#### ゲージ個別指定する設定値のリスト
- customFulls (object)

#### 各ゲージ個別設定（headerConvert, loadDos関数で呼び出すgetGaugeSetting関数で作成）
※いずれも[gaugeX](dos-h0022-gaugeX.html)の指定があった場合のみ作成。
  
- gaugeNormals
  - lifeBorders, lifeRecoverys, lifeDamages, lifeInits (array)
- gaugeEasys
- gaugeHards
- gaugeOriginals
- gaugeLights
- gaugeHeavys
- gaugeNoRecoverys

### 補足：dmgSurvival, dmgBorderにおけるライフ最大値仕様について
- これらは初期起動時に仮指定されるが、  
ライフ最大値については`headerConvert()`を通過しないとわからない。
- 仮指定時の文字として C_LFE_MAXLIFE (=`maxLife`) を割り当て、`headerConvert()`通過時に設定。  
本来は数字が入る箇所のため、カスタムで上書きする場合は直接数字を入れること。

|Version|変更内容|
|----|----|
|[v21.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.1.0)|・譜面毎のカスタムゲージリストに合わせてプロパティ追加|
|[v1.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|・初回実装|