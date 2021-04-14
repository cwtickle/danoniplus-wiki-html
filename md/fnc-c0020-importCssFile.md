[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# importCssFile
### 概要
- 外部CSSファイルを読み込む関数。
- これを使うと、htmlファイル内に読み込む外部CSSファイルが指定されていなくても  
引数に渡した外部CSSファイルが読み込まれるようになる。
- ただし、この関数を指定した以後で読込を開始するため、基本的に遅延読み込みになる。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_href|string|*|外部CSSファイルのURL|
|_func|function||読込完了後に実行する処理|

### 返却値
- なし

### 使用例
```javascript
const randTime = new Date().getTime();
importCssFile(`${g_headerObj.skinRoot}danoni_skin_${g_headerObj.skinType}.css?${randTime}`, _ => {
	if (g_headerObj.skinType2 !== ``) {
		importCssFile(`${g_headerObj.skinRoot2}danoni_skin_${g_headerObj.skinType2}.css?${randTime}`, _ => initAfterCssLoaded());
	} else {
		initAfterCssLoaded();
	}
});
```

### 関連項目
- [loadScript](fnc-c0010-loadScript.html)

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.2.0)|・読込完了を待つように変更、引数`_func`を追加|
|[v10.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v10.0.0)|・初回実装|