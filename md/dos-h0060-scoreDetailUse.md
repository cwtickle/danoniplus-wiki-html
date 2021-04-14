[← 譜面ヘッダー仕様に戻る](dos_header.html)
## scoreDetailUse

### 使い方
```
|scoreDetailUse=false|
```
### 説明
設定画面において譜面の速度変化の遷移グラフ、譜面密度分布といった詳細表示を行うかどうかを設定します。  
指定しない場合は `true`(譜面明細表示を行う)。  

|値|既定|内容|
|----|----|----|
|false||譜面明細表示を使用しない|
|true|*|譜面明細表示を使用する<br>（速度変化グラフ、譜面密度グラフなどを表示するボタンが追加される）|

### 関連項目
- [startFrame](dos-h0005-startFrame.html) (★)  プレイ開始フレーム数 

### 更新履歴

|Version|変更内容|
|----|----|
|[v11.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v11.3.0)|初回実装|