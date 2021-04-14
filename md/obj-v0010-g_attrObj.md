[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_attrObj

### 概要
- 矢印・フリーズアロー個別の属性を管理するためのオブジェクト。   
v17まではオブジェクトの`setAttribute`により管理していたが、  
v18以降は`g_attrObj`で管理している。  
```javascript
const g_attrObj = {};
const arrowName = `arrow0_20`; // 0番目のレーンの20番目に出現させる矢印

g_attrObj[arrowName] = {
	cnt: g_workObj.arrivalFrame[g_scoreObj.frameNum] + 1,
	boostCnt: g_workObj.motionFrame[g_scoreObj.frameNum],
	boostSpd: boostSpdDir, 
	dividePos: dividePos,
	prevY: firstPosY,
 	y: firstPosY,
};
```

### 生成タイミング
- 矢印・フリーズアロー出現時  
※オブジェクト自体は画面起動時から利用可能

### プロパティ
#### 矢印／フリーズアロー共通
- cnt (number) - ステップゾーンまでの残フレーム数
- boostCnt (number) - ステップゾーンまでの残フレーム数 (Motion用)
- boostSpd (number) - スクロール方向付き移動倍率 (boost_dataにより変化)
- dividePos (number) - スクロール方向 (通常:0, リバース:1)
- y (number) - オブジェクトのY座標

#### 矢印固有
- prevY (number) - 一つ前の矢印のY座標

#### フリーズアロー固有
- judgEndFlg (boolean) - 判定終了フラグ (初期値: `false`)
- isMoving (boolean) - 移動中フラグ (初期値: `true`)
- frzBarLength (number) - フリーズアローバーの長さ
- keyUpFrame (number) - キーを離したフレーム数
- dir (number) - スクロール方向 (通常:1, リバース:-1)
- barY (number) - フリーズアローバーの相対Y座標
- btmY (number) - フリーズアロー(後方矢印)の相対Y座標