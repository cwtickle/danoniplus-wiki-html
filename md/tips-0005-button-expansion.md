[← Tips Indexに戻る](tips-index.html)
# ボタン処理の拡張・上書き
- v17.1.0より、既存ボタンを上塗りすることなく処理を足すことが可能になりました。  
既存ボタンに処理を足したり、上書きする場合の方法を記載します。

## 使い方
- customjs (danoni_custom.js) のボタンがある関数内に記述します。  
対応する画面とカスタム関数の対応表は次の通りです。  
※末尾に`2`がつく関数は2つ目のcustomjsを使用する場合の関数名です。

|画面|対応するカスタム関数|
|----|----|
|タイトル画面|customTitleInit<br>customTitleInit2|
|設定画面|customOptionInit<br>customOptionInit2|
|設定（ディスプレイ）画面|customSettingsDisplayInit<br>customSettingsDisplayInit2|
|キーコンフィグ画面|customKeyConfigInit<br>customKeyConfigInit2|
|メイン画面(初期)|customMainInit<br>customMainInit2|
|メイン画面(フレーム毎)|customMainEnterFrame<br>customMainEnterFrame2|
|結果画面|customResultInit<br>customResultInit2|

### 処理を足す
- `g_btnAddFunc.` の後に処理を追加するボタンのID名を指定します。  
下記の例では、「Click Here!!」のボタン (btnStart)に処理を追加しています。  
- ID名については [ID一覧](IdReferenceIndex.html)をご覧ください。
- 既存ボタンの処理がされた後に、追加処理を行います。
```javascript
    g_btnAddFunc.btnStart = _ => {
        commentInit(); // g_btnAddFunc.(ボタンID) に関数を定義することでその処理を後から挿入
    };
```

### 処理を上書きする
- 処理を上書きするには、`g_btnDeleteFlg.` の後に上書きしたいボタンのID名を指定し、`true`を指定します。
※本来そのボタンが担う処理は無くなりますのでご注意ください。
- 実際にはその後に、カスタムで処理させたい処理を「処理を足す」と同様に記述します。
```javascript
    g_btnDeleteFlg.btnStart = true;  // g_btnDeleteFlg.(ボタンID) = true でボタンIDが行っている処理をやめる
    g_btnAddFunc.btnStart = _ => {
        commentInit(); // g_btnAddFunc.(ボタンID) に関数を定義することでその処理を後から挿入
    };
```

## 動作確認バージョン
- [v17.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.1.0)以降で利用可能です。

## ページ作成者
- ティックル

## 関連項目
- [ID一覧](IdReferenceIndex.html)