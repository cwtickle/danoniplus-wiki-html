[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# transTimerToFrame
### 概要
- `分:秒.差分フレーム数`の書式をフレーム数に変換する関数。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_str|string||`分:秒.差分フレーム数`の書式|

### 返却値
- フレーム数

### 使用例
```javascript
console.log(transTimerToFrame(`2:01`)); // 7260
console.log(transTimerToFrame(`0:20.40`)); // 1240
```

### 関連項目
- [transFrameToTimer](fnc-c0030-transFrameToTimer.html)

### 更新履歴

|Version|変更内容|
|----|----|
|[v20.3.1](https://github.com/cwtickle/danoniplus/releases/tag/v20.3.1)|・const関数として再定義|
