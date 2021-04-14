[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# escapeHtml / escapeHtmlForEnabledTag

### 概要
- 特殊文字を含む文字を検知して、エスケープ文字を含む文字列に変換する関数。
- この2関数はどちらもエスケープする関数であることは同じだが、対象範囲が異なる。

|関数|対象範囲|
|----|----|
|escapeHtmlForEnabledTag|`g_escapeStr.escapeTag`で定義された特殊文字<br>([譜面データにおける特殊文字の取り扱い](SpecialCharacters.html)に掲載)が対象。|
|escapeHtml|`g_escapeStr.escapeTag`で定義された特殊文字に加えて、<br>他のエスケープリストを利用できる。<br>デフォルトは`g_escapeStr.escape`を追加で利用。|

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_str|string|*|元の文字列|
|_escapeList|array||[変換元,変換先]をペアとした二次元配列<br>※escapeHtmlのみ指定可能|

### 返却値
- エスケープ文字を含む文字列

### 使用例
```javascript
console.log(escapeHtml(`<tag>`)); // &lt;tag&gt;
console.log(escapeHtmlForEnabledTag(`T*amp*J`)); // T&amp;J
```

### 関連項目
- [g_escapeStr](obj-v0023-g_escapeStr.html)
- [unEscapeHtml](fnc-c0033-unEscapeHtml.html)
