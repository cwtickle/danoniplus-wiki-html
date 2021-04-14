[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_scoreObj

### 概要
- 譜面に関連するオブジェクト。  
初期化時は作成されず、譜面データに依存するプロパティが格納される。  
```javascript
g_scoreObj.arrowData = [];
g_scoreObj.frzData = []
```

### 生成タイミング
- タイトル画面開始時、ロード画面時の一時変数、プレイ開始前、結果画面表示時。

### プロパティ
※主に使用する画面として記載していますが、他の画面でも参照している場合があります。

#### タイトル画面
- titleFrameNum (number)
- backTitleFrameNum (number)
- maskTitleFrameNum (number)
- backTitleLoopCount (number)
- maskTitleLoopCount (number)

#### ロード画面
- arrowData (array2)
- frzData (array2)
- dummyArrowData (array2)
- dummyFrzData (array2)
- speedData (array)
- boostData (array)
- colorData (array)
- acolorData (array)
- shadowColorData (array)
- ashadowColorData (array)
- arrowCssMotionData (array)
- frzCssMotionData (array)
- dummyArrowCssMotion (array)
- dummyFrzCssMotion (array)
- wordData (array)
- wordMaxDepth (number)
- maskData (array)
- maskMaxDepth (number)
- backData (array)
- backMaxDepth (number)

#### メイン画面
- **frameNum** (number)
- **baseFrame** (number)
- fadeOutFrame (number)
- fadeOutTerm (number)
- fullFrame (number)
- nominalFrameNum (number)

#### 結果画面
- resultFrameNum (number)
- backResultFrameNum (number)
- maskResultFrameNum (number)
- backResultLoopCount (number)
- maskResultLoopCount (number)
