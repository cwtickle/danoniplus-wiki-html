# ローカルストレージ仕様 / LocalStorage
Dancing☆Onigiri (CW Edition)で使用しているローカルストレージのデータ格納仕様です。  
データはドメイン別に格納され、ドメインを跨いで共有されることはありません。  

## 作品別
- キー：作品URL (http://...)  
    - URLパラメーターの`scoreId`は無視される。
    - それ以外のURLパラメーターはURLの一部と見なされ、区別される。
- 設定値

|キー|設定値の例|補足|
|----|----|----|
|adjustment|0|作品別のAdjustmentの初期値|
|volume|75|作品別のVolume(音量)の初期値|
|highscores|7k-Normal:<br>{ii:700, shakin:20, matari:3, ...}<br>11k-Hard:<br>{ii:1100, shakin:15, matari:2, ...}|譜面別のハイスコア情報を判定数別とスコアに分けて格納。<br>キー数＋譜面名(＋制作者名※)で区別しているため、<br>この組み合わせで重複が起こらないよう譜面名を決める必要がある<br>※譜面ヘッダー：[makerView](dos-h0050-makerView.html)=trueを指定した場合のみ|
|reverseX|ON|keyExtraList指定キー(Xkey)におけるReverseの初期値|
|keyCtrlX|37, 40, (38,0), 39, 83, 68, <br>70, 32, 74, 75, 76|keyExtraList指定キー(Xkey)におけるキーコンフィグの初期値|
|keyCtrlPtnX|0|keyExtraList指定キー(Xkey)におけるベースとするキーコンフィグパターン|
|appearance|Visible|Appearanceの初期値|
|opacity|100|Opacityの初期値|
|colorType|Default|ColorTypeの初期値|
|d_stepzone|ON|Display:StepZoneの初期値|
|d_judgment|ON|Display:Judgmentの初期値|
|d_fastslow|ON|Display:FastSlowの初期値|
|d_lifegauge|ON|Display:LifeGaugeの初期値|
|d_score|ON|Display:Scoreの初期値|
|d_musicinfo|ON|Display:MusicInfoの初期値|
|d_filterline|ON|Display:FilterLineの初期値|

### ハイスコア(highscores)詳細

|キー|設定値の例|補足|
|----|----|----|
|ii|700|ハイスコアのイイの判定数|
|shakin|20|ハイスコアのシャキンの判定数|
|matari|3|ハイスコアのマターリの判定数|
|shobon|0|ハイスコアのショボーンの判定数|
|uwan|0|ハイスコアのウワァンの判定数|
|kita|70|ハイスコアのキターの判定数|
|iknai|3|ハイスコアのイクナイの判定数|
|maxCombo|200|ハイスコアのMaxCombo数|
|fmaxCombo|50|ハイスコアのフリーズアローのMaxCombo数|
|score|947000|ハイスコア|

## キー別 (keyExtraList指定作品を除く)
- キー：danonicw-Nk (Nにはキー数が入る)
- 設定値

|キー|設定値の例|補足|
|----|----|----|
|reverse|ON|Reverseの初期値|
|keyCtrl|37, 40, (38,0), 39, 83, 68, <br>70, 32, 74, 75, 76|キーコンフィグの初期値|
|keyCtrlPtn|0|ベースとするキーコンフィグパターン|

### 更新履歴

|Version|変更内容|
|----|----|
|[v18.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.3.0)|・作品別にColorTypeを自動保存する機能を実装|
|[v18.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.1.0)|・作品別にDisplay設定、Appearance、Opacityを自動保存する機能を実装|
|[v8.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v8.7.0)|・作品別のキーからscoreIdを除去するよう変更|
|[v6.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v6.6.0)|・特殊キー(keyExtraList指定キー)に対してリバース、キーコンフィグ保存機能を実装|
|[v4.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v4.6.0)|・キー毎にリバース、キーコンフィグを自動保存する機能を実装|
|[v4.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v4.3.0)|・作品別にハイスコア時のスコア・判定情報を自動保存する機能を実装|
|[v4.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v4.1.0)|・作品別にAdjustment, Volumeを自動保存する機能を実装（初回実装）|