[← 譜面ヘッダー仕様に戻る](dos_header.html)
## customGauge
### 使い方
```
|customGauge=Original::F,Normal::V,Escape::V|
|customGauge2=Original::F,Normal::V,Escape::V,SuddenDeath::F|
|customGauge3=customDefault| // 共通設定ファイルより g_presetGaugeList に設定されたリストを継承
|customGauge4=survival|      // ライフ制ゲージの設定を継承
|customGauge5=border|        // ノルマ制ゲージの設定を継承

|gaugeOriginal=x,4,60,25$x,3,20,25|
|gaugeNormal=50,70,1,25$x,3,25,25|
|gaugeEscape=0,1,50,100$x,5,30,25|
```

### 説明
- [gaugeX](dos-h0022-gaugeX.html)と合わせて使用します。
- カンマ区切りで、ゲージ設定毎の設定を行います。  
「ゲージ名::回復/ダメージ量設定」の組み合わせで設定します。  
回復/ダメージ量設定は、「F」なら矢印数によらず固定、  
「V」なら矢印数により変動します。  
- ライフ制/ノルマ制の区別は各個別のゲージ設定([gaugeX](dos-h0022-gaugeX).html)にて行います。  
このため、ノルマ制ながら回復/ダメージ量は固定にするといった設定が可能になります。  

#### 特殊な指定方法
- 既存のゲージ設定リストを継承する設定が可能です。

|設定名|継承先のリスト|
|----|----|
|survival|ライフ制ゲージ<br>[`Original`, `Heavy`, `NoRecovery`, `SuddenDeath`, `Practice`, `Light`]|
|border|ノルマ制ゲージ<br>[`Normal`, `Hard`, `SuddenDeath`, `Easy`]|
|customDefault|共通設定ファイルの g_presetGaugeList で定義されたリスト|

### 補足
- カスタムゲージを指定した場合は [gaugeX](dos-h0022-gaugeX.html) の指定 もしくは  
`danoni_setting.js`の`g_presetGaugeCustom`の設定が必須です。  
また、OriginalとNormalがデフォルトゲージで無い場合についても、  
設定が必須となります。ご注意ください。  
- 原則、ライフ設定は [difData](dos-h0002-difData.html) ではなく [gaugeX](dos-h0022-gaugeX.html) で行い、  
自動設定されているゲージ設定についても、個別に設定してください。
- カスタムゲージを設定した場合、その作品全体でゲージ設定が共有されます。  
譜面個別にゲージ設定を設定する場合は、customGauge2, customGauge3, ...で指定します。
- `danoni_setting.js`の`g_presetGaugeCustom`に追加するゲージ設定を記載することで  
どの作品に対してもカスタムゲージを適用できるようになります。

```javascript
// ゲージ設定（デフォルト以外）
const g_presetGaugeCustom = {
	// (省略)
	Escape: {
		Border: 70,
		Recovery: 1,
		Damage: 50,
		Init: 70,
	},
};
```

### 関連項目
- [**difData**](dos-h0002-difData.html) (★)  譜面情報 
- [**gaugeX**](dos-h0022-gaugeX.html)  ゲージ設定の詳細
- [maxLifeVal](dos-h0045-maxLifeVal.html)  ライフの上限値
- [frzStartjdgUse](dos-h0037-frzStartjdgUse.html)  フリーズアロー開始判定の設定有無
- [frzAttempt](dos-h0038-frzAttempt.html)  フリーズアローヒット時の許容フレーム数

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.1.0)|・2譜面目以降の個別設定、既存リスト継承設定に対応|
|[v9.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.0)|・初回実装|