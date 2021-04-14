[← 譜面ヘッダー仕様に戻る](dos_header.html)
## makerView

### 使い方
```
|makerView=true|
```
### 説明
譜面別の制作者表示を設定画面・結果画面に表示するかどうかを設定できます。  
また有効化(true)することで、譜面別データ(LocalStorage)のハイスコアキー項目に制作者名を付加できるようになります。  

デフォルトは`false`(表示しない)です。

|値|既定|内容|
|----|----|----|
|false|*|譜面別の制作者表示はリザルトコピーのみ<br>LocalStorageのハイスコアキー項目：キー数＋譜面名|
|true||譜面別の制作者表示を設定・結果画面へ拡大する<br>LocalStorageのハイスコアキー項目：キー数＋譜面名＋制作者名|

### 関連項目
- [**difData**](dos-h0002-difData.html) (*, ★)  譜面情報 
- [difSelectorUse](dos-h0051-difSelectorUse.html)  譜面選択セレクターの利用有無
- [**tuning**](dos-h0017-tuning.html) (★)  製作者クレジット

### 更新履歴

|Version|変更内容|
|----|----|
|[v8.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v8.2.0)|初回実装|