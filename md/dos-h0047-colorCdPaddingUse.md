[← 譜面ヘッダー仕様に戻る](dos_header.html)
## colorCdPaddingUse

### 使い方
```
|colorCdPaddingUse=true|
```
### 説明
初期矢印色・初期フリーズアロー色のカラーコードについて、  
ゼロパディングするかどうかの設定を行います。  
例えば、`0xff`を`#0000ff`、`0xffff`を`#00ffff`のように補完します。  

デフォルトは`false`(ゼロパディングしない)です。

|値|既定|内容|
|----|----|----|
|false|*|ゼロパディングしない|
|true||ゼロパディングする|

### 関連項目
- [**setColor**](dos-h0003-setColor.html) (*, ★)  矢印色
- [**frzColor**](dos-h0004-frzColor.html) (*, ★)  フリーズアロー色

### 更新履歴

|Version|変更内容|
|----|----|
|[v7.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v7.4.0)|初回実装|