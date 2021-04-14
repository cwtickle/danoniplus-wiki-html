[← 譜面ヘッダー仕様に戻る](dos_header.html)
## skinType
### 使い方
```
|skinType=skyblue|
|skinType=skyblue,background|
|skinType=skyblue,(..)background|
|skinType=(..)skin/|
```
### 説明
適用するスキン名を指定します。カンマ区切りで、最大2つまで指定が可能です。  
未指定の場合、`default`スキンが適用されます。  
1つ目は共通スキン、2つ目は作品個別スキンのような使い方が可能です。

### 補足  
両方で同じスタイルが指定された場合は、以下の優先度で適用されます。  
なお、`!important`指定した場合はこの限りではありません。

2つ目のスキン ＞ 1つ目のスキン ＞ ページ直指定 ＞ danoni_main.css

### 関連項目
- [**setColor**](dos-h0003-setColor.html) (*, ★)  矢印色
- [**frzColor**](dos-h0004-frzColor.html) (*, ★)  フリーズアロー色
- [setShadowColor](dos-h0041-setShadowColor.html)  矢印の内側を塗りつぶす設定および色の設定
- [**customjs**](dos-h0019-customjs.html)  カスタムjsファイルの指定
- [settingType](dos-h0056-settingType.html)  共通設定名

### 更新履歴

|Version|変更内容|
|----|----|
|[v19.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.3.0)|・カレント＋サブディレクトリ指定に対応|
|[v10.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v10.0.0)|・初回実装|