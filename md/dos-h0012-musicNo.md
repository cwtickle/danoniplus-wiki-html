[← 譜面ヘッダー仕様に戻る](dos_header.html)
## musicNo
[ver4.x以降]

### 使い方
```
|musicNo=0$0$1|
```
### 説明
譜面毎にどの曲を対象にするか指定します。"$"区切り。  
musicTitle, musicUrlと連動しており、1曲目＝0, 2曲目＝1, 3曲目＝2 のように指定します。

### 関連項目
- [**musicTitle**](dos-h0001-musicTitle.html) (*, ★)  楽曲／楽曲クレジット
- [**difData**](dos-h0002-difData.html) (*, ★)  譜面情報 
- [**musicUrl**](dos-h0011-musicUrl.html) (*)  楽曲ファイル名

### 更新履歴

|Version|変更内容|
|----|----|
|[v4.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v4.0.0)|初回実装|