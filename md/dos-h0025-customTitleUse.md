[← 譜面ヘッダー仕様に戻る](dos_header.html)
## customTitleUse
[ver2.x以降]

### 使い方
```
|customTitleUse=false|
```
### 説明
タイトル画面の曲名文字の形式を個別に設定するか、デフォルトのものを使用するかを指定します。   

|値|既定|内容|
|----|----|----|
|false|*|デフォルトの形式を採用|
|true||個別設定|

### customTitleUse の適用範囲
![dos-h0025-01.png](./wiki/dos-h0025-01.png)

### 関連項目
- [customTitleArrowUse](dos-h0026-customTitleArrowUse.html)  タイトルの背景矢印
- [customBackUse](dos-h0027-customBackUse.html)  背景(プレイ画面以外)
- [背景・マスクモーション (back_data, mask_data)](dos-e0004-animationData.html)  

### 更新履歴

|Version|変更内容|
|----|----|
|[v3.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.6.0)|デフォルト値変更 (true -> false)|
|[v2.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v2.1.0)|初回実装|