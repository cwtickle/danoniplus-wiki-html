# Flash版との機能差異について
- Dancing☆Onigiri (CW Edition)では基本的にParaFla!版の仕様に準拠していますが、  
細かい点が従来と異なります。

- :heavy_check_mark: 対応 / :warning: 一部対応 / :x: 未対応 / :heavy_minus_sign: 対象外(仕組み無し)

## 環境対応表
- CW Editionでは、従来FlashやParaFla!で行っている部分をJavaScriptや譜面データで置き換えます。  
※完全ではありません。
- HTML5やJavaScriptにはフレームの概念はありませんが、疑似的に再現しています。

<img src="./wiki/flash-html5.png" width="90%" alt="flash-html5">

## 動作環境

|項目|CW Edition<br>(GitHub)|ParaFla! ver 5.34x<br>(おにぎり☆ぼっくす)|Flash MX ver2<br>(祭'05)|
|----|----|----|----|
|動作環境|:heavy_check_mark:<br>Windows, MacOS, <br>Android, iOS (iPadOS)<br>(モバイルはキーボードが<br>使用できる場合に限る)|:warning:<br>Windowsのみ|:warning:<br>Windowsのみ|
|動作ブラウザ|:warning:<br>Chrome, MS Edge, Vivaldi<br>(Blink系)|:warning:<br>IE, Chrome, <br>MS Edge, Vivaldi|:warning:<br>IE, Chrome, <br>MS Edge, Vivaldi|
|開発環境|:heavy_check_mark:<br>Windows, MacOS|:warning:<br>Windowsのみ|:heavy_check_mark:<br>Windows, MacOS|
|開発言語|JavaScript (ES6), CSS 3|ActionScript 1.0|ActionScript 1.0|
|開発ツール|テキストエディター<br>(Visual Studio Code 他)|ParaFla!|Flash MX|
|ローカルプレイ|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
|使用可能音源|:heavy_check_mark:<br>mp3, wav, ogg|:warning:<br>mp3のみ|:warning:<br>mp3, wav|
|画面最小サイズ|500px x 500px<br>(設定にて変更可)|500px x 400px<br>(設定にて変更可)|350px x 350px<br>(設定にて変更不可)|
|キーコンフィグ|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|

## 譜面データ
- 従来のエディターはほぼそのまま使えます。
- Flash非使用のエディターとして「[Dancing☆Onigiri エディター(CW Edition 対応)](https://github.com/superkuppabros/danoni-editor)」が開発されています。

|項目|CW Edition<br>(GitHub)|ParaFla! ver 5.34x<br>(おにぎり☆ぼっくす)|Flash MX ver2<br>(祭'05)|
|----|----|----|----|
|記載場所|htmlファイル直指定<br>もしくは<br>テキストファイル|テキストファイル|テキストファイル|
|譜面ファイルの分離|:heavy_check_mark:|:heavy_check_mark:|:x:|
|セパレート文字列|&#124;, $, :, ::<br>(&も使用可能だが<br>一部制限あり)|&, $|&|
|エディター互換|:heavy_check_mark:|:heavy_check_mark:|:warning:<br>(速度変化のみ特殊)|

### 譜面データの例
- CW Editionでも`&`区切りのデータが使えますが、特殊文字で利用しているため`|`文字の利用を推奨します。
```
&left_data=200,300&down_data=300,400&...
|left_data=200,300|down_data=300,400|...
```

## 譜面初期設定（譜面ヘッダー）
- CW Editionの場合、下記の他に数多くの設定が可能です。  
詳細は「[譜面ヘッダー仕様](dos_header.html)」をご覧ください。
- 移行ツールとして「[Dancing☆Onigiri Chart Converter](https://github.com/cwtickle/danoniplus-converter)」があります。

|項目|CW Edition<br>(GitHub)|ParaFla! ver 5.34x<br>(おにぎり☆ぼっくす)|Flash MX ver2<br>(祭'05)|
|----|----|----|----|
|musicTitle<br>(曲名、アーティスト情報)|:heavy_check_mark:|:heavy_check_mark:|:heavy_minus_sign:|
|difData<br>(譜面初期設定)|:heavy_check_mark:|:heavy_check_mark:|:heavy_minus_sign:|
|difStep<br>(difDataの旧形式。キー数)|:x:<br>(変換ツールあり)|:heavy_check_mark:|:heavy_minus_sign:|
|difName<br>(difDataの旧形式。譜面名)|:x:<br>(変換ツールあり)|:heavy_check_mark:|:heavy_minus_sign:|
|speedlock<br>(difDataの旧形式。初期速度)|:x:<br>(変換ツールあり)|:heavy_check_mark:|:heavy_minus_sign:|
|setColor<br>(矢印色設定)|:heavy_check_mark:<br>(グラデーション指定可)|:heavy_check_mark:<br>(グラデーション指定不可)|:heavy_minus_sign:|
|frzColor<br>(フリーズアロー色設定)|:heavy_check_mark:<br>(複数パターン可、グラデーション指定可)|:heavy_check_mark:<br>(1種類のみ, グラデーション指定不可)|:heavy_minus_sign:|
|startFrame<br>(楽曲フェードイン開始フレーム)|:heavy_check_mark:<br>(譜面毎に設定可)|:heavy_check_mark:<br>(全譜面共通)|:heavy_minus_sign:|
|fadeFrame<br>(楽曲フェードアウト開始フレーム)|:heavy_check_mark:|:x:|:heavy_minus_sign:|
|endFrame<br>(楽曲終了フレーム)|:heavy_check_mark:|:x:|:heavy_minus_sign:|
|musicUrl<br>(楽曲ファイルの名前)|:heavy_check_mark:|(ParaFla直指定)|:heavy_minus_sign:|
|tuning<br>(製作者情報)|:heavy_check_mark:|:heavy_check_mark:|:heavy_minus_sign:|
|TwitURL<br>(ツイッター用短縮リンク)|(自動付与)|:heavy_check_mark:|:heavy_minus_sign:|

## オブジェクトの種類

|項目|CW Edition<br>(GitHub)|ParaFla! ver 5.34x<br>(おにぎり☆ぼっくす)|Flash MX ver2<br>(祭'05)|
|----|----|----|----|
|単発矢印|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
|フリーズアロー|:heavy_check_mark:|:heavy_check_mark:|:x:|
|ダミー単発矢印|:heavy_check_mark:|:x:|:x:|
|ダミーフリーズアロー|:heavy_check_mark:|:x:|:x:|

## 譜面エフェクト
- CW Editionの場合、従来のFlash版の仕様に加えて拡張仕様があります。  
詳細は「[譜面エフェクト仕様](dos_effect.html)」をご覧ください。
- 色変化で使用する矢印番号は一部非互換です。  
「[Dancing☆Onigiri Chart Converter](https://github.com/cwtickle/danoniplus-converter)」のような変換ツールを使ったり、  
[色変化における仕様変更](dos-e0002-colorData#flash版との差異について)に関する記述を参考にしてください。

|項目|CW Edition<br>(GitHub)|ParaFla! ver 5.34x<br>(おにぎり☆ぼっくす)|Flash MX ver2<br>(祭'05)|
|----|----|----|----|
|速度変化(全体)|:heavy_check_mark:|:heavy_check_mark:|:warning:<br>(専用エディター必須)|
|速度変化(個別)|:heavy_check_mark:|:heavy_check_mark:|:x:|
|マイナス速度|:heavy_check_mark:|:heavy_check_mark:|:x:|
|色変化(全体)|:heavy_check_mark:|:heavy_check_mark:|:x:|
|色変化(個別)|:heavy_check_mark:|:heavy_check_mark:|:x:|
|歌詞表示|:heavy_check_mark:|:heavy_check_mark:|:x:|
|歌詞表示の<br>フェードイン・アウト|:heavy_check_mark:|:x:|:heavy_minus_sign:|
|歌詞表示の<br>表示位置変更|:heavy_check_mark:|:x:|:heavy_minus_sign:|
|歌詞表示の<br>フォント変更|:heavy_check_mark:|:x:|:heavy_minus_sign:|
|背景、マスク表示|:heavy_check_mark:<br>(譜面データ形式で指定)|:warning:<br>(Parafla!にて<br>独自カスタマイズ)|:warning:<br>(Flashにて<br>独自カスタマイズ)|

## プレイ中の設定

|項目|CW Edition<br>(GitHub)|ParaFla! ver 5.34x<br>(おにぎり☆ぼっくす)|Flash MX ver2<br>(祭'05)|
|----|----|----|----|
|楽曲フェードイン|:heavy_check_mark:|:heavy_check_mark:|:x:|
|楽曲フェードアウト|:heavy_check_mark:|:x:|:x:|
|曲中ショートカット|:heavy_check_mark:|:heavy_check_mark:|:x:|

## プレイ画面

|項目|CW Edition<br>(GitHub)|ParaFla! ver 5.34x<br>(おにぎり☆ぼっくす)|Flash MX ver2<br>(祭'05)|
|----|----|----|----|
|矢印・おにぎりのサイズ|すべて等幅|おにぎりのみ横長|おにぎりのみ横長|
|おにぎりのシャウト|:x:|:heavy_check_mark:|:heavy_check_mark:|
|現在の判定数表示|:heavy_check_mark:|:heavy_check_mark:|:x:|
|矢印を押したときの<br>判定に応じた色変更|:heavy_check_mark:|:heavy_check_mark:|:x:|
|現在のスコア・ランク表示|:x:|:heavy_check_mark:|:x:|
|クレジット表示|:heavy_check_mark:|:heavy_check_mark:|:x:|
|経過時間・プレイ時間表示|:heavy_check_mark:|:heavy_check_mark:|:x:|
|経過時間表示バー|:x:|:heavy_check_mark:|:x:|
|ライフ数値|:heavy_check_mark:|:x:|:x:|
|Fast/Slowの差分フレーム数|:heavy_check_mark:|:x:|:x:|
|ストップ時のキー操作|:heavy_check_mark:|:x:|:heavy_minus_sign:|
|フリーズアローを離したときの<br>猶予フレーム|:heavy_check_mark:|:heavy_check_mark:|:heavy_minus_sign:|

## 作成・プレイ可能なキー数

|項目|CW Edition<br>(GitHub)|ParaFla! ver 5.34x<br>(おにぎり☆ぼっくす)|Flash MX ver2<br>(祭'05)|
|----|----|----|----|
|5|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
|7, 7i, 8, 9A[DP], 9B, <br>11, 11L, 11i, 12, 13[TP],<br>14i, 15A, 15B, 16i, 17|:heavy_check_mark:|:heavy_check_mark:|:x:|
|9i, 11W, 14, 23|:heavy_check_mark:|:x:|:x:|
|上記以外の独自拡張キー|:heavy_check_mark:|:x:|:x:|

## キー数の設定

|項目|CW Edition<br>(GitHub)|ParaFla! ver 5.34x<br>(おにぎり☆ぼっくす)|Flash MX ver2<br>(祭'05)|
|----|----|----|----|
|代替キー|:heavy_check_mark:<br>(設定で拡張可)|:heavy_check_mark:<br>(設定で拡張不可)|:x:|
|キーコンフィグパターン|:heavy_check_mark:<br>(設定で拡張可)|:heavy_check_mark:<br>(設定で拡張不可)|:x:|
|別キーモード|:heavy_check_mark:|:x:|:x:|

## オプション

|項目|CW Edition<br>(GitHub)|ParaFla! ver 5.34x<br>(おにぎり☆ぼっくす)|Flash MX ver2<br>(祭'05)|
|----|----|----|----|
|難易度選択 (Difficulty)|:heavy_check_mark:|:heavy_check_mark:|:x:|
|譜面一覧選択、ランダム選択|:heavy_check_mark:|:x:|:x:|
|キー別譜面フィルター|:heavy_check_mark:|:x:|:x:|
|速度変更 (Speed)|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
|速度モーション変更 (Motion)|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
|ステップエリア変更 (StepArea)|:warning:<br>(Flatのみ)|:heavy_check_mark:|:x:|
|リバース (Reverse)|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
|スクロール拡張 (Scroll)|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
|画面内の非表示化 (Dark)|:heavy_check_mark:<br>(複数個別指定可)|:warning:<br>(パターン指定のみ)|:x:|
|矢印の一部非表示化 (Appearance)|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
|ライフゲージの設定 (Gauge)|:heavy_check_mark:<br>(独自ゲージ設定可)|:warning:<br>(ゲージ設定固定)|:x:|
|オートプレイ (AutoMode)|:heavy_check_mark:|:heavy_check_mark:|:x:|
|ミラー、ランダム (Shuffle)|:heavy_check_mark:|:heavy_check_mark:|:x:|
|判定位置の設定 (JudgePos)|:x:|:heavy_check_mark:|:x:|
|判定幅の設定 (JudgeRange)|:x:|:heavy_check_mark:|:x:|
|Fast/Slow表示 (TimingCheck)|:heavy_check_mark:|:heavy_check_mark:|:x:|
|空押し判定有無 (Pgya)|:x:|:heavy_check_mark:|:x:|
|矢印色調整 (ColorType)|:heavy_check_mark:|:heavy_check_mark:|:x:|

## オプション（環境設定）

|項目|CW Edition<br>(GitHub)|ParaFla! ver 5.34x<br>(おにぎり☆ぼっくす)|Flash MX ver2<br>(祭'05)|
|----|----|----|----|
|譜面位置調整 (Adjustment)|:heavy_check_mark:|:heavy_check_mark:|:x:|
|速度変化・色変化OFF|:heavy_check_mark:|:heavy_check_mark:|:x:|
|フェードイン|:heavy_check_mark:|:heavy_check_mark:|:x:|
|音量調整|:heavy_check_mark:|:heavy_check_mark:|:x:|

## 譜面情報表示

|項目|CW Edition<br>(GitHub)|ParaFla! ver 5.34x<br>(おにぎり☆ぼっくす)|Flash MX ver2<br>(祭'05)|
|----|----|----|----|
|速度変化状況|:heavy_check_mark:<br>(グラフで表示)|:warning:<br>(最大/最小のみ表示)|:x:|
|速度変化数|:heavy_check_mark:|:x:|:x:|
|譜面密度分布|:heavy_check_mark:|:x:|:x:|
|APM|:heavy_check_mark:|:x:|:x:|
|プレイ時間|:heavy_check_mark:|:x:|:x:|
|総矢印数|:heavy_check_mark:|:x:|:x:|
|総フリーズアロー数|:heavy_check_mark:|:x:|:heavy_minus_sign:|
|譜面レベル表示|:heavy_check_mark:|:x:|:x:|
|レーン別矢印数|:heavy_check_mark:|:x:|:x:|
|3つ押し箇所表示|:heavy_check_mark:|:x:|:x:|

## ローカルデータ保存

|項目|CW Edition<br>(GitHub)|ParaFla! ver 5.34x<br>(おにぎり☆ぼっくす)|Flash MX ver2<br>(祭'05)|
|----|----|----|----|
|ハイスコア|:heavy_check_mark:|:heavy_check_mark:|:heavy_minus_sign:|
|プレイ・クリア回数|:x:|:heavy_check_mark:|:heavy_minus_sign:|
|譜面位置調整 (Adjustment)|:heavy_check_mark:|:heavy_check_mark:|:heavy_minus_sign:|
|音量調整|:heavy_check_mark:|:x:|:heavy_minus_sign:|
|画面内の非表示化 (Dark)|:heavy_check_mark:|:x:|:heavy_minus_sign:|
|矢印の一部非表示化 (Appearance)|:heavy_check_mark:|:x:|:heavy_minus_sign:|
|リバース設定(キー毎)|:heavy_check_mark:|:x:|:heavy_minus_sign:|
|キーコンフィグ(キー毎)|:heavy_check_mark:|:x:|:heavy_minus_sign:|

## 結果画面

|項目|CW Edition<br>(GitHub)|ParaFla! ver 5.34x<br>(おにぎり☆ぼっくす)|Flash MX ver2<br>(祭'05)|
|----|----|----|----|
|結果判定数表示|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
|オプション利用状況表示|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
|ハイスコア表示|:heavy_check_mark:|:heavy_check_mark:|:heavy_minus_sign:|
|ハイスコア差分表示|:heavy_check_mark:|:x:|:heavy_minus_sign:|
|リザルトコピー|:heavy_check_mark:<br>(Tweet画面)|:heavy_check_mark:<br>(掲示板/Tweet)|:x:|
|リトライ|:heavy_check_mark:|:heavy_check_mark:|:x:|

## 画面の違い

|画面名|CW Edition<br>(GitHub)|ParaFla! ver 5.34x<br>(おにぎり☆ぼっくす)|Flash MX ver2<br>(祭'05)|
|----|----|----|----|
|Title|<img src="./wiki/disp/01A_title.png" width="100%">|<img src="./wiki/disp/01B_title.png" width="100%">|<img src="./wiki/disp/01C_title.png" width="100%">|
|Settings|<img src="./wiki/disp/02A_settings.png" width="100%">|<img src="./wiki/disp/02B_settings.png" width="100%">|<img src="./wiki/disp/02C_settings.png" width="100%">|
|Extra<br>Settings|<img src="./wiki/disp/03A_settingsplus.png" width="100%">|<img src="./wiki/disp/03B_settingsplus.png" width="100%">||
|KeyConfig|<img src="./wiki/disp/04A_keyconfig.png" width="100%">|<img src="./wiki/disp/04B_keyconfig.png" width="100%">|<img src="./wiki/disp/04C_keyconfig.png" width="100%">|
|Main|<img src="./wiki/disp/05A_main.png" width="100%">|<img src="./wiki/disp/05B_main.png" width="100%">|<img src="./wiki/disp/05C_main.png" width="100%">|
|Result|<img src="./wiki/disp/06A_result.png" width="100%">|<img src="./wiki/disp/06B_result.png" width="100%">|<img src="./wiki/disp/06C_result.png" width="100%">|