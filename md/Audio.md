# オーディオ仕様 / Audio
- Dancing☆Onigiri (CW Edition)における音源再生は、可能な限りWeb Audio APIを使っています。  
しかし、Web Audio APIの仕様で利用できないケースがあり、  
一部でHTML5のAudio要素を使用しています。

## Web Audio APIに対応しているパターン
- :heavy_check_mark: 対応 / :x: 未対応 (HTML5 Audioで代用)

※js, txt形式(エンコード有)は楽曲データをエンコードしたデータのことです。  
　[ダンおに曲データjs化ツール](https://github.com/suzme/danoni-base64)にて変換したデータを作成できます。

|    |mp3, ogg形式|js, txt形式(エンコード有)|
|----|----|----|
|ローカル (htmlを直接開く方法)|:x:|:heavy_check_mark:|
|ローカル ([Xamppを使用してサーバーを立てる方法](HowToLocalPlay#a-ローカルサーバーを立てる))|:heavy_check_mark:|:heavy_check_mark:|
|リモート (Web上にアップロードして公開した状態)|:heavy_check_mark:|:heavy_check_mark:|

## HTML5のAudio要素を使用した場合の制限
- HTML5のAudioはWeb Audio APIよりも機能が制限されます。  
現状、以下の事象を確認しています。

- :heavy_check_mark: 問題なし / :warning: 一部問題あり / :x: 機能使用不可

||Web Audio API|HTML5 Audio|
|----|----|----|
|フェードインによる<br>譜面ズレ|:heavy_check_mark:<br>ズレなし|:warning:<br>音源によりずれることがある|
|音量設定|:heavy_check_mark:<br>問題なし|:heavy_check_mark: (Windows) 問題なし<br>:x: (Mac / iPad) 常時100％|
|フェードイン音量|:heavy_check_mark:<br>問題なし|:heavy_check_mark: (Windows) 問題なし<br>:x: (Mac / iPad) フェードインしない|
|フェードアウト音量|:heavy_check_mark:<br>問題なし|:heavy_check_mark: (Windows) 問題なし<br>:x: (Mac / iPad) フェードアウトしない|