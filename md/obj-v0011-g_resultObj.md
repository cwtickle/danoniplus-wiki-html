[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_resultObj

### 概要
- プレイ中の判定数やスコアを管理するためのオブジェクト。   
 
```javascript
const g_resultObj = {
    ii: 0,
    shakin: 0,
    matari: 0,
    shobon: 0,
    uwan: 0,
    kita: 0,
    sfsf: 0,
    iknai: 0,
    combo: 0,
    maxCombo: 0,
    fCombo: 0,
    fmaxCombo: 0,
    score: 0,

    fast: 0,
    slow: 0,

    spState: ``,
};
```

### 生成タイミング
- メイン画面開始時

### プロパティ
#### 判定数情報
- ii
- shakin
- matari
- shobon
- uwan
- kita
- iknai

#### コンボ数、スコア、Fast/Slow情報
- combo
- maxCombo
- fCombo
- fmaxCombo
- score
- slow
- fast

#### パーフェクト、フルコンボ情報
- spState
