[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# drawDefaultBackImage
### 概要
- 画面の背景部分を再描画する関数。通常、[clearWindow](fnc-c0021-clearWindow.html) 関数とセットで使用する。  
※ver20.4.0以降、clearWindow関数に内包。
- メイン画面と使い分けがあるが、これは背景をカスタムする関数がメイン画面とそれ以外で異なるため。  
（それぞれ、customBackMainUse, customBackUse）

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_key|string|*|画面名。メイン画面との使い分けで使用。<br>`Main`: メイン画面、`(空)`: それ以外|

### 返却値
- なし

### 使用例
```javascript
function optionInit() {
    clearWindow();
    drawDefaultBackImage(``);
    // 省略
}
```
