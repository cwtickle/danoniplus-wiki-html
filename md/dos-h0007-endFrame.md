[← 譜面ヘッダー仕様に戻る](dos_header.html)
## endFrame

### 使い方
```
|endFrame=6000$7800|
|endFrame=2:40$3:10.20| <- 疑似タイマー表記 (ver13.6.0以降対応)
```
### 説明
楽曲終了時のフレーム数です。  
通常は楽曲データから取得するため設定不要ですが、尺余りするときに使います。  
譜面ごとに設定が可能で、"$"で区切って使います。  
endFrameを使った場合、結果画面終了後も曲が尺余りしていると曲が流れ続けます。  

単一の値を指定した場合、全ての譜面に対してそのフレーム数で終了するようになります。 

ver13.6.0以降は疑似タイマー表記(`分:秒.差分フレーム数`)に対応しています。 

### fadeFrameとendFrame、リザルト画面突入時間の関係
![dos-h0008-01.png](./wiki/dos-h0008-01.png)

### 関連項目
- [**difData**](dos-h0002-difData.html) (*, ★)  譜面情報 
- [startFrame](dos-h0005-startFrame.html) (★)  プレイ開始フレーム数
- [**fadeFrame**](dos-h0008-fadeFrame.html)  フェードアウト開始フレーム数

### 更新履歴

|Version|変更内容|
|----|----|
|[v13.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v13.6.0)|疑似タイマー表記に対応|
|[v1.10.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.10.0)|"$"区切りで譜面別に指定できるように変更（従来の使い方も可能）|
|[v1.0.0<br>(v0.42.0)](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|初回実装|