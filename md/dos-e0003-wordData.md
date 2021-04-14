[← 譜面エフェクト仕様に戻る](dos_effect.html)
## 歌詞表示 ( word_data )
### 使い方
```
|word_data=
1436,0,[fadein]
1436,0,　　♪ 降りしきる流星の雨
1638,0,　　♪ 鮮やかに染まるビジョンに
1852,0,　　♪ 瞬く閃光　気づかないまま
2028,0,　　♪ 無限の海に溺れるだけ
2242,0,[fadeout]
9000,0,[center]
9000,0,Thank You For Playing!
9120,0,[fadeout],120
|
```
3つで1セット。改行も可ですが行末にカンマが必要です。  
ParaFla版と比較して、フェードイン・アウトなどの機能が追加されています。  
※ver3.10.0以降は改行区切りを条件に、行末カンマは任意となりました。

### データ名の種類
- 使う場面の違いだけで、使い方は同じです。  
リバース用はReverse専用です。指定が無ければ、通常のものが使用されます。  
Cross, Split 他についてはScrollが`---`以外が指定された場合（通常、ステップゾーンが上下両方にある場合）のものです。

|画面|歌詞表示|
|----|----|
|メイン(通常)|word_data, <br>word2_data, <br>...|
|メイン(リバース)|wordRev_data, <br>wordRev2_data, <br>...|
|メイン(Cross, Split 他)|wordAlt_data, <br>wordAlt2_data, <br>...|

例えば 2譜面目リバース時については以下の順で適用されます。

|適用順|適用モーション|意味|
|----|----|----|
|1|wordRev2_data|歌詞表示(リバース時)の２譜面目|
|2|wordRev_data|歌詞表示(リバース時)の１譜面目|
|3|word2_data|歌詞表示(通常時)の２譜面目|
|4|word_data|歌詞表示(通常時)の１譜面目|

### 通常表記

|番号|論理名|設定例|内容|
|----|----|----|----|
|1|Frame|1436|変更するタイミングのフレーム数を指定します。|
|2|Position|0|歌詞表示する位置。<br>"0","2", ..(偶数)が上段、"1","3", ..(奇数)が下段です。|
|3|Lyrics|♪ 歌詞を表示|歌詞表示。文字色などのタグが利用できます。|

### 歌詞変化(フェードイン・アウト、表示位置変更)

|番号|論理名|設定例|内容|
|----|----|----|----|
|1|Frame|1436|変更するタイミングのフレーム数を指定します。|
|2|Position|0|歌詞表示を制御する位置。<br>"0","2", ..(偶数)が上段、"1","3", ..(奇数)が下段です。|
|3|Fadein/Out|[fadein]|キーワード指定。<br>[fadein] 歌詞フェードイン(徐々に表示)<br>[fadeout] 歌詞フェードアウト(徐々に非表示)<br>[left] 歌詞表示を左揃え<br>[center] 歌詞表示を中央揃え<br>[right] 歌詞表示を右揃え<br>[fontSize=XX] フォントサイズをXXpxに変更|
|4|FadeFrame|60|歌詞フェードイン・アウトするフレーム数を指定。<br>キーワードに[fadein][fadeout]が指定された場合のみ有効。<br>デフォルトは30フレーム。|

### コメント

|番号|論理名|設定例|内容|
|----|----|----|----|
|1|Frame|200|フレーム数指定。指定は任意です。|
|2|Position|-|ハイフン固定。|
|3|Comment|＜コメント入力＞|コメント文を自由に入力できます。|

### 補足
- ver15.3.0より、次の条件を全て満たした場合のみ、歌詞表示の上下を反転します。  
この制御設定は、[譜面ヘッダーやdanoni_setting.js](dos-h0069-wordAutoReverse.html)にて設定が可能です。
  - 上下スクロールを挟まないキーに限定（5key, 7key, 7ikey, 9A/9Bkeyなど）
  - リバース・スクロール拡張用の歌詞表示（wordRev_data / wordAlt_data）が設定されていない作品
  - SETTINGS 画面で Reverse：ON、Scroll：--- (指定なし) を指定してプレイ開始した場合
  - 歌詞表示がすべて1段表示の場合（2段の場合、反転すると文字が重なる場合があるため）

### 関連項目
- [displayUse](dos-h0057-displayUse.html)  Display項目の利用有無
- [wordAutoReverse](dos-h0069-wordAutoReverse.html)  Reverse時に歌詞表示を条件付きで反転させる設定
- [背景・マスクモーション (back_data, mask_data)](dos-e0004-animationData.html)  

### 更新履歴

|Version|変更内容|
|----|----|
|[v15.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.5.0)|・歌詞表示のフォントサイズ変更に対応|
|[v15.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.3.0)|・Reverse時に条件付きで歌詞を上下逆の位置に表示するよう変更|
|[v15.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.1.0)|・フレーム数、深度において数式記法に対応|
|[v10.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v10.2.1)|・スクロール拡張設定用歌詞表示(wordAlt_data)の実装|
|[v9.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v9.3.0)|・リバース用歌詞表示(wordRev_data)の実装|
|[v7.9.0](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.0)|・コメント行を実装|
|[v5.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v5.6.0)|・セット毎改行区切りに限り、歌詞フェードイン・アウトするフレーム数を<br>指定できるように変更（歌詞変化の4番目の項目を追加）|
|[v3.10.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.10.0)|・セット毎改行区切りに対応、改行区切り時は行末のカンマを任意に変更|
|[v1.0.0<br>(v0.46.0)](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|初回実装|