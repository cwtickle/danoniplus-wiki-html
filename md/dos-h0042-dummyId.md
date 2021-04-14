[← 譜面ヘッダー仕様に戻る](dos_header.html)
## dummyId

### 使い方
```
|dummyId=101$102|
```
### 説明
演出で使用する常時オートのダミー矢印が定義されている譜面番号を指定します。 
譜面ごとに設定が可能で、"$"で区切って使います。  

上記の場合、以下の譜面をダミー譜面として1譜面目と同時に流します。  
```
|left101_data=380,389|down101_data=360,389|
```

### 関連項目
- [**difData**](dos-h0002-difData.html) (*, ★)  譜面情報 

### 更新履歴

|Version|変更内容|
|----|----|
|[v6.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v6.0.0)|初回実装|