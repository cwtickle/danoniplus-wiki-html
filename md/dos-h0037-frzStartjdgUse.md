[← 譜面ヘッダー仕様に戻る](dos_header.html)
## frzStartjdgUse
### 使い方
```
|frzStartjdgUse=true|
```
### 説明
フリーズアローが最初に押されたタイミングで判定を取るかどうかを指定します。  
指定しない場合は false。  

フリーズアロー開始判定を使用した場合、それに合わせてスコアも修正されます。  
(矢印総数が変わるため)  

|値|既定|内容|
|----|----|----|
|false|*|フリーズアロー開始判定を使用しない|
|true||フリーズアロー開始判定を使用する|

### 関連項目
- [customGauge](dos-h0053-customGauge.html)  カスタムゲージ設定
- [**gaugeX**](dos-h0022-gaugeX.html)  ゲージ設定の詳細
- [frzAttempt](dos-h0038-frzAttempt.html)  フリーズアローヒット時の許容フレーム数

### 更新履歴

|Version|変更内容|
|----|----|
|[v5.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v5.7.0)|初回実装|