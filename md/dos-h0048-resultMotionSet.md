[← 譜面ヘッダー仕様に戻る](dos_header.html)
## resultMotionSet

### 使い方
```
|resultMotionSet=false|
```
### 説明
リザルトモーションのON/OFFを、DisplayオプションのBackgroundのON/OFFと連動させるかを設定します。    

デフォルトは`true`(連動する)です。

|値|既定|内容|
|----|----|----|
|false||設定と連動しない|
|true|*|設定と連動する|

### 関連項目
- [maskresultButton](dos-h0044-maskresultButton.html)  リザルト画面上のボタン群の有効/無効設定
- [背景・マスクモーション (back_data, mask_data)](dos-e0004-animationData.html)  

### 更新履歴

|Version|変更内容|
|----|----|
|[v7.8.0](https://github.com/cwtickle/danoniplus/releases/tag/v7.8.0)|初回実装|