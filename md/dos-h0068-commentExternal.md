[← 譜面ヘッダー仕様に戻る](dos_header.html)
## commentExternal

### 使い方
```
|commentExternal=true|
```
### 説明
[commentVal](dos-h0066-commentVal.html)をタイトル内ではなく、画面の外に表示するかを設定します。
画面外に表示する場合、以下いずれかをhtml内に記述する必要があります。
```html
<span id="commentArea"></span>
<div id="commentArea"></div>
<p id="commentArea"></p>
```

|値|既定|内容|
|----|----|----|
|false|*|作品コメント(commentVal)をタイトル画面内に配置する|
|true||作品コメント(commentVal)を画面外に表示する|

### 関連項目
- [commentVal](dos-h0066-commentVal.html)  コメント表示
- [commentAutoBr](dos-h0067-commentAutoBr.html)  コメント表示時に改行タグを自動挿入する設定

### 更新履歴

|Version|変更内容|
|----|----|
|[v15.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.0)|初回実装|