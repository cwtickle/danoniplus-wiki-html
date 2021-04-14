[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# fuzzyListMatching
### 概要
  - 検索文字がリストの中の一部に合致（前方・後方一致）するかどうかを  
英大文字・英小文字を区別せずにチェックする。
  - 検索文字の英字は小文字にして比較するため、検索リストの英字は小文字にする必要がある。
  - listMatching関数との違いは、初めから前方・後方一致両方を指定できるところが異なります。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_str|string|*|対象文字|
|_headerList|array|*|前方一致検索リスト (英字は小文字にする必要あり)|
|_footerList|array|*|後方一致検索リスト (英字は小文字にする必要あり)|

### 返却値
- 合致した場合は`true`, いずれにも合致しない場合は`false`を返却（真偽値）。

### 使用例
```javascript
fuzzyListMatching(`gaugeNormal`, [`gauge`], [`_data`, `_change`]) // true(前方一致)
fuzzyListMatching(`speed_data`, [`gauge`], [`_data`, `_change`]) // true(後方一致)
fuzzyListMatching(`difData`, [`gauge`], [`_data`, `_change`]) // false
```

### 関連項目
- [listMatching](fnc-c0006-listMatching.html)

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.1.0)|・初回実装|