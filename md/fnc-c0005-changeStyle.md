[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# changeStyle
### 概要
- ラベル、ボタンに対して座標、サイズ、フォントなどを変更する。  
ただし、指定が無い項目は変更しない。

### 引数

|引数|型|必須|指定内容|
|----|----|----|----|
|_id|string|*|ボタンのID名|
|_obj|object||`x`:  X座標, `y`:  Y座標, `w`: 幅, `h`: 高さ,<br>`siz`: フォントサイズ, `align`: 文字位置, <br>`(属性名)`: (属性に対する設定)|

### 返却値
- なし

### 使用例
- btnSaveのidがついたボタンの座標位置、サイズを変更する例
```javascript
changeStyle(`btnSave`, {x: 20, y: 30, w:170, h:45, siz:14, align:C_ALIGN_RIGHT`});
```

### 更新履歴

|Version|変更内容|
|----|----|
|[v17.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.1.0)|・初回実装|