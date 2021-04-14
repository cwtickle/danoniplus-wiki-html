[← 譜面ヘッダー仕様に戻る](dos_header.html)
## adjustment
[ver2.x以降]

### 使い方
```
|adjustment=3$0$0|
```
### 説明
この値を指定することで、譜面の流れるタイミングを指定フレーム数遅く(早く)設定できます。  
$区切りで譜面単位に設定でき、単一指定で全譜面に対して適用できます。  
デフォルトは0（タイミング調整なし）です。  

### 楽曲開始位置、blankFrame、adjustmentの関係
![dos-h0006-01.png](./wiki/dos-h0006-01.png)

### 関連項目
- [**difData**](dos-h0002-difData.html) (*, ★)  譜面情報 
- [startFrame](dos-h0005-startFrame.html) (★)  プレイ開始フレーム数
- [blankFrame](dos-h0006-blankFrame.html)  曲開始までの空白フレーム数
- [**playbackRate**](dos-h0010-playbackRate.html)  楽曲再生速度（主にテストプレイ用）

### 更新履歴

|Version|変更内容|
|----|----|
|[v2.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v2.2.0)|初回実装|