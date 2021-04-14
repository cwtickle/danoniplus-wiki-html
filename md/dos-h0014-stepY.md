[← 譜面ヘッダー仕様に戻る](dos_header.html)
## stepY

### 使い方
```
|stepY=100|
```
### 説明
ステップゾーンのY座標を指定します。単位はpx。デフォルトは70pxです。  
Reverseの場合は下からstepYを差し引いた位置に配置します。  

### 使用例
- stepYの値を変えると、ステップゾーンのY座標が上下それぞれ下記のように変わります。

![dos-h0014-01.png](./wiki/dos-h0014-01.png)

### 関連項目
- [stepYR](dos-h0049-stepYR.html)  ステップゾーン(下)のY座標現位置からの差分
- [arrowJdgY / frzJdgY](dos-h0058-jdgY.html)  判定キャラクタのY座標位置

### 更新履歴

|Version|変更内容|
|----|----|
|[v1.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|初回実装|