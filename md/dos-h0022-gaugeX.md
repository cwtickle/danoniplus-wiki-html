[← 譜面ヘッダー仕様に戻る](dos_header.html)
## gaugeNormal / gaugeEasy / gaugeHard<br>(ノルマ制ゲージ)

### 使い方
```
|gaugeEasy=70,2,5,40$70,5,7,30| // 2譜面分をまとめて記述
|gaugeHard=x,1,50,100|  // 全譜面共通の設定

|gaugeExHard=x,1,70,100| // 1譜面目
|gaugeExHard2=x,1,80,100| // 2譜面目
```
### 説明
ゲージパラメータの設定を記述します。 
 
gaugeNormal, gaugeEasy, gaugeHardがそれぞれNormal, Easy, Hardゲージの設定です。  
"$"区切りで譜面ごとの設定で、  
さらにカンマ区切りでノルマ割合、ライフ増加・減少割合、初期ライフ割合を指定します。  
カンマ区切りの内容は次の通りです。  

|番号|設定例|内容|
|----|----|----|
|1|70|対象譜面が達成すべきノルマ率を0～100で指定します。<br>0を指定した場合、ライフが0になるとゲームオーバーです。|
|2|2|対象譜面のライフ増加割合を0～100で指定します。|
|3|5|対象譜面のライフ減少割合を0～100で指定します。|
|4|40|対象譜面の初期ライフ割合を0～100で指定します。|

### 未設定時の既定値について (ノルマ制ゲージ)
当パラメータが未設定の場合、`danoni_setting.js`を参照します。  
そこにも定義されていない場合は、下記の値が適用されます。  

|ゲージ種類|ノルマ|回復割合|ダメージ割合|初期ライフ割合|
|----|----|----|----|----|
|Normal|70%|2|7|25%|
|Easy|70%|4|7|25%|
|Hard|0|1|50|100%|

1譜面目の設定をgauge***で行っているが2譜面目の設定はない場合、一律以下の設定になります。  
→ノルマ70%、ライフ増加2、ライフ減少7、初期ライフ25%

## gaugeOriginal / gaugeLight / gaugeHeavy / gaugeNoRecovery<br>(ライフ制ゲージ)

### 使い方
```
|gaugeLight=x,20,70,30$x,30,40,30|
|gaugeNoRecovery=x,0,100,100$|
```
### 説明
ゲージパラメータの設定を記述します。 
 
gaugeOriginal, gaugeLight, gaugeHeavy, gaugeNoRecoveryがそれぞれ  
Original, Light, Heavy, NoRecoveryゲージの設定です。  
"$"区切りで譜面ごとの設定で、  
さらにカンマ区切りでノルマ割合、**ライフ増加・減少量(固定)**、初期ライフ割合を指定します。  
カンマ区切りの内容は次の通りです。  

|番号|設定例|内容|
|----|----|----|
|1|x|x固定。|
|2|30|対象譜面の**ライフ増加量**を指定します。|
|3|70|対象譜面の**ライフ減少量**を指定します。|
|4|40|対象譜面の初期ライフ割合を0～100で指定します。|

### 未設定時の既定値について (ライフ制ゲージ)
当パラメータが未設定の場合、`danoni_setting.js`を参照します。  
そこにも定義されていない場合は、下記の値が適用されます。  

|ゲージ種類|ノルマ|回復量|ダメージ量|初期ライフ割合|
|----|----|----|----|----|
|Original|-|6|40|25%|
|Light|-|12|40|25%|
|Heavy|-|2|50|50%|
|NoRecovery|-|0|50|100%|

### 関連項目
- [**difData**](dos-h0002-difData.html) (★)  譜面情報 
- [customGauge](dos-h0053-customGauge.html)  カスタムゲージ設定
- [maxLifeVal](dos-h0045-maxLifeVal.html)  ライフの上限値
- [frzStartjdgUse](dos-h0037-frzStartjdgUse.html)  フリーズアロー開始判定の設定有無
- [frzAttempt](dos-h0038-frzAttempt.html)  フリーズアローヒット時の許容フレーム数

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.1.0)|・2譜面目以降の分割書式に対応|
|[v19.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.0.0)|・2譜面目以降が未指定の場合、1譜面目の設定で補完する設定を追加|
|[v18.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.6.0)|・gaugeHeavy (ライフ制ゲージ)を実装|
|[v9.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.0)|・gaugeXXXを実装（XXXは任意のカスタムゲージ名）|
|[v6.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v6.5.0)|・gaugeOriginal / gaugeLight / gaugeNoRecovery (ライフ制ゲージ)を実装。<br>・既定値をゲージ設定ごとに個別設定できるように変更|
|[v1.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.5.0)|初回実装|