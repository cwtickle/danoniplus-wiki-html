[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# createScTextCommon
### 概要
- ショートカットキーの画面表示を画面別に一括で行う関数。
- 引数に合致した[g_btnPatterns](obj-v0021-g_btnPatterns.html)のプロパティ内にある項目すべてに対して  
[createScText](fnc-c0008-createScText.html)を呼び出し、ショートカットキーの画面表示を行う。
- [g_btnPatterns](obj-v0021-g_btnPatterns.html)の制約上、ボタンのid名が`btn`から始まる必要がある。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_displayName|string|*|画面名|

### 返却値
- なし

### 関数の依存関係
- **createScTextCommon**
  - [createScText](fnc-c0008-createScText.html)
  - [g_btnPatterns](obj-v0021-g_btnPatterns.html)

### 使用例
```javascript
g_btnPatterns.title = { Start: 0, Comment: -10 };
createScTextCommon(`title`);
```
これは下記と同義である。
```javascript
createScText(btnStart, `Start`, { displayName: `title`, targetLabel: `btnStart`, x: 0 });
createScText(btnComment, `Comment`, { displayName: `title`, targetLabel: `btnComment`, x: -10 });
```

### 関連項目
- [**g_shortcutObj**](obj-v0017-g_shortcutObj.html)
- [createScText](fnc-c0008-createScText.html)
- [g_btnPatterns](obj-v0021-g_btnPatterns.html)

### 更新履歴

|Version|変更内容|
|----|----|
|[v19.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.5.0)|・初回実装|