[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_rankObj

### 概要
- 結果画面で表示するランク情報を管理するためのオブジェクト。   
`rankMarkXX`がランク名、`rankColorXX`がランクに対応するカラーコード、  
`rankRate`がランクごとの必要達成率を表す。
 
```javascript
const g_rankObj = {
    rankMarks: [`SS`, `S`, `SA`, `AAA`, `AA`, `A`, `B`, `C`],
    rankRate: [97, 90, 85, 80, 75, 70, 50, 0],
    rankColor: [`#00ccff`, `#6600ff`, `#ff9900`, `#ff0000`, `#00ff00`, `#ff00ff`, `#cc00ff`, `#cc9933`],

    rankMarkPF: `PF`,
    rankColorPF: `#cccc00`,
    rankMarkF: `F`,
    rankColorF: `#999999`,
    rankMarkX: `X`,
    rankColorX: `#996600`
};
```

### 生成タイミング
- 初回起動時

### プロパティ
- rankMarks (array)
- rankRate (array)
- rankColor (array)
- rankMarkPF (string)
- rankColorPF (string)
- rankMarkF (string)
- rankColorF (string)
- rankMarkX (string)
- rankColorX (string)
