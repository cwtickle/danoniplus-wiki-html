[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_detailObj

### 概要
- 譜面詳細データを管理するためのオブジェクト。   
譜面毎の矢印数、譜面密度、難易度レベルなどをタイトル画面前に取得し、格納する。    
```javascript
const g_detailObj = {
	arrowCnt: [],
	frzCnt: [],
	maxDensity: [],
	densityData: [],
	startFrame: [],
	playingFrame: [],
	playingFrameWithBlank: [],
	speedData: [],
	boostData: [],
	toolDif: [],
};
```

### 生成タイミング
- `storeBaseData ()`呼び出し時（譜面読込時）

### プロパティ
※設定されるプロパティはすべて譜面毎の配列になっています。
- arrowCnt
- frzCnt
- maxDensity
- densityData
- startFrame
- playingFrame
- playingFrameWithBlank
- speedData
- boostData
- toolDif