[← 譜面ヘッダー仕様に戻る](dos_header.html)
## transKeyUse
[ver4.8以降]

### 使い方
```
|transKeyUse=false|
```
### 説明
11keyの譜面を11Lkeyとしてプレイするような、別キーモードを許可するかどうかを指定します。  
指定しない場合は `true`。  

|値|既定|内容|
|----|----|----|
|false|*|別キー利用を許可しない|
|true||別キー利用を許可する|

### 別キーモードの例
- 下記は11Lkeyの譜面ですが、11keyを別キーとしてプレイできることを示す例です。  
別キーモード時は正規譜面として扱われず、  
ハイスコアやキーコンフィグ保存は使用できなくなっています。  
キーが変わるとステップゾーンの描画位置が変わることがあるため、  
必要に応じて譜面ヘッダー「transKeyUse」を使用し制限を掛けます。

![dos-h0024-01.png](./wiki/dos-h0024-01.png)

### 関連項目
- [**settingUse**](dos-h0035-settingUse.html)  設定項目の利用有無
   - motionUse, scrollUse, shuffleUse, ... etc
- [displayUse](dos-h0057-displayUse.html)  Display項目の利用有無, 初期値設定
   - stepZoneUse, judgmentUse, fastSlowUse, ... etc

### 更新履歴

|Version|変更内容|
|----|----|
|[v4.8.0](https://github.com/cwtickle/danoniplus/releases/tag/v4.8.0)|初回実装|