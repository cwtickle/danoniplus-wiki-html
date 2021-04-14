[← 譜面ヘッダー仕様に戻る](dos_header.html)
## customjs

### 使い方
```
|customjs=danoni_custom.js,danoni_custom-0190.js|
|customjs=danoni_custom.js,(..)special.js|  // 2つ目は作品ページと同じフォルダを参照
```
### 説明
作品別の割り込み処理が行えるcustomのjsファイルを指定します。  
デフォルトは「danoni_custom.js」を読み込みます。  
最大2ファイルをカンマ区切りで指定できます。  

### 関連項目
- [masktitleButton](dos-h0043-masktitleButton.html)  タイトル画面上のボタン群の有効/無効設定
- [maskresultButton](dos-h0044-maskresultButton.html)  リザルト画面上のボタン群の有効/無効設定
- [**skinType**](dos-h0054-skinType.html)  スキン設定
- [settingType](dos-h0056-settingType.html)  共通設定名

### 更新履歴

|Version|変更内容|
|----|----|
|[v19.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.3.0)|・カレント＋サブディレクトリ指定に対応|
|[v10.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v10.0.0)|・`(..)`を先頭に指定することで作品ページと同じフォルダを参照するように変更|
|[v1.0.0<br>(v0.40.0)](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|・初回実装|