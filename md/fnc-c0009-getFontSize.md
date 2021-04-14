[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# getFontSize
### 概要
- 最大フォントサイズ(`_maxFontsize`)からだんだん小さくしていき、  
指定した横幅(`_maxWidth`)に合ったフォントサイズを取得する関数。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_str|string|*|対象の文字列|
|_maxWidth|number|*|横幅|
|_font|string||フォントリスト。デフォルトは`getBasicFont()`|
|_maxFontsize|number||最大フォントサイズ。デフォルトは64px。|


### 返却値
- フォントサイズ

### 使用例
```javascript
const name = `green symphony -short ver-`;
const width = 600;
const maxFontsize = 60;
const siz = getFontSize(name, width, `'メイリオ', 'Verdana'`, maxFontsize);
```

### 更新履歴

|Version|変更内容|
|----|----|
|[v20.1.2](https://github.com/cwtickle/danoniplus/releases/tag/v20.1.2)|・初回実装|