[← 譜面ヘッダー仕様に戻る](dos_header.html)
## motionUse / scrollUse / shuffleUse / autoPlayUse / gaugeUse / appearanceUse

### 使い方
```
|motionUse=false|
|scrollUse=false|
|shuffleUse=false|
|autoPlayUse=false|
|gaugeUse=false|
|appearanceUse=false|
```
### 説明
設定画面の項目「Motion」「Scroll」「Shuffle」「AutoPlay」「Gauge」「Appearance」を作品の都合上使用させない場合に使用します。  
「ScrollUse」については、falseにした場合でもReverseは設定可能です。  

|値|既定|内容|
|----|----|----|
|false||設定変更不可|
|true|*|設定変更可|

### 使用例
- 上記の「使い方」に記載のオプションを全て適用（使用禁止）した場合

![dos-h0035-01.png](./wiki/dos-h0035-01.png)

### 補足
- danoni_setting.jsの`g_presetSettingUse`で作品共通に指定できます。  
両方指定があった場合、譜面ヘッダー側 (settingUse) が優先されます。  

```javascript
const g_presetSettingUse = {
	motion: `true`,
	scroll: `true`,
	shuffle: `true`,
	autoPlay: `true`,
	gauge: `true`,
	appearance: `true`,
};
```

### 関連項目
- [displayUse](dos-h0057-displayUse.html)  Display項目の利用有無, 初期値設定
   - stepZoneUse, judgmentUse, fastSlowUse, ... etc
- [transKeyUse](dos-h0024-transKeyUse.html)  別キーモードの利用有無
- [customGauge](dos-h0053-customGauge.html)  カスタムゲージ設定
- [**gaugeX**](dos-h0022-gaugeX.html)  ゲージ設定の詳細

### 更新履歴

|Version|変更内容|
|----|----|
|[v10.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v10.2.1)|スクロール拡張実装に伴い、Scrollの利用有無設定を追加|
|[v9.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v9.0.0)|Appearance実装に伴い、Appearanceの利用有無設定を追加|
|[v3.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.1.0)|初回実装|