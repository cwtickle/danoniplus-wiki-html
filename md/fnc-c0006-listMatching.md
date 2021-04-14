[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# listMatching
### 概要
  - 検索文字がリストの中の一部に合致（部分一致）するかどうかを  
英大文字・英小文字を区別せずにチェックする。
  - 検索文字の英字は小文字にして比較するため、検索リストの英字は小文字にする必要がある。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_str|string|*|対象文字|
|_list|array|*|検索リスト (英字は小文字にする必要あり)|
|prefix|string||前方一致条件 (前方一致時は ^)|
|suffix|string||後方一致条件 (後方一致時は $)|

### 返却値
- 合致した場合は`true`, いずれにも合致しない場合は`false`を返却（真偽値）。

### 使用例
```javascript
const str = `image.png`;
const list = [`.jpg`, `.png`, `.gif`];

if (listMatching(str, list, { suffix: `$` }){
  // 対象の拡張子に合致した場合の処理
}
```

### 関連項目
- [fuzzyListMatching](fnc-c0039-fuzzyListMatching.html)

### 更新履歴

|Version|変更内容|
|----|----|
|[v19.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.2.0)|・初回実装|