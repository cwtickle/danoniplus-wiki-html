[← 譜面ヘッダー仕様に戻る](dos_header.html)
## playbackRate
[ver2.x以降]

### 使い方
```
|playbackRate=0.5|
```
### 説明
この値を指定することで、楽曲の再生速度を変更できます。  
デフォルトは1 (1倍)。楽曲の再生速度に合わせ、譜面も自動的に修正されます。    
※danoni_custom.js等でタイミングを別途調整している場合、ずれることがあります。  

### 関連項目
- [**musicUrl**](dos-h0011-musicUrl.html) (*)  楽曲ファイル名
- [**adjustment**](dos-h0009-adjustment.html)  譜面位置の初期調整

### 更新履歴

|Version|変更内容|
|----|----|
|[v2.8.0](https://github.com/cwtickle/danoniplus/releases/tag/v2.8.0)|初回実装|