[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_headerObj

### 概要
- 初期化時に作成されるオブジェクト。`headerConvert ()`関数にて作成される。  
譜面データのうち、譜面ヘッダーの情報を取り出して(厳密にはg_rootObjから)、必要な変換、補完処理を掛けて格納している。  
```javascript
g_headerObj.keyX = value;
```

### 生成タイミング
- タイトル画面呼び出し前 (`headerConvert ()`呼び出し時)

### 補足
- ほとんどの項目は譜面ヘッダー項目とリンクしている。  
- 基本的に１度定義されれば変わることはないが、一部例外がある。(下記に示す)

### プロパティ
(* :初期定義中に値が決まるプロパティ、@ :設定により置き換わる可能性のあるプロパティ)
- customFont (string) *
- musicTitles (array)
- musicTitlesForView (array)
- artistNames (array)
- musicNos (array)
- artistName (string)
- artistUrl (string)
- minSpeed (float)
- maxSpeed (float)
- keyRetry (number)
- keyRetryDef (number)
- keyTitleBack (number)
- keyTitleBackDef (number)
- frzAttempt (number)
- tuning (string) @
- creatorUrl (string)
- tuningInit (string)
- keyLabels (array)
- difLabels (array)
- initSpeeds (array)
- lifeBorders (array)
- lifeRecoverys (array)
- lifeDamages (array)
- lifeInits (array)
- creatorNames (array)
- keyLists (array)
- difSelectorUse (boolean)
- defaultColorgrd (array)
- colorCdPaddingUse (boolean)
- maxLifeVal (float)
- defaultFrzColorUse (boolean)
- setColorInit (array)
- setColor (array) @
- setColorType0 (array)
- setColorType1 (array)
- setColorType2 (array)
- setColorStr (array)
- setColorStrType0 (array)
- setColorOrg (array)
- setColorOrgType0 (array)
- setShadowColorInit (array)
- setShadowColor (array)
- setShadowColorStr (array)
- setShadowColorOrg (array)
- frzColorInit (array)
- frzColor (array2) @
- frzColorType0 (array2)
- frzColorType1 (array2)
- frzColorType2 (array2)
- frzColorStr (array2)
- frzColorStrType0 (array2)
- frzColorOrg (array2)
- frzColorOrgType0 (array2)
- frzColorDefault (array2)
- frzShadowColorInit (array)
- frzShadowColor (array2)
- setDummyColor (array)
- dummyScoreNos (array)
- blankFrame (number) @
- blankFrameDef (number)
- startFrame (array)
- fadeFrame (array2)
- endFrame (array)
- adjustment (array)
- playbackRate (float)
- skinType (string)
- skinType2 (string)
- skinRoot (string)
- skinRoot2 (string)
- customjs (string)
- customjs2 (string)
- customjsRoot (string)
- customjsRoot2 (string)
- bottomWordSetFlg (boolean)
- musicFolder (string)
- musicUrls (array)
- hashTag (string)
- autoPreload (boolean) *
- preloadImages (array)
- finishView (string)
- releaseDate (string)
- customTitleUse (boolean)
- customTitleArrowUse (boolean)
- customBackUse (boolean)
- customBackMainUse (boolean)
- customReadyUse (boolean)
- readyDelayFrame (number)
- titlesize (number)
- titlefont (string)
- titlegrds (array)
- titlearrowgrds (array)
- titlegrd (string)
- titlearrowgrd (string)
- titlepos (string)
- titlelineheight (number)
- frzStartjdgUse (boolean)
- makerView (boolean)
- motionUse (boolean)
- scrollUse (boolean)
- shuffleUse (boolean)
- autoPlayUse (boolean)
- gaugeUse (boolean)
- appearanceUse (boolean) 
- stepzoneUse (boolean)
- stepzoneSet (switch)
- stepzoneChainOFF (array)
- judgmentUse (boolean) 
- judgmentSet (switch) 
- judgmentChainOFF (array)
- fastSlowUse (boolean) 
- fastSlowSet (switch) 
- fastSlowChainOFF (array)
- lifegaugeUse (boolean) 
- lifegaugeSet (switch) 
- lifegaugeChainOFF (array)
- scoreUse (boolean) 
- scoreSet (switch) 
- scoreChainOFF (array)
- musicInfoUse (boolean) 
- musicInfoSet (switch) 
- musicInfoChainOFF (array)
- filterLineUse (boolean) 
- filterLineSet (switch) 
- filterLineChainOFF (array)
- speedUse (boolean) 
- speedSet (switch) 
- speedChainOFF (array)
- colorUse (boolean) 
- colorSet (switch) 
- colorChainOFF (array)
- lyricsUse (boolean) 
- lyricsSet (switch) 
- lyricsChainOFF (array)
- backgroundUse (boolean) 
- backgroundSet (switch) 
- backgroundChainOFF (array)
- arrowEffectUse (boolean) 
- arrowEffectSet (switch) 
- arrowEffectChainOFF (array)
- specialUse (boolean) 
- specialSet (switch) 
- specialChainOFF (array)
- transKeyUse (boolean) 
- backTitleData (array)
- backTitleMaxDepth (number)
- maskTitleData (array)
- maskTitleMaxDepth (number)
- maskTitleButton (boolean) 
- maskResultButton (boolean) 
- colorDataType (string)
- resultMotionSet (boolean)
- scoreDetailUse (boolean)
- jdgPosReset (boolean)
- commentVal (string)
- commentExternal (boolean)
- wordAutoReverse (string)
- playingWidth (number)
- playingX (number)
- justFrames (number)
- resultFormat (string)