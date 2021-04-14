[← 譜面ヘッダー仕様に戻る](dos_header.html)
## blankFrame

### 使い方
```
|blankFrame=200|
```
### 説明
曲が始まるまでのフレーム数を指定します。デフォルトは「200」。  
曲開始までが長い場合、この値を小さくすることで少しだけ調整が可能です。  

### 楽曲開始位置、blankFrame、adjustmentの関係
![dos-h0006-01.png](./wiki/dos-h0006-01.png)

### 関連項目
- [startFrame](dos-h0005-startFrame.html) (★)  プレイ開始フレーム数
- [**adjustment**](dos-h0009-adjustment.html)  譜面位置の初期調整

### 更新履歴

|Version|変更内容|
|----|----|
|[v1.0.0<br>(v0.42.0)](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|初回実装|
