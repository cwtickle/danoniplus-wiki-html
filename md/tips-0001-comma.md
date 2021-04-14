[← Tips Indexに戻る](tips-index.html)
# タイトルや歌詞表示に半角コンマ(,)を使う
半角コンマは区切り文字として使用しているため、  
通常はタイトルや歌詞表示に使うことができません。  
本tipsでは文字参照を使って半角コンマを表示する方法を説明します。

## 方法1
1. `,`の代わりに`*comma*`を使用します。

## 方法2
1. 譜面データを`&`区切りにしている場合は`|`区切りに修正します
2. HTMLに以下の記述を追加します
```
<input type="hidden" name="enableAmpersandSplit" id="enableAmpersandSplit" value="false">
```
3. 半角コンマを使いたい場所に`&comma;`を記述します

## CW Editionの特殊文字の取り扱い
- [譜面データにおける特殊文字の取り扱い](SpecialCharacters.html)をご覧ください。  
良く使用する特殊文字はカバーしています。

## その他の特殊文字（正式）
よく使いそうな特殊文字の書き方を以下の表に示します。  
これ以外の文字については[Character Entity Reference Chart](https://dev.w3.org/html5/html-author/charref)などをご覧ください。

| 文字 | 文字参照 |
----|----
| &amp; | `&amp;` |
| &vert; | `&vert;` |
| &lt; | `&lt;` |
| &gt; | `&gt;` |

## 動作確認バージョン
- 方法1: [v14.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v14.4.0)で追加
- 方法2: [v5.8.0](https://github.com/cwtickle/danoniplus/releases/tag/v5.8.0)で追加

## ページ作成者
- すずめ
- ティックル

## 更新履歴

|更新日|変更内容|
|----|----|
|2020/10/10|特殊文字のエスケープ実装に伴い、内容を追記|

## 関連項目
- [譜面の作成概要](HowtoMake.html)
- [歌詞表示 (word_data)](dos-e0003-wordData.html)
- [譜面データにおける特殊文字の取り扱い](SpecialCharacters.html)