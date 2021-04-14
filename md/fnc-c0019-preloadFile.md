[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# preloadFile
### 概要
- 画像等のpreloadを行う関数。`<link rel=preload>`の機能を使用している。
- Firefox 84以前では`<link rel=preload>`が使用できないため、  
画像については画像読込を先に行うことでその代替としている。
- 同じファイルが二重に指定された場合、先に指定されたもののみpreload指定される。  
`g_preloadFiles`でpreload対象を管理しており、リストに無いものをpreloadする仕組みになっている。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_as|string|*|preload対象。画像は`image`, フォントは`font`が入る。|
|_href|string|*|preload対象のアドレス、もしくはsvgパス。|
|_type|string||MIME タイプ|
|_crossOrigin|string||オリジン指定。既定は`crossOrigin="anonymous"`が指定される。|

### 返却値
- なし

### 使用例
```javascript
preloadFile(`image`, `giko.svg`);
preloadFile(`image`, `iyo.svg`);
```
