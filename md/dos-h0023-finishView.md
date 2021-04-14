[← 譜面ヘッダー仕様に戻る](dos_header.html)
## finishView

### 使い方
```
|finishView=none|
```
### 説明
フルコンボ演出の有無を設定します。  
"none"を指定することでフルコンボ演出を表示せず、通常のコンボ表示を行います。  
コンボ表示も消す場合は、danoni_custom.js等で設定してください。   


|値|既定|内容|
|----|----|----|
|(未指定)|*|フルコンボ演出あり|
|none||フルコンボ演出なし|

### 関連項目
- [**customjs**](dos-h0019-customjs.html)  カスタムjsファイルの指定

### 更新履歴

|Version|変更内容|
|----|----|
|[v1.15.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.0)|初回実装|