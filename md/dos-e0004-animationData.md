[← 譜面エフェクト仕様に戻る](dos_effect.html)

## 背景・マスクモーション (back_data, mask_data)
### 使い方
```
|mask_data=
400,0,../img/frzbar.png,,0,250,500,250,1
700,0
|

|back_data=
200,0,../img/c_600.png,,20,20,200,200,0.5,leftToRightFade,120
200,1,../img/iyo_600.png,,220,220,200,200,1,spinY,120
300,0
320,1,../img/iyo_600.png,,220,220,200,200,0,leftToRightFade,120
400,2,文字のフローテスト,,100,140,36,0,0,fromBig,100
500,2,文字のフローテスト,,100,140,36,0,0,upToDown,100
600,2,文字のフローテスト,,100,140,36,0,1,spinX,100
700,2,文字のフローテスト,,100,140,36,0,1,spinY,100
800,2,文字のフローテスト,,100,140,36,0,1,spinZ,100
900,2,文字のフローテスト,,100,140,36,0,1
950,2
|

|backtitle_data=
200,0,../img/c_600.png,,20,20,200,200,0.5,leftToRightFade,120
200,1,../img/iyo_600.png,,220,220,200,200,1,spinY,120
300,0
320,1,../img/iyo_600.png,,220,220,200,200,0,leftToRightFade,120
400,2,文字のフローテスト,,100,140,36,0,0,fromBig,100
500,2,文字のフローテスト,,100,140,36,#ff9999,0,upToDown,100
600,2,文字のフローテスト,,100,140,36,#ffff99,1,spinX,100
700,2,文字のフローテスト,,100,140,36,#99ff99,1,spinY,100
800,2,文字のフローテスト,,100,140,36,#99ffff,1,spinZ,100
900,2,文字のフローテスト,,100,140,36,0,1
1000,0,[jump],1100,3
1050,0,[loop],200:700:700
1200,0,../img/giko_600.png,,220,220,200,200,1,spinX,120
1300,0
|
```

### データ名の種類
設定を行う画面により、データ名が異なります。  
back_data, mask_dataはメイン画面用のため、譜面別にデータを持たせることができます。  
メイン(リバース)は未指定の場合、メイン(通常)のものが採用されます。  
メイン(Cross, Split 他)についても同様です。  

|画面|背景用モーション|マスク用モーション|
|----|----|----|
|タイトル|backtitle_data|masktitle_data|
|メイン(通常)|back_data, <br>back2_data, <br>...|mask_data, <br>mask2_data, <br>...|
|メイン(リバース)|backRev_data, <br>backRev2_data, <br>...|maskRev_data, <br>maskRev2_data, <br>...|
|メイン(Cross, Split 他)|backAlt_data, <br>backAlt2_data, <br>...|maskAlt_data, <br>maskAlt2_data, <br>...|
|リザルト(クリア時)|backresult_data<br>backresult2_data<br>...|maskresult_data<br>maskresult2_data<br>...|
|リザルト(途中終了時)|backfailedS_data<br>backfailedS2_data<br>...|maskfailedS_data<br>maskfailedS2_data<br>...|
|リザルト(ノルマ失敗時)|backfailedB_data<br>backfailedB2_data<br>...|maskfailedB_data<br>maskfailedB2_data<br>...|

1行1セット。他と異なり、改行区切りです。  
それぞれはカンマ区切りで、最初の2つ以外は省略が可能です。  

設定により、&lt;img&gt;タグ版と&lt;span&gt;タグ版の2種類に分けられます。  
メイン画面以外のモーションでは、back_dataやmask_dataと利用方法は同じですが、  
フレーム移動やループ操作が可能となっています。  

タイトルモーション以外のモーションについては指定が無い場合、  
例えば 2譜面目のリザルト(ノルマ失敗時) については以下の順で適用されます。

|適用順|適用モーション|意味|
|----|----|----|
|1|backfailedB2_data|リザルト(ノルマ失敗時)の２譜面目|
|2|backfailedB_data|リザルト(ノルマ失敗時)の１譜面目|
|3|backresult2_data|リザルト(クリア時)の２譜面目|
|4|backresult_data|リザルト(クリア時)の１譜面目|

### &lt;img&gt;タグ版

|番号|論理名|設定例|内容|
|----|----|----|----|
|1|Frame|200|変更するタイミングのフレーム数を指定します。|
|2|Depth|0|背景の深度を数字で指定します。0以上の値を指定。<br>深度は大きくすることもできますが、その分背景スプライトの数が増えるので重くなる可能性があります。|
|3|Img Source|../img/c_600.png|表示する画像のパスを指定します。相対パス可。<br>画像はpng/jpg/gif/bmpのいずれかを拡張子付きで指定します。|
|4|Img Class|imgMotion|imgタグにつけるCSSのClassを設定します。以下で設定が足りない場合などに使用します。|
|5|Left(X)|25|画像を表示するX座標を指定します。|
|6|Top(Y)|30|画像を表示するY座標を指定します。|
|7|Width(X)|200|画像の横サイズをpxで指定します。デフォルトは画像自体の横サイズです。|
|8|Height(Y)|200|画像の縦サイズをpxで指定します。デフォルトは画像自体の縦サイズです。|
|9|Opacity|0.5|画像の透明度を0～1の間で指定します。デフォルトは1(透明度なし)。<br>CSSアニメーション後、表示を消したいときは0を指定するとアニメーション後に画像が消えます。|
|10|Animation-Name|leftToRightFade|CSSアニメーション名を指定します。内容はCSSで定義します。<br>デフォルトはnone(なし)です。|
|11|Animation-Duration|120|CSSアニメーションを動かす間隔をフレーム数で指定します。|

### &lt;span&gt;タグ版

|番号|論理名|設定例|内容|
|----|----|----|----|
|1|Frame|200|変更するタイミングのフレーム数を指定します。|
|2|Depth|0|背景の深度を数字で指定します。0以上の値を指定。<br>深度は大きくすることもできますが、その分背景スプライトの数が増えるので重くなる可能性があります。|
|3|Display|フローテスト|画像のパスではなく、文字を入れると&lt;span&gt;タグとして扱います。HTMLタグが使用できます。|
|4|Span Class|spanMotion|spanタグにつけるCSSのClassを設定します。以下で設定が足りない場合などに使用します。|
|5|Left(X)|25|文字を表示するX座標を指定します。|
|6|Top(Y)|30|文字を表示するY座標を指定します。|
|7|FontSize|36|画像の横サイズをpxで指定します。デフォルトは画面の横サイズです。<br>(画像自体の幅ではありません)|
|8|FontColor|#ffff00|文字の色をカラーコードで指定します。|
|9|Opacity|0.5|画像の透明度を0～1の間で指定します。デフォルトは1(透明度なし)。<br>CSSアニメーション後、表示を消したいときは0を指定するとアニメーション後に画像が消えます。|
|10|Animation-Name|leftToRightFade|CSSアニメーション名を指定します。内容はCSSで定義します。<br>デフォルトはnone(なし)です。|
|11|Animation-Duration|120|CSSアニメーションを動かす間隔をフレーム数で指定します。|

### 表示の消去

|番号|論理名|設定例|内容|
|----|----|----|----|
|1|Frame|200|変更するタイミングのフレーム数を指定します。|
|2|Depth|0|背景の深度を数字で指定します。0以上の値を指定。<br>ALLを指定した場合、全ての深度で設定されている表示を消去します。|
|3|Display||空にすると、画像・文字を消去できます。以降の指定は不要です。|

### コメント

|番号|論理名|設定例|内容|
|----|----|----|----|
|1|Frame|200|フレーム数指定。指定は任意です。|
|2|Depth|-|ハイフン固定でコメント扱いとなり、行ごと読込対象外となります。|
|3|Comment|＜演出開始＞|コメント文を自由に入力できます。|

### ループ・フレームジャンプ (タイトル/リザルトモーションのみ)

|番号|論理名|設定例|内容|
|----|----|----|----|
|1|Frame|200|変更するタイミングのフレーム数を指定します。|
|2|ー|0|指定なし|
|3|Keyword|[jump]|キーワード指定。<br>[loop]指定フレームへ戻ります。<br>[jump]ループ条件付きで指定フレームへ移動します。|
|4|gotoAndPlay|1200|移動先のフレームを指定します。<br>コロン（：）指定で、どのフレームに飛ぶかを確率で分岐できます。<br>例）300:1500 → 1/2の確率で300フレーム、1/2の確率で1500フレーム<br>例）300:300:1200 → 2/3の確率で300フレーム、1/3の確率で1200フレーム|
|5|LoopCondition|2|[jump]のみ指定。<br>ここで指定した回数分のループが終わっていれば、4で指定したフレームへ移動します。|

### 関連項目
- [displayUse](dos-h0057-displayUse.html)  Display項目の利用有無
- [masktitleButton](dos-h0043-masktitleButton.html)  タイトル画面上のボタン群の有効/無効設定
- [maskresultButton](dos-h0044-maskresultButton.html)  リザルト画面上のボタン群の有効/無効設定
- [resultMotionSet](dos-h0048-resultMotionSet.html)  リザルトモーションのON/OFF設定
- [**preloadImages**](dos-h0021-preloadImages.html)  画像ファイルの事前読み込み設定
- [**autoPreload**](dos-h0055-autoPreload.html)  画像ファイルの自動読み込み設定
- [歌詞表示 (word_data)](dos-e0003-wordData.html)(★)  

### 更新履歴

|Version|変更内容|
|----|----|
|[v18.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.4.0)|・&lt;span&gt;タグ版のDisplayにおいてHTMLタグが使えるように変更|
|[v15.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.1.0)|・フレーム数、深度において数式記法に対応|
|[v10.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v10.2.1)|・スクロール拡張設定用背景・マスクモーション<br>(backAlt_data, maskAlt_data)の実装|
|[v9.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v9.1.0)|・背景／マスクモーションの適用順序設定を追加<br>（リザルトモーションと同様の設定）|
|[v8.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.0)|・リザルトモーションの譜面別設定を実装|
|[v7.9.0](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.0)|・クリア失敗時のリザルトモーション実装<br>・コメント行を実装|
|[v7.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v7.7.0)|・表示の消去において深度「ALL」（全消去）を実装|
|[v7.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v7.6.0)|・タイトル／リザルトモーションのループ・フレームジャンプを拡張|
|[v6.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v6.3.0)|・タイトルモーション(masktitle_data), <br>　リザルトモーション(backresult_data, maskresult_data)を実装<br>・リバース用背景・マスクモーション(backRev_data, maskRev_data)の実装|
|[v4.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v4.7.0)|・タイトルモーション(backtitle_data)に対して<br>　ループ・フレームジャンプを実装|
|[v4.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v4.4.0)|・タイトルモーション(backtitle_data)を実装|
|[v4.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v4.2.0)|・マスク表示(mask_data)を実装|
|[v1.0.0<br>(v0.67.0)](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|・背景表示(back_data) 初回実装|