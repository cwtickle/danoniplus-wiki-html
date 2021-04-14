[← 譜面ヘッダー仕様に戻る](dos_header.html)
## commentVal

### 使い方
```
|commentVal=
このような形で
コメントを入れます。
<img src="image.png" alt="画像タグや"><a href="index.html">リンクも可能です。</a>
|
```
### 説明
タイトル画面、もしくは本体外部にコメントを表示します。  
詳細の設定は関連譜面ヘッダーにて指定します。  
htmlタグも使えますが、シングルクォートなどの特殊文字は[譜面データ中の特殊文字の取り扱い](SpecialCharacters.html)に従って置き換えてください。  
なお、区切り文字の関係でダブルクォートは必須ではありません。

### 関連項目
- [commentAutoBr](dos-h0067-commentAutoBr.html)  コメント表示時に改行タグを自動挿入する設定
- [commentExternal](dos-h0068-commentExternal.html)  コメントを本体の外部に置く設定
- [譜面データ中の特殊文字の取り扱い](SpecialCharacters.html)

### 更新履歴

|Version|変更内容|
|----|----|
|[v15.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.0)|初回実装|