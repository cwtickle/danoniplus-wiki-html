[← 譜面ヘッダー仕様に戻る](dos_header.html)
## commentAutoBr

### 使い方
```
|commentAutoBr=false|
|commentVal=
<p>
ページ整形の関係で、改行タグを個別にしたい場合は<br>
commentAutoBrをfalseに設定してください。<br>
</p>
|
```
### 説明
[commentVal](dos-h0066-commentVal.html)ではデフォルトで自動で改行タグを挿入しますが、  
諸事情で挿入したくない場合に、制御するための項目です。

|値|既定|内容|
|----|----|----|
|false||commentValで改行しても改行タグを挿入しない|
|true|*|commentValで改行した場合、自動で改行タグを挿入する|


### 関連項目
- [commentVal](dos-h0066-commentVal.html)  コメント表示
- [commentExternal](dos-h0068-commentExternal.html)  コメントを本体の外部に置く設定

### 更新履歴

|Version|変更内容|
|----|----|
|[v15.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.0)|初回実装|