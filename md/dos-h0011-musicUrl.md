[← 譜面ヘッダー仕様に戻る](dos_header.html)
## musicUrl (*)

### 使い方
```
|musicUrl=PetitMagie.mp3|
|musicUrl=PetitMagie.js|
|musicUrl=rainbow.mp3$rainbow2.js|
|musicUrl=(..)PetitMagie.mp3|  // 作品ページと同じフォルダを参照
```
### 説明
1. 楽曲ファイル本体(mp3/wav/ogg)を指定する場合
   - 楽曲ファイル名(mp3/wav/ogg)を入れます。実際のファイルは「music」フォルダ※に入れてください。  
   - またmp3/wav/oggファイルをアップロードする場合で、  
".htaccess" が使えるサーバであれば、下記を ".htaccess" ファイルとして保存して、  
「music」フォルダに入れてください。以下のように指定します。
<pre>
SetEnvIf Request_URI "\.(mp3|wav|ogg)$" deny_ref
SetEnvIf Referer <b>"cw7\.sakura\.ne\.jp"</b> !deny_ref
Order Allow,Deny
Allow from all
Deny from env=deny_ref
</pre>
太字のところはサーバによって読み替えてください。「\.」は「\\\.」で置き換えます。  

2. 楽曲データをbase64変換したデータを利用する場合
   - 最初に、mp3データをbase64エンコードしたデータを用意します。  
musicUrlの値は、「jsファイル」もしくは「txtファイル」として指定してください。  
この場合、以下の書式で保存したものを「music」フォルダ※に入れることになります。  

```javascript
function musicInit(){
  g_musicdata='base64エンコードされた音楽データ';
}
```
※フォルダの名前は後述の「musicFolder」変数にて変更が可能です。  

（補足）base64変換ができるサイト・ソフト  
- [ダンおに曲データjs化ツール](https://suzme.github.io/danoni-base64/)  ( [GitHub](https://github.com/suzme/danoni-base64) )  
  - 音楽データを上記の指定フォーマットに変換し、そのまま使うことができます。
- https://tool-taro.com/base64_encode_binary/  
- https://www.vector.co.jp/soft/win95/util/se128122.html  

### 補足
ver4.0.0以降、"$"区切りで複数曲指定できるようになりました。  
musicTitleの"$"区切り、musicNoの番号と連動します。

### 関連項目
- [**musicTitle**](dos-h0001-musicTitle.html) (*, ★)  楽曲／楽曲クレジット
- [**difData**](dos-h0002-difData.html) (*, ★)  譜面情報 
- [musicNo](dos-h0012-musicNo.html)  楽曲ファイルと譜面の対応付け
- [musicFolder](dos-h0013-musicFolder.html)  楽曲ファイルの格納先
- [**playbackRate**](dos-h0010-playbackRate.html)  楽曲再生速度（主にテストプレイ用）

### 更新履歴

|Version|変更内容|
|----|----|
|[v10.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v10.0.0)|`(..)`を先頭に指定することで作品ページと同じフォルダを参照するように変更|
|[v4.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v4.0.0)|"$"区切りで複数曲指定できるように変更|
|[v1.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.7.0)|base64変換したmp3データ(jsファイル)を指定できるように変更|
|[v1.0.0<br>(v0.40.0)](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|初回実装|