[← 譜面ヘッダー仕様に戻る](dos_header.html)
## customBackMainUse
[ver2.x以降]

### 使い方
```
|customBackMainUse=false|
```
### 説明
タイトル画面の背景を個別に設定するか、デフォルトのものを使用するかを指定します。  
customBackUseとは異なり、メイン画面のみに適用されます。  
v10以降はskin側で設定できるため、Canvas未使用時は無効となっています。

|値|既定|内容|
|----|----|----|
|false|*|デフォルトの形式を採用|
|true||個別設定|

### 関連項目
- [customBackUse](dos-h0027-customBackUse.html)  背景(プレイ画面以外)
- [customReadyUse](dos-h0029-customReadyUse.html)  プレイ開始時演出
- [背景・マスクモーション (back_data, mask_data)](dos-e0004-animationData.html)  

### 更新履歴

|Version|変更内容|
|----|----|
|[v3.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.6.0)|デフォルト値変更 (true -> false)|
|[v2.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v2.1.0)|初回実装|