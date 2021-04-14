[← 譜面ヘッダー仕様に戻る](dos_header.html)
## fadeFrame

### 使い方
```
|fadeFrame=3600,600$7200|
|fadeFrame=2:30| <- 疑似タイマー表記 (ver13.6.0以降対応)
```
### 説明
フェードアウトを開始するタイミングのフレーム数です。  
譜面ごとに設定が可能で、"$"で区切って使います。  
「endFrame」との併用が可能で、  
フェードアウトに合わせて結果画面に移行させることもできます。  

ver13.6.0以降は疑似タイマー表記(`分:秒.差分フレーム数`)に対応しています。

|番号|設定例|内容|
|----|----|----|
|1|3600|フェードアウト開始フレーム|
|2|1000|フェードアウト長(フレーム)。省略した場合は420フレーム(7秒)。|

### fadeFrameとendFrame、リザルト画面突入時間の関係
![dos-h0008-01.png](./wiki/dos-h0008-01.png)

### 関連項目
- [**difData**](dos-h0002-difData.html) (*, ★)  譜面情報 
- [**endFrame**](dos-h0007-endFrame.html)  プレイ終了フレーム数

### 更新履歴

|Version|変更内容|
|----|----|
|[v13.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v13.6.0)|・フェードアウト開始フレームの疑似タイマー表記に対応|
|[v8.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.0)|・楽曲のフェードアウト長を指定できるように変更|
|[v1.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|・初回実装|
