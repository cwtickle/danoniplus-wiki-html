[← 譜面ヘッダー仕様に戻る](dos_header.html)
## musicTitle (*)

### 使い方
```
|musicTitle=プチ・マギエ,Napi,http://mart.kitunebi.com/|
|musicTitle=にじいろクレヨン,四葉かげろう,http://www.kagerow.net/$にじいろクレヨン -DR style mix-,AOiRO_Manbow,http://manbow.org/|
|musicTitle=曲名がとても長い曲<br>テストテストテスト,アーティスト名,http://...|
```
### 説明
楽曲情報を記述します。  
カンマ区切りで、「曲名」「アーティスト名」「アーティストのサイトURL」を指定します。  
また、ver4.0.0以降は"$"区切りで2曲目以降を指定できます。

|番号|設定例|内容|既定値|
|----|----|----|----|
|1|にじいろクレヨン|曲名を指定。タイトルの曲名もここで指定します。<br>※ver3.5.0以降、途中に&lt;br&gt;などをつけることで2行に分けることができます。|MusicName|
|2|四葉かげろう|アーティスト名|ArtistName|
|3|http://www.kagerow.net/|アーティストのサイトURL||
|4||曲名を指定します。<br>[musicNo](dos-h0012-musicNo.html)に`0`(1曲目)が指定されたときのみ使用可能な項目です。<br>タイトル表示で表示する曲名と1曲目の曲名の表示を分けたい場合に指定します。<br>ここで指定した曲名は、タイトル画面の表示以外で優先的に使用します。||

項目1, 4の曲名の改行タグについては、1行で表示した場合によってタグが異なります。

#### 半角スペースで置換するケース（従来の方法。&lt;br&gt;で折り返す）
```
|musicTitle=曲名が長い曲<br>半角スペース入り,アーティスト,http://|
```
- 1行にすると「曲名が長い曲_半角スペース入り」("_" は半角スペース)と表記。

#### 半角スペースで置換しないケース（&lt;nbr&gt;で折り返す）
```
|musicTitle=曲名が長い曲<nbr>半角スペース抜き,アーティスト,http://|
```
- 1行にすると「曲名が長い曲半角スペース抜き」と表記。

#### 全角スペースで置換するケース (&lt;dbr&gt;で折り返す)
```
|musicTitle=曲名が長い曲<dbr>全角スペース入り,アーティスト,http://|
```
- 1行にすると「曲名が長い曲＿全角スペース入り」("＿" は全角スペース)と表記。

### 使用例
```
|musicTitle=Careless Prince Came Back<br>from the Adventure - Web Style -,ASK,https://cw7.sakura.ne.jp/rdart/?artistId=20|
```
![dos-h0001-01.png](./wiki/dos-h0001-01.png)

### 関連項目
- [**difData**](dos-h0002-difData.html) (*, ★)  譜面情報 
- [**musicUrl**](dos-h0011-musicUrl.html) (*)  楽曲ファイル名
- [musicNo](dos-h0012-musicNo.html)  楽曲ファイルと譜面の対応付け
- [musicFolder](dos-h0013-musicFolder.html)  楽曲ファイルの格納先
- [**customTitleUse**](dos-h0025-customTitleUse.html)  タイトルの曲名文字
- [**titlesize**](dos-h0030-titlesize.html)  文字サイズ
- [**titlefont**](dos-h0031-titlefont.html)  フォント

### 更新履歴

|Version|変更内容|
|----|----|
|[v8.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v8.2.0)|・曲名（複数行）を1行で表示する場合に<br>　間を空白で埋めない（全角で埋める）設定を追加|
|[v4.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v4.0.0)|・"$"区切りで2曲目以降を指定できるように変更<br>・4番目の項目を追加|
|[v3.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.5.0)|・曲名指定部分に&lt;br&gt;を入れることで<br>　タイトル・結果画面の曲名表示を2行にできるように変更|
|[v1.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|初回実装|