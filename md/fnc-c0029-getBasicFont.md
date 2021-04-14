[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# getBasicFont
### 概要
- フォントリストを取得する関数。
- デフォルトは`"Meiryo UI", sans-serif`と、譜面ヘッダー：customFontで指定されたフォントが取得される。
- 引数に追加できる優先フォントはリスト形式のため、Font-Familyで指定する方法と同様に指定が可能。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_priorityFont|string||優先フォントリスト|

### 返却値
- フォント名の優先順位リスト (Font-Familyの書式)

### 使用例
```javascript
console.log(getBasicFont(`"Century"`)); // "Century", "Meiryo UI", sans-serif
console.log(getBasicFont(`"メイリオ", "游ゴシック"`)); // "メイリオ", "游ゴシック", "Meiryo UI", sans-serif
```

### 更新履歴

|Version|変更内容|
|----|----|
|[v20.3.1](https://github.com/cwtickle/danoniplus/releases/tag/v20.3.1)|・引数`_priorityFont`を追加|