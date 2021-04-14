[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_escapeStr
### 概要
- [譜面データにおける特殊文字の取り扱い](SpecialCharacters.html)で定義されている特殊文字を  
ブラウザで解釈できるエスケープ文字に変換したり、  
逆にエスケープ文字を元の文字に逆変換する二次元配列を管理するオブジェクト。

### 生成タイミング
- 初回起動時

### 補足
- escapeHtml, escapeHtmlForEnabledTag, unEscapeHtml関数で利用する。

### プロパティ
```javascript
const g_escapeStr = {
    escape: [[`&`, `&amp;`], [`<`, `&lt;`], [`>`, `&gt;`], [`"`, `&quot;`]],
    escapeTag: [
        [`*amp*`, `&amp;`], [`*pipe*`, `|`], [`*dollar*`, `$`], [`*rsquo*`, `&rsquo;`],
        [`*quot*`, `&quot;`], [`*comma*`, `&sbquo;`], [`*squo*`, `&#39;`], [`*bkquo*`, `&#96;`],
        [`*lt*`, `&lt;`], [`*gt*`, `&gt;`],
    ],
    unEscapeTag: [
        [`&amp;`, `&`], [`&rsquo;`, `’`], [`&quot;`, `"`], [`&sbquo;`, `,`],
        [`&lt;`, `<`], [`&gt;`, `>`], [`&#39;`, `'`], [`&#96;`, `\``],
    ],
    escapeCode: [
        [`<script>`, ``], [`</script>`, ``],
    ],
};
```

### 関連項目
- [escapeHtml / escapeHtmlForEnabledTag](fnc-c0032-escapeHtml.html)
- [unEscapeHtml](fnc-c0033-unEscapeHtml.html)
