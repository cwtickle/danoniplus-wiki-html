# 譜面の作成概要

## 準備するもの
- ブラウザ ([Chromeブラウザ](https://www.google.co.jp/chrome/)推奨です。）  
※必要に応じて、[ローカルでのプレイ方法](HowToLocalPlay.html)も参考にしてください。

- Dancing☆Onigiri(CW Edition)ソース一式  
(GitHubの[Releases](https://github.com/cwtickle/danoniplus/releases), もしくは`git clone`にてダウンロード)
  - Releasesからダウンロードする場合は、  
「Source code(zip)」を押すと一式がダウンロードできます。
- Dancing☆Onigiriエディター　※いずれかを利用します。
  - [Dancing☆Onigiri エディター(CW Edition 対応)](https://superkuppabros.github.io/danoni-editor/)
  - [Cross Walker](http://cw7.sakura.ne.jp/)   
-> [Tools]   
　-> Dan★Oniエディター(Ver3.6.0以降)
  - [気分転換にRPG](http://www.kt-rpg.sakura.ne.jp/)  
-> [ツール類]   
　-> editor200.lzh (5/7/7i/9/11key用) または nkeyeditor.lzh (他キー用)  
    - 「気分転換にRPG」のエディターを利用する場合、  
[こちら](https://cw7.sakura.ne.jp/gift/editorFuji_templateHTML5.zip)よりテンプレートファイルのダウンロード＆置き換えをお願いします。  

- テキストエディター (使いやすいものを利用して良い。以下はおススメを記載。)  
  - [サクラエディタ](https://sakura-editor.github.io/) : HTML, CSS編集用  
  - [Visual Studio Code](https://code.visualstudio.com/) : HTML, CSS + JavaScriptも触る人向け  

## 譜面作成の概要

1. Dancing☆Onigiri(CW Edition)ソース一式を任意のフォルダに保存します。  
2. ソース一式にある、[danoni/danoni0.html]を参考に、htmlのベースを作成します。  
最低限、下記の記述が必要です。(コピペ可)  
保存先は、[danoni]フォルダもしくは、同じ階層の任意のフォルダに置いてください。  
これだけの記述でも、起動はできるはずです。  
譜面ヘッダーで、細かい設定が可能です。詳細は[譜面ヘッダー仕様](dos_header.html)をご覧ください。  
```html
<!DOCTYPE html>
<html>
  <head>
    <!--// 文字コードの指定(Shift_jis, UTF-8など、htmlの文字コードを指定) //-->
    <meta http-equiv="Content-Type" content="text/html;charset=UTF-8">

    <!--// Javascript, CSSの利用定義 //-->
    <meta http-equiv="Content-Script-Type" content="text/javascript">
    <meta http-equiv="Content-Style-Type" content="text/css">

    <!--// Dan☆Oniで使用するJavascript, CSSファイル。このページ用の別CSSファイル等も指定できる。下記は必須。 //-->
    <script src="../js/danoni_main.js" charset="UTF-8"></script>
    <link rel="stylesheet" type="text/css" href="../css/danoni_main.css">

  </head>
  <body>
    <!--//
      譜面データ本体。最低限、下記の記述が必要です。
      括弧書きの部分とhttp://～の箇所は実際のアドレスに直す必要があります。
        musicTitle: 楽曲情報
        difData: 譜面情報 (キー数, 譜面名, 初期速度の順に指定。$区切りで複数譜面。)
        musicUrl: [music]フォルダに格納する楽曲のファイル名を指定します。
        tuning: 製作者情報
    //-->
    <input type="hidden" name="dos" id="dos" value='

|musicTitle=(曲名),(アーティスト名),http://www.google.co.jp/|
|difData=5,Normal,3.5$5,Hard,3.5|
|setColor=#99ffff,#ffff33,#ffffff,#ff0066,#ff9966|
|frzColor=#66ffff,#6666ff,#ffff66,#ffff66|
|startFrame=0|
|musicUrl=nosound.mp3|

|left_data=200|down_data=|up_data=|right_data=|space_data=300|

|tuning=(製作者名),http://www.google.co.jp/|

    '>
    <!--// Dancing☆Onigiri(CW Edition)本体。widthの値は変更可能。500px以上推奨。 //-->
    <div id="canvas-frame" style="width:500px;margin:auto;">
	<p>ゲームを準備しています...</p>
	<p>このメッセージがいつまでも消えない場合、<br>
		Google ChromeやFirefox等、HTML5に対応したブラウザをご利用ください。</p>
    </div>
  </body>
</html>
```

3. 楽曲ファイルを[music]フォルダに置きます。  
2.で記載したhtmlファイルの中の |musicUrl=nosound.mp3| という記述について、  
保存した楽曲ファイルの名前に置き換えます。  
   - サーバーにアップする際に全角文字があると支障が出ることがあるので、  
楽曲ファイルを半角英数字に置き換えることをおススメします。  

4. 作成したhtmlファイルを開いて、画面が表示されることを確認します。  
また、[Click Here!]->[Play]と進んで、指定した楽曲ファイルが読み込まれていることを確認します。  

5. 準備物の[Dancing☆Onigiriエディター]を開いて、譜面を作成します。  
   - 作り方はエディター内のヘルプを参照してください。[こことか。](http://cw7.sakura.ne.jp/gift/editor/editorhelp.html)  
   - Flash版を作ったことがある方は、この手順は全く同じです。  
   - 手順にある「dos.txt」は、上記の譜面データ本体に相当します。  
swfファイルはFlash版のみの話なので、上記のhtmlファイルがあればOKです。  

6. 作成した譜面データを、2. で作成したhtmlファイル内の下記の部分と置き換えます。  
```
|left_data=300|down_data=|up_data=|right_data=|space_data=200|
```

7. htmlファイルを保存して、楽曲・譜面が流れるか確認してください。  
タイミングはエディターを使って適宜調整してみてください。  

## 譜面データを外部ファイルで記述する場合 (ver2.5.0以降)
記述方法が異なるだけで、変数等は同じです。  
上の方法との組み合わせも可能です。

```html
<!DOCTYPE html>
<html>
  <head>
    <!--// 文字コードの指定(Shift_jis, UTF-8など、htmlの文字コードを指定) //-->
    <meta http-equiv="Content-Type" content="text/html;charset=UTF-8">

    <!--// Javascript, CSSの利用定義 //-->
    <meta http-equiv="Content-Script-Type" content="text/javascript">
    <meta http-equiv="Content-Style-Type" content="text/css">

    <!--// Dan☆Oniで使用するJavascript, CSSファイル。このページ用の別CSSファイル等も指定できる。下記は必須。 //-->
    <script src="../js/danoni_main.js" charset="UTF-8"></script>
    <link rel="stylesheet" type="text/css" href="../css/danoni_main.css">

  </head>
  <body>
    <!--// 譜面データ本体を別ファイルに記載する場合の記述 //-->
    <input type="hidden" name="externalDos" id="externalDos" value="dos1.txt">
    <!--// 譜面ファイルの文字コード設定。ページと譜面ファイル双方が同じ文字コードなら不要 //-->
    <input type="hidden" name="externalDosCharset" id="externalDosCharset" value="Shift_JIS">
    <!--// Dancing☆Onigiri(CW Edition)本体。widthの値は変更可能。500px以上推奨。 //-->
    <div id="canvas-frame" style="width:500px;margin:auto;">
	<p>ゲームを準備しています...</p>
	<p>このメッセージがいつまでも消えない場合、<br>
		Google ChromeやFirefox等、HTML5に対応したブラウザをご利用ください。</p>
    </div>
  </body>
</html>
```

外部ファイル(この場合はdos1.txt)の中身  
（上下2行ずつの文字は必須）
```javascript
function externalDosInit() {   /* 必須行 */
  g_externalDos = `            /* 必須行 */

|musicTitle=(曲名),(アーティスト名),http://www.google.co.jp/|
|difData=5,Normal,3.5$5,Hard,3.5|
|setColor=#99ffff,#ffff33,#ffffff,#ff0066,#ff9966|
|frzColor=#66ffff,#6666ff,#ffff66,#ffff66|
|startFrame=0|
|musicUrl=nosound.mp3|

|left_data=200|down_data=|up_data=|right_data=|space_data=300|

|tuning=(製作者名),http://www.google.co.jp/|

  `;                           /* 必須行 */
}                              /* 必須行 */
```

### (補足)FUJIさんエディターを使って外部譜面ファイルを作成する場合
- 以下のように設定しておくことで、テキストファイルへ直接譜面データを出力できます。

#### ヘッダ部
```javascript
function externalDosInit() {
  g_externalDos = `

|musicTitle=(曲名),(アーティスト名),http://www.google.co.jp/|
|difData=5,Normal,3.5$5,Hard,3.5|
|setColor=#99ffff,#ffff33,#ffffff,#ff0066,#ff9966|
|frzColor=#66ffff,#6666ff,#ffff66,#ffff66|
|startFrame=0|
|musicUrl=nosound.mp3|
```
#### フッタ部
- 後ろに `&tuning=NAME`が入るため、jsエラーを防ぐために最後に `//`を入れます。
```javascript
|
`;
}//
```

## 参考：その他の設定
### 譜面データのURIデコード設定
- 例えば「%26」が「&」に変換されます。デフォルトはURIデコードしません。
有効化するには、HTML側に以下を記述する必要があります。
```HTML
<input type="hidden" name="enableDecodeURI" id="enableDecodeURI" value="true">
```

### 譜面データの&区切り可否の設定
- &区切りをやめることで、曲名やURLに&が使えるようになります。
デフォルトは&, |区切りの両方を許容します。
&区切りをやめるには、HTML側に以下を記述します。
```HTML
<input type="hidden" name="enableAmpersandSplit" id="enableAmpersandSplit" value="false">
```
### 譜面毎のファイル分割設定
- `externalDos`と組み合わせて使用します。デフォルトは分割しない（false）設定です。  
分割した場合、下記の例であれば1譜面目は「musicscore.txt」、2譜面目は「musicscore2.txt」、3譜面目は「musicscore3.txt」、・・・となります。
```html
<!--// 外部dos定義 //-->
<input type="hidden" name="externalDos" id="externalDos" value="musicscore.txt">

<!--// 譜面分割フラグ（valueを"true"にすると譜面毎にファイル分割） //-->
<input type="hidden" name="externalDosDivide" id="externalDosDivide" value="true">
```

- また通常の場合、譜面番号は2譜面目なら「2」、3譜面目なら「3」となりますが、
ファイル分割しても譜面番号を変えたくないケースもあると思います。
その場合は下記の設定を追加すれば可能です。
（常に`left_data`, `down_data`のように数字無しの譜面データが読み込まれる）
```html
<!--// 譜面番号固定フラグ（valueを"true"にすると譜面番号が変わっても譜面番号は1譜面目と同じ） //-->
<input type="hidden" name="externalDosLock" id="externalDosLock" value="true">
```
