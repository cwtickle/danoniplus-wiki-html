[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# プレイ開始前設定
### 概要
- 楽曲データの読込、譜面データの分解などプレイ開始前の設定を行う。
- プレイ開始前に必ず実行される。

### 処理の流れ
1. 楽曲データのファイル名・ディレクトリ名を取得、Now Loading表示を行う ( **loadMusic** 関数 )
2. 楽曲の読込処理を行う ( **setAudio**, **initWebAudioAPI** 関数 )  
※**initWebAudioAPI**はhtmlファイル直接起動時は使用しない。詳細は[オーディオ仕様](Audio.html)を参照。
3. iOSのみ、楽曲読込終了後に「PLAY!」ボタンを表示し押した後に処理を再開させる ( **readyToStart** 関数 )
4. 譜面データの分解、速度変化・色変化などのデータ分解、ライフ設定などを行う ( **loadScoreInit** 関数 )
5. Firefoxのみ、画像ファイルが全て読込済みであることを確認してからプレイを開始 ( **loadScoreInit** 関数 )

以上の処理が完了後、プレイ画面描画を行う ( Maininit 関数 )