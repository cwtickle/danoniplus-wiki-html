[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_hidSudObj

### 概要
- Appearanceフィルタに関する各種情報を管理するオブジェクト。   
 
```javascript
const g_hidSudObj = {
    filterPos: 10,
    pgDown: {},
    pgUp: {},
    std: {},
    filterPosDefault: {},
};
```

### 生成タイミング
- 初回起動時

### プロパティ
- filterPos (number) - Appearanceフィルタの適用割合
- pgDown (object) - Appearanceフィルタを下げる場合の対応キー
- pgUp (object) - Appearanceフィルタを上げる場合の対応キー
- std (object) - Appearanceフィルタのパーセント表示の表示箇所
- filterPosDefault (object) - Appearanceフィルタの初期位置 (Visible, Hidden, Sudden時)
- (Visible, Hidden, Hidden+, Sudden, Sudden+, Hid&Sud+) (number)