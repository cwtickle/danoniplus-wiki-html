[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# openLink
### 概要
- 引数で渡されたリンクを新しいタブで開く関数。  
ただし、リンクが無い場合は何もしない。
- リンクかどうかは`http://`もしくは`https://`開始かどうかで簡易的に判断している。
- 別タブで開くとき、`target="_blank"`と`rel="noopener"`を自動で付加。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_url|string|*|URL情報|

### 返却値
- なし

### 使用例
```javascript
openLink(`https://gitter.im/danonicw/freeboard`);  // 指定したURLを新しいタブで開く
```
