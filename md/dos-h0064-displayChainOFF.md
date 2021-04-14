[← 譜面ヘッダー仕様に戻る](dos_header.html)
## displayChainOFF<br>(stepZone, judgment, fastSlow, lifeGauge, score, musicInfo, filterLine, speed, color, lyrics, background, arrowEffect, special)

### 使い方
```
|stepZoneChainOFF=|
|judgmentChainOFF=|
|fastSlowChainOFF=|
|lifeGaugeChainOFF=|
|scoreChainOFF=|
|musicInfoChainOFF=|
|filterLineChainOFF=|
|speedChainOFF=|
|colorChainOFF=|
|lyricsChainOFF=|
|backgroundChainOFF=judgment,fastSlow|
|arrowEffectChainOFF=|
|specialChainOFF=judgment,fastSlow|
```

### 説明
Displayオプションの設定をONにしたときに、  
連動して設定をOFFにする他のDisplayオプションを指定します。  
上記の場合、「Background」をONにすると「Judgment」「FastSlow」がOFFになります。  
逆にOFFにした場合、上記の例では「Background」「Special」の両方がOFFになれば  
「Judgment」「FastSlow」がONになります。  

ボタンの無効化設定は行いません。  
また、下記のようにお互いを打ち消したり、同一のものを指定する設定は行えません。
```
|stepZoneChainOFF=judgment|
|judgmentChainOFF=stepZone| <- お互いを打ち消す設定は行えない
|fastSlowChainOFF=fastSlow| <- 同一値の指定もNG
```

### 関連項目
- [displayUse](dos-h0057-displayUse.html)  Display項目の利用有無, 初期値設定
   - stepZoneUse, judgmentUse, fastSlowUse, ... etc

### 更新履歴

|Version|変更内容|
|----|----|
|[v14.0.2](https://github.com/cwtickle/danoniplus/releases/tag/v14.0.2)|・初回実装|