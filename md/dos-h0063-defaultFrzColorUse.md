[← 譜面ヘッダー仕様に戻る](dos_header.html)
## defaultFrzColorUse

### 使い方
```
|defaultFrzColorUse=false|
```
### 説明
フリーズアロー色(frzColor)が指定されない場合、データ補完が行われます。  
その補完方法について、デフォルトのフリーズアロー色セットから取得するか、  
矢印色の設定(setColor)から取得するかを選択できるようにします。  
デフォルトは`true`です。

|値|既定|内容|
|----|----|----|
|false||矢印色の設定(setColor)から取得する|
|true|*|デフォルトのフリーズアロー色セットから取得する|

### 補足
この設定については、全体の設定として`danoni_setting.js`からも設定できます。  
どちらも設定があった場合は、譜面ヘッダーの値(defaultFrzColorUse)が優先されます。
```javascript
// フリーズアローのデフォルト色セットの利用有無 (true: 使用, false: 矢印色を優先してセット)
const g_presetFrzColors = true;
```

またv13.3.1以降は、`danoni_setting.js`で定義された`g_presetFrzColors`が`false`、  
もしくは譜面ヘッダー`|defaultFrzColorUse=false|`のとき、  
`frzColor`が1要素でも定義されていれば、その`frzColor`の値を使用します。

```
|setColor=a,b,c,d,e|
|frzColor=A,B,C,D|
-> |frzColor=A,B,C,D$A,B,C,D$A,B,C,D$A,B,C,D$A,B,C,D|

|setColor=a,b,c,d,e|
|frzColor=A,B|
-> |frzColor=A,B,A,B$A,B,A,B$A,B,A,B$A,B,A,B$A,B,A,B|

|setColor=a,b,c,d,e|
|frzColor=,,A,B|
-> |frzColor=a,a,A,B$b,b,A,B$c,c,A,B$d,d,A,B$e,e,A,B|

|setColor=a,b,c,d,e|
-> |frzColor=a,a,a,a$b,b,b,b$c,c,c,c$d,d,d,d$e,e,e,e|
```


### 関連項目
- [**frzColor**](dos-h0004-frzColor.html) (*, ★)  フリーズアロー色

### 更新履歴

|Version|変更内容|
|----|----|
|[v13.3.1](https://github.com/cwtickle/danoniplus/releases/tag/v13.3.1)|・フリーズアロー色(frzColor)の補完ルールを一部変更|
|[v13.1.1](https://github.com/cwtickle/danoniplus/releases/tag/v13.1.1)|・初回実装|