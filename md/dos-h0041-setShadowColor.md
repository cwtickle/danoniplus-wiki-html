[← 譜面ヘッダー仕様に戻る](dos_header.html)
## setShadowColor
### 使い方
```
|setShadowColor=#000000|
|setShadowColor=Default|
|setShadowColor=#ffcccc:#ffffff@radial-gradient,#ff9999:#ffff99@conic-gradient,#ffffff,#ffff99,#ff9966|
```
### 説明
矢印の内側を塗りつぶすかどうかを設定します。  
指定する場合はそのカラーコードを指定するか、`Default`を指定します。  
デフォルト（未指定）は矢印の内側を塗りつぶしません。

`Default`が指定された場合は、ベースの矢印色と同色にすることができます。  
(透明度は0.5で自動調整されます)

ver13より、setColorと同じようにグラデーション記述方式に対応しました。  
またver21より、setColorと同じように2譜面目以降の個別設定に対応しました。

### 関連項目
- [**setColor**](dos-h0003-setColor.html) (*, ★)  矢印色
- [**frzColor**](dos-h0004-frzColor.html) (*, ★)  フリーズアロー色
- [frzShadowColor](dos-h0062-frzShadowColor.html)  フリーズアローの矢印内側を塗りつぶす設定および色の設定
- [グラデーション仕様](dos-c0001-gradation.html) 

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.1.0)|・2譜面目以降の個別設定に対応（譜面分割＆譜面番号可変時）|
|[v21.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.0.0)|・2譜面目以降の個別設定に対応|
|[v13.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v13.0.0)|・グラデーション記述に対応|
|[v5.12.0](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.0)|・初回実装|