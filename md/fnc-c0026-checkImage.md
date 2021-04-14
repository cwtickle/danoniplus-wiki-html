[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# checkImage
### 概要
- 引数として渡したファイル名が、画像かどうかを判断する関数。  
画像かどうかを判断するためのリストは `g_imgExtensions` (danoni_constants.js) にて別途定義している。  
- ファイル名末尾の拡張子にて、画像かどうかを確認している。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_str|string|*|ファイル名のパス|

### 返却値
- 画像と判断した場合は`true`、そうでない場合は`false`を返す。

### 使用例
```javascript
if (g_headerObj.autoPreload) {
	if (checkImage(tmpObj.path)) {
		preloadFile(`image`, tmpObj.path);
	}
}
```
