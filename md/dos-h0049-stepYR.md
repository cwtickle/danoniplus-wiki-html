[← 譜面ヘッダー仕様に戻る](dos_header.html)
## stepYR

### 使い方
```
|stepYR=-100|
```
### 説明
ステップゾーン(下)のY座標の差分を指定します。単位はpx。デフォルトは0pxです。    

### 使用例
- stepYRの値を変えると、ステップゾーン(下)のY座標だけが変わります。  
ステップゾーン(上)は変化しません。
- Ready?位置、判定キャラクタ・コンボ位置も合わせて補正されます。

![dos-h0049-01.png](./wiki/dos-h0049-01.png)

### 関連項目
- [stepY](dos-h0014-stepY.html)  ステップゾーンのY座標位置
- [arrowJdgY / frzJdgY](dos-h0058-jdgY.html)  判定キャラクタのY座標位置
- [bottomWordSet](dos-h0059-bottomWordSet.html)  下側の歌詞表示位置をステップゾーン位置に連動させる設定

### 更新履歴

|Version|変更内容|
|----|----|
|[v8.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.0)|初回実装|