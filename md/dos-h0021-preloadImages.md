[← 譜面ヘッダー仕様に戻る](dos_header.html)
## preloadImages

### 使い方
```
|preloadImages=myimage.png,myImage2.png,../img/otherfile.jpg|
|preloadImages=file*.png@4|     // -> file1.png ~ file4.png
|preloadImages=file*.png@2-9|   // -> file2.png ~ file9.png
|preloadImages=file*.png@5-10|     // -> file05.png ~ file10.png
|preloadImages=file*.png@01-08|     // -> file01.png ~ file08.png
```
### 説明
- プリロードしたい画像をカンマ区切りで指定します。相対パスも可。  
- アスタリスク（＊）とアットマーク（@）の利用により、  
複数ファイルのまとめ指定が可能です。  
`ファイル名*.拡張子@[開始番号-]終了番号`の形で指定すると、  
アスタリスク（＊）の部分が範囲指定した数字に置き換えられます。

### 関連項目
- [**autoPreload**](dos-h0055-autoPreload.html)  画像ファイルの自動読み込み設定

### 更新履歴

|Version|変更内容|
|----|----|
|[v7.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v7.5.0)|連番指定により、複数ファイルのまとめ記述に対応|
|[v1.0.0<br>(v0.67.1)](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|初回実装|