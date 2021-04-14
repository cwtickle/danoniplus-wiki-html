[← 譜面ヘッダー仕様に戻る](dos_header.html)
## startFrame

### 使い方
```
|startFrame=0|
```
### 説明
開始時のフレーム数を指定します。通常公開する場合は「0」を指定。  
テストプレイ時に、途中から開始したい場合などに使用できます。  
単位はフレーム数なので、60秒なら 60秒×60fps＝3600フレームとなります。  

ver3.11.0以降は譜面ごとに設定することも可能で、その場合は"$"で区切って使います。  
(詳しくはfadeFrame, endFrameの項を参照）

ver13.6.0以降は疑似タイマー表記(`分:秒.差分フレーム数`)に対応しています。
```
|startFrame=0:15.20| <- 15秒+20フレームのタイミングで開始
```

### 関連項目
- [**difData**](dos-h0002-difData.html) (*, ★)  譜面情報 
- [blankFrame](dos-h0006-blankFrame.html)  曲開始までの空白フレーム数
- [**endFrame**](dos-h0007-endFrame.html)  プレイ終了フレーム数
- [**fadeFrame**](dos-h0008-fadeFrame.html)  フェードアウト開始フレーム数

### 更新履歴

|Version|変更内容|
|----|----|
|[v13.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v13.6.0)|疑似タイマー表記に対応|
|[v3.11.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.11.0)|"$"区切りで譜面毎にstartFrameを設定できるように変更|
|[v1.0.0<br>(v0.42.0)](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|初回実装|