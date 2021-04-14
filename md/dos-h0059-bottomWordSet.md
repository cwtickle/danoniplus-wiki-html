[← 譜面ヘッダー仕様に戻る](dos_header.html)
## bottomWordSet

### 使い方
```
|bottomWordSet=true|
```
### 説明
下側の歌詞表示位置を、ステップゾーン位置に連動させるかを設定します。  
※ stepY, stepYR を変更した場合に有効です。  

デフォルトは`false`(連動しない)です。

|値|既定|内容|
|----|----|----|
|false|*|下側ステップゾーン位置と連動しない|
|true||下側ステップゾーン位置と連動する|

### 歌詞表示位置の違いについて
![dos-h0059-01.png](./wiki/dos-h0059-01.png)

### 関連項目
- [stepY](dos-h0014-stepY.html)  ステップゾーンのY座標位置
- [stepYR](dos-h0049-stepYR.html)  ステップゾーン(下)のY座標現位置からの差分

### 更新履歴

|Version|変更内容|
|----|----|
|[v11.1.1](https://github.com/cwtickle/danoniplus/releases/tag/v11.1.1)|初回実装|