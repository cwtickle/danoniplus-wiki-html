[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_wordObj

### 概要
- 歌詞表示データの現在の状態を管理するためのオブジェクト。   
歌詞データがあれば、このオブジェクトの情報が更新される。    
```javascript
const g_wordObj = {
	wordDir: 0,
	wordDat: ``,
	fadeInFlg0: false,
	fadeInFlg1: false,
	fadeOutFlg0: false,
	fadeOutFlg1: false
};
```

### 生成タイミング
- メイン画面開始時

### プロパティ
- wordDir (number) 歌詞表示の階層
- wordDat (string) 歌詞表示データ本体
- fadeInFlg*N* (boolean) フェードイン中フラグ (*N*は深度、偶数:上段、奇数:下段)
- fadeOutFlg*N* (boolean) フェードアウト中フラグ (*N*は深度、偶数:上段、奇数:下段)