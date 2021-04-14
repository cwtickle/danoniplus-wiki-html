[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# keyIsDown
### 概要
- キーが押されているかをチェックする関数。  
引数には [KeyBoardEvent.code](https://developer.mozilla.org/ja/docs/Web/API/KeyboardEvent/code) に対応した名前を指定する必要がある。
- KeyBoardEvent.keyCode との互換を保つため、Alt, Ctrl, Shiftキーのみ  
それぞれ「AltLeft」「ControlLeft」「ShiftLeft」と指定する必要がある。

### 仕様補足
- document.keyDown にてキーが押された状態を検知すると `g_inputKeyBuffer[コード] = true;`に変わる。  
（逆に、document.keyUpでは`g_inputKeyBuffer[コード] = false;`になる）
- keyIsDown関数では、この`g_inputKeyBuffer[コード]`の値を判断して押した状態かどうかを判断している。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_code|string|*|`KeyBoardEvent.code`に対応したコード|

### 返却値
- キーを押した状態である場合は`true`, そうではない場合は`false`を返す。

### 使用例
```javascript
if (keyIsDown(`ShiftLeft`)) {
    // Shiftキーを押したときの動作
}

if (keyIsDown(`ShiftLeft`) && keyIsDown(`KeyS`)) {
    // Shiftキーと Sキーを同時に押したときの動作
}
```
