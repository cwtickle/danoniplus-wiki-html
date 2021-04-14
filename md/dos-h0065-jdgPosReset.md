[← 譜面ヘッダー仕様に戻る](dos_header.html)
## jdgPosReset

### 使い方
```
|jdgPosReset=false|
```
### 説明
判定キャラクタ及びコンボ表示について、  
Backgroundの表示がOFFのときに[arrowJdgY / frzJdgY](dos-h0058-jdgY.html)を初期化するかどうかを設定します。 

|値|既定|内容|
|----|----|----|
|false||初期化しない (Backgroundの設定によらず判定位置を変えない)|
|true|*|初期化する (Background:OFF時、判定位置をデフォルトに戻す)|

### 関連項目
- [arrowJdgY / frzJdgY](dos-h0058-jdgY.html)  判定キャラクタのY座標位置

### 更新履歴

|Version|変更内容|
|----|----|
|[v15.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.0)|初回実装|