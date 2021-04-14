[← 譜面ヘッダー仕様に戻る](dos_header.html)
## difData (*)

### 使い方
```
|difData=11W,Normal,3.5,x,10,5$11W,Hard::tickle,3.5,70,2,7$11W,Extra::ティックル,3.5,70,2,7|
```
### 説明
譜面情報を記述します。まず、"$"区切りで譜面ごとの設定です。  
さらにカンマ区切りでキー数、譜面名などを指定します。  
カンマ区切りの内容は次の通りです。  
（指定なしでも問題はありませんが、最低限キー数項目は指定した方が無難です。）  

|番号|設定例|内容|既定値|
|----|----|----|----|
|1|11W|対象譜面のキー数を指定します。|7|
|2|Normal|対象譜面の名前を指定します。<br>また、コロンを2つ繋いでその後に制作者名を入れると、<br>リザルトコピー他でその制作者名が表示されるようになります（制作者名の指定は任意）。|Normal|
|3|3.5|対象譜面の初期速度を指定します。|3.5|
|4|70|対象譜面が達成すべきノルマ率を0～100で指定します。<br>0を指定した場合、ライフが0になるとゲームオーバーです。<br>また、"x"を指定するとライフ制となり、<br>ライフの増減量が矢印数に関係なく同じとなります。|x|
|5|2|対象譜面のライフ増加割合を0～100で指定します。|6|
|6|7|対象譜面のライフ減少割合を0～100で指定します。|40|
|7|40|対象譜面の初期ライフ割合を0～100で指定します。|25|

### 使用例
```
|difData=11,Moving::izkdic＆ティックル,2.5,70,1,5|
```
![dos-h0002-01.png](./wiki/dos-h0002-01.png)

### 関連項目
- [**musicTitle**](dos-h0001-musicTitle.html) (*, ★)  楽曲／楽曲クレジット
- [**musicUrl**](dos-h0011-musicUrl.html) (*)  楽曲ファイル名
- [musicNo](dos-h0012-musicNo.html)  楽曲ファイルと譜面の対応付け
- [dummyId](dos-h0042-dummyId.html)  ダミー譜面の指定
- [startFrame](dos-h0005-startFrame.html) (★)  プレイ開始フレーム数
- [**endFrame**](dos-h0007-endFrame.html)  プレイ終了フレーム数
- [**fadeFrame**](dos-h0008-fadeFrame.html)  フェードアウト開始フレーム数
- [**adjustment**](dos-h0009-adjustment.html)  譜面位置の初期調整
- [customGauge](dos-h0053-customGauge.html)  カスタムゲージ設定
- [**gaugeX**](dos-h0022-gaugeX.html)  ゲージ設定の詳細
- [**makerView**](dos-h0050-makerView.html)  譜面別の制作者名表示設定


### 更新履歴

|Version|変更内容|
|----|----|
|[v8.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v8.2.0)|譜面別の制作者表示に対応|
|[v1.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|初回実装|