[← 譜面ヘッダー仕様に戻る](dos_header.html)
## customReadyUse
[ver2.x以降]

### 使い方
```
|customReadyUse=false|
```
### 説明
メイン画面のReady?を個別に設定(もしくは非表示)するか、デフォルトのものを使用するかを指定します。  

|値|既定|内容|
|----|----|----|
|false|*|デフォルトの形式を採用|
|true||個別設定|

### 関連項目
- [readyDelayFrame](dos-h0052-readyDelayFrame.html)  Ready?が表示されるまでの遅延フレーム数
- [customBackUse](dos-h0027-customBackUse.html)  背景(プレイ画面以外)

### 更新履歴

|Version|変更内容|
|----|----|
|[v3.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.6.0)|デフォルト値変更 (true -> false)|
|[v2.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v2.1.0)|初回実装|