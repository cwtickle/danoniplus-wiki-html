[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# transFrameToTimer
### 概要
- フレーム数を`分:秒`の形式に変換する関数。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_frame|number||フレーム数|

### 返却値
- `分:秒`の書式に変換した文字列

### 使用例
```javascript
console.log(transFrameToTimer(300)); // 0:05
console.log(transFrameToTimer(320)); // 0:05 ※端数切り捨て
console.log(transFrameToTimer(7260)); // 2:01
```

### 補足
- 端数フレーム数は切り捨てる。

### 関連項目
- [transTimerToFrame](fnc-c0031-transTimerToFrame.html)

### 更新履歴

|Version|変更内容|
|----|----|
|[v20.3.1](https://github.com/cwtickle/danoniplus/releases/tag/v20.3.1)|・初回実装|
