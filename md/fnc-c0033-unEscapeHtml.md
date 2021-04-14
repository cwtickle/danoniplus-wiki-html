[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# unEscapeHtml

### 概要
- エスケープされた文字を検知して、元の文字列に変換する関数。  
`escapeHtml`関数の逆。`g_escapeStr.unEscapeTag`で定義された二次元配列を使って変換する。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_str|string|*|エスケープされた文字列|

### 返却値
- 元の文字列（エスケープを含まない文字列）

### 使用例
```javascript
console.log(unEscapeHtml(`&lt;tag&gt;`)); // <tag>
console.log(unEscapeHtml(`T&amp;J`)); // T&J
```

### 関連項目
- [g_escapeStr](obj-v0023-g_escapeStr.html)
- [escapeHtml / escapeHtmlForEnabledTag](fnc-c0032-escapeHtml.html)
