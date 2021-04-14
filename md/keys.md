# キー数仕様 / Keys' Specification
<img src="./wiki/keys1.png" width="400">

Dancing☆Onigiri (CW Edition)における各キーは、キーとパターンの組み合わせから成っています。  
以下であれば、11keyの1番目（0番目）のパターンであることを示します。
<pre>
pos<b>11</b>_<b>0</b>
</pre>

同じキーに属するパターンの設定は似ていますが、  
全く別のキーの扱いです。設定も個別に変更できます。  
配列の記載順は、必ず**左から右、上から下**になるよう記載が必要です。  

|要素|意味|詳細|
|----|----|----|
|charaX_Y|読込変数の接頭辞|left_data, down_dataなどの _dataより前の文字列を表す。|
|colorX_Y|矢印色の割り当て|譜面データ内「setColor」で記載のカラーコードを割り振る。<br>通常0～4が利用可能で、それぞれ「setColor」を配列にした場合の番号に対応した色が初期色として割り当てられる。|
|stepRtnX_Y|角度/AAの種類|左向き矢印を基準に、何度回転した矢印を配置するかを表す。<br>もしくは、対象のアスキーアート(AA)を指定する。<br>指定できるAAは、「onigiri」「giko」「iyo」「c」「morara」「monar」の6種類。|
|posX_Y|ステップゾーン位置|ステップゾーンを等間隔で置いた場合に、どこに置くかを示した数字。上記画像参照。<br>等間隔にしたくない場合は、上の例のように番号をスキップすることでステップゾーンを置かないことができる。|
|divX_Y|上段/下段折り返し位置|ステップゾーンの上段、下段を折り返す位置を指定する。<br>指定対象は、posX_Yの値を使用。初めて下段となる数字を指定する。<br>上段/下段の括りがない場合は、最後の数字+1を指定する。|
|blankX_Y|ステップゾーン間隔(X座標)|ステップゾーンの間隔を指定。指定がない場合は、通常55pxとなる。|
|scaleX_Y|矢印の描画エリアの拡大・縮小|矢印の描画エリアの拡大率を指定。指定がない場合は、1(1倍)となる。|
|keyCtrlX_Y|キーコンフィグ|各ステップに対応するキーコードを指定。多次元配列で表現する。同じステップに対して複数のキーを割り当てることも可能。|
|shuffleX_Y|シャッフルグループ|Mirror, Random, S-Random使用時、同じグループ同士で入れ替える。同じ数字が同じグループになる。|
|transKeyX_Y|別キーモードの設定|指定されたキーパターンが別キーのものである場合にそのキーの名前を指定。<u>同一キーの場合は指定しない。</u><br>指定した場合、結果画面にてここで指定したキーが補足情報として表示される。<br>また、別キーモードでプレイ中はハイスコアやキーコンフィグ等の保存対象外となる。|
|keyRetryX_Y|リトライキー|プレイ中ショートカットで、リトライが行えるキーのキーコードを指定。<br>デフォルトは8(BackSpace)。|
|keyTitleBackX_Y|タイトルバックキー|プレイ中ショートカットで、タイトルバックが行えるキーのキーコードを指定。<br>デフォルトは46(Delete)。|
|scrollNameX|スクロール拡張名|スクロール拡張で使用する名前。デフォルトは`---`。|
|scrollDirX_Y|スクロール拡張の方向設定|矢印毎の方向設定。「1」は下から上へ、「-1」は上から下へ流れる。|
|assistNameX|キーアシスト名|一部のキーのアシストで使用する名前。これにALL(全て)やOFFは含まれない。デフォルトはなし。|
|assistPosX_Y|アシストするキーの設定|矢印毎のアシスト設定。「1」はオートプレイ対象、「0」はオートプレイ対象外。|

## 少しだけ具体例 (11keyの場合)  

文字で書いてもピンと来ないかもしれないので、  
具体的に11keyのパターン0(1番目)の例を見ていきましょう。  
設定値はこんな感じになっています。並び順は左から右、上から下の順です。  
  
|要素|実際の値|
|----|----|
|chara11_0|["sleft", "sdown", "sup", "sright", "left", "leftdia", "down", "space", "up", "rightdia", "right"]|

この場合、下記のような譜面形式で読み込みができます。(数字は省略)  
<pre>
|sleft_data=...|sdown_data=...|...|right_data=...|
</pre>

|要素|実際の値|
|----|----|
|color11_0|[3, 3, 3, 3, 0, 1, 0, 2, 0, 1, 0]|
|setColor|0xcc99ff, 0xffccff, 0xffffff, 0xffff99, 0xff9966|

一番上の画像において、上段は3(=#ffff99, 黄色)、  
下段の奇数番目は0(=#cc99ff, 紫色)、偶数番目は1(=#ffccff, ピンク)、  
おにぎりは2(=#ffffff, 白色)となっています。  


|要素|実際の値|
|----|----|
|stepRtn11_0|[0, -90, 90, 180, 0, -45, -90, "onigiri", 90, 135, 180]|

一番上の画像において、左矢印を基準にすると  
-90°は下矢印、90°は上矢印、180°は右矢印となります。  
"onigiri"の箇所はおにぎりになっていますね。  

|要素|実際の値|
|----|----|
|pos11_0|[2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]|
|div11_0|6|

一番上の画像の黄色文字で数字を入れました。  
数字が6と書いてあるところから下段に折り返しています。  
0と1は指定が無いので、矢印が表示されていません。  

|要素|実際の値|
|----|----|
|keyCtrl11_0|[ [37], [40], [38, 0], [39], [83], [68], [70], [32], [74], [75], [76] ]|

キーコードが書かれています。  
これだけだとピンときませんが、3番目だけ要素が2つあるのが確認できると思います。  
この部分は代替キーがあることを表します。 
 
### 補足 (キーコンフィグ)
この画像の例では3番目だけ代替キーがありますが、  
現在のバージョンでは全てのキーに代替キーを最低１つ割り当てています。  
ここで指定する番号は [KeyboardEvent.keyCode](https://developer.mozilla.org/ja/docs/Web/API/KeyboardEvent/keycode) の値です。0は未割り当てを表します。  
なおKeyCodeは非推奨のため、内部的には [KeyboardEvent.code](https://developer.mozilla.org/ja/docs/Web/API/KeyboardEvent/code) に変換しています。
```javascript
keyCtrl11_0: [[37, 0], [40, 0], [38, 0], [39, 0], [83, 0], [68, 0], [70, 0], [32, 0], [74, 0], [75, 0], [76, 0]],
```

## カスタムキーの場合  

自分で作ったキーを公開する場合、譜面データに記述が必要です。  
基本的な考え方は上述と全く同じですが、記述方法が少し異なります。  

### keyExtraList
追加するキーのリストです。カンマ区切りでいくつでも追加できます。  
<pre>
|keyExtraList=6|
</pre>

### colorX, charaX, divX, stepRtnX, keyCtrlX, blankX, shuffleX
それぞれ、colorX_Y, charaX_Y, divX_Y, stepRtnX_Y, keyCtrlX_Y, blankX_Y, shuffleX_Yに相当します。複数指定の場合は"$"で区切ります。  
keyCtrlの場合、代替キー指定はスラッシュ(/)で区切ります。    

### scrollX, assistX
コロンを2つ繋げてコロンの前が名称、後が矢印ごとの設定になるよう記述します。 
設定を増やす場合はスラッシュ(/)で区切ります。  
キーパターンが複数ある場合は"$"で区切ります。 

これらのみ、通常キーの変数の定義方法とは異なります。 

|追加キーでの指定名|通常キーでの変数名|
|----|----|
|scrollX|scrollNameX<br>scrollDirX_Y|
|assistX|assistNameX<br>assistPosX_Y|

### 使用例

|要素|指定の仕方|
|----|----|
|colorX|color6=0,1,0,1,0,2$0,1,0,1,0,2|
|charaX|chara6=arrowA,arrowB,arrowC,arrowD,arrowE,arrowF$arrowA,arrowB,arrowC,arrowD,arrowE,arrowF|
|divX|div6=6$3|
|stepRtnX|stepRtn6=0,45,-90,135,180,onigiri$0,45,-90,135,180,onigiri|
|keyCtrlX|keyCtrl6=75,79,76,80,187,32/0$75,79,76,80,187,32/0|
|blankX|blank6=60$60|
|scaleX|scale6=1$0.8|
|shuffleX|shuffle6=0,0,0,0,0,1$0,0,0,0,0,1|
|transKeyX|transKey6=$6i|
|keyRetryX|keyRetry6=9|
|keyTitleBackX|keyTitleBack6=46|
|scrollX|scroll6=Cross::1,1,-1,-1,1,1/Split::1,1,1,-1,-1,-1/Alternate::1,-1,1,-1,1,-1$Cross::1,1,-1,-1,1,1/Split::1,1,1,-1,-1,-1/Alternate::1,-1,1,-1,1,-1|
|assistX|assist6=Onigiri::0,0,0,0,0,1/AA::0,0,0,1,1,1$...|

### 更新履歴

|Version|変更内容|
|----|----|
|[v15.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.0)|・キーアシスト設定(assistNameX, assistPosX_Y)を追加|
|[v12.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.1.0)|・矢印描画エリアを縮小する設定(scaleX_Y)を追加|
|[v10.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v10.2.1)|・スクロール拡張設定(scrollNameX, scrollDirX_Y)を追加|
|[v5.11.0](https://github.com/cwtickle/danoniplus/releases/tag/v5.11.0)|・タイトルバック、リトライ用ショートカットキー設定(keyRetryX_Y, keyTtitleBackX_Y)を追加|
|[v4.8.0](https://github.com/cwtickle/danoniplus/releases/tag/v4.8.0)|・別キーとしてプレイできるモードの設定(transKeyX_Y)を追加|
|[v3.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.1.0)|・ミラー／ランダムの設定(shuffleX_Y)を追加|
|[v1.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|・初期実装|