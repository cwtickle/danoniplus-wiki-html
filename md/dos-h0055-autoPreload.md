[← 譜面ヘッダー仕様に戻る](dos_header.html)
## autoPreload
### 使い方
```
|autoPreload=true|
```
### 説明
背景・マスクモーション※に bmp/gif/png/jpg の拡張子が含まれていれば、  
自動でその画像をプリロードするかどうかを設定します。  
有効にした場合、自動プリロード対象の画像は、[preloadImages](dos-h0021-preloadImages.html)への指定が不要です。

※ back/mask_data, back/masktitle_data, back/maskresult_data     

|値|既定|内容|
|----|----|----|
|false|*|画像をプリロードしない|
|true||画像をプリロードする|

### 関連項目
- [**preloadImages**](dos-h0021-preloadImages.html)  画像ファイルの事前読み込み設定
- [背景・マスクモーション (back_data, mask_data)](dos-e0004-animationData.html)  

### 更新履歴

|Version|変更内容|
|----|----|
|[v10.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v10.0.0)|初回実装|