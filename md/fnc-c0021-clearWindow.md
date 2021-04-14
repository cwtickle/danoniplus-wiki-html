[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# clearWindow
### 概要
- 現在表示されている画面をクリアする関数。
- 厳密には、id:`divRoot`配下のオブジェクトを全て削除し、  
`document.onkeyup`, `document.onKeyDown`が指定されていた場合、初期化する。
- 基本、画面系の処理の先頭に記載しているため独自画面を生成するとき以外は個別に指定する必要はない。
- 背景を整備する`drawDefaultBackImage()`とセットで使うことが多いため、  
ver20.4.0以降は _redrawFlg を設定することでまとめて設定できるようになった。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_redrawFlg|boolean||背景を再描画を行うかどうかのフラグ (false:しない)|
|_customDisplayName|string||背景の再描画方法。drawDefaultBackImageで使用。<br>(デフォルト:`(空)`)|

### 返却値
- なし

### 関数の依存関係
- **clearWindow**
  - resetKeyControl
  - [drawDefaultBackImage](fnc-c0024-drawDefaultBackImage.html)

### 使用例
```javascript
function optionInit() {
    clearWindow(true);
    // 省略
}
```

### 更新履歴

|Version|変更内容|
|----|----|
|[v20.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v20.4.0)|・引数に`_redrawFlg`, `_customDisplayName`を追加|
|[v1.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|・初回実装|