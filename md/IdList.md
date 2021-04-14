# ID一覧
- document.querySelector(`#____`)で取得できるIdの一覧です。

## タイトル画面

### 主要Div要素
|ID名|概要|位置|補足|
|----|----|----|----|
|divBack|背景表示用|||
|backTitleSprite|backtitle_dataの表示用|||
|maskTitleSprite|masktitle_dataの表示用|||

### 表示系、リンク
|ID名|概要|位置|補足|
|----|----|----|----|
|lblTitle|Dancing☆Onigiriの文字|x=0<br>y=15||
|lblmusicTitle|曲名|x=横幅×(-1)+補正<br>y=0+補正|補正はtitleposより指定|
|btnStart|Click Here!!ボタン|x=0<br>y=縦幅-100||
|btnReset|Data Resetボタン|x=0<br>y=縦幅-20||
|btnReload|リロードボタン|x=10<br>y=10||
|lnkMaker|Makerリンク|x=20<br>y=縦幅-45||
|lnkArtist|Artistリンク|x=横幅/2<br>y=縦幅-45||
|lnkVersion|GitHubリンク|x=横幅/4<br>y=縦幅-20||
|lblWarning|警告メッセージエリア|x=0<br>y=70||

## 設定画面

### 主要Div要素
|ID名|概要|位置|補足|
|----|----|----|----|
|divBack|背景表示用|||
|optionsprite|設定一覧の表示エリア|||

### optionsprite内Div要素
|ID名|概要|位置|補足|
|----|----|----|----|
|difficultySprite|Difficultyの表示エリア|x=25<br>y=15||
|speedSprite|Speedの表示エリア|x=25<br>y=20+23×2||
|motionSprite|Motionの表示エリア|x=25<br>y=20+23×3||
|reverseSprite|Reverseの表示エリア|x=25<br>y=20+23×4||
|scrollSprite|Scrollの表示エリア|x=25<br>y=20+23×4||
|shuffleSprite|Shuffleの表示エリア|x=25<br>y=20+23×5.5||
|autoplaySprite|AutoPlayの表示エリア|x=25<br>y=20+23×6.5||
|gaugeSprite|Gaugeの表示エリア|x=25<br>y=20+23×7.5||
|adjustmentSprite|Adjustmentの表示エリア|x=25<br>y=20+23×10||
|fadeinSprite|Fadeinの表示エリア|x=25<br>y=20+23×11||
|volumeSprite|Volumeの表示エリア|x=25<br>y=20+23×12||

### difficulySprite内Div要素
|ID名|概要|位置|補足|
|----|----|----|----|
|lblDifficulty|Difficulty|x=0<br>y=-5||
|lnkDifficulty|Difficulty変更ボタン|x=160<br>y=0||
|lnkDifficultyL|Difficulty変更ボタン(左回り)|x=120<br>y=0||
|lnkDifficultyR|Difficulty変更ボタン(右回り)|x=200<br>y=0||

### 表示系、リンク
|ID名|概要|位置|補足|
|----|----|----|----|
|lblTitle|SETTINGSの文字|x=0<br>y=15||
|btnBack|Backボタン|x=0<br>y=縦幅-100||
|btnKeyConfig|KeyConfigボタン|x=横幅/3<br>y=縦幅-100||
|btnNext|Nextボタン|x=横幅×2/3<br>y=縦幅-100||
|btnDisplay|Display画面へのリンク|x=横幅/2+195<br>y=25||
|btnSave|ローカル保存ON/OFFボタン|x=0<br>y=5||
