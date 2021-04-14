[← 譜面ヘッダー仕様に戻る](dos_header.html)
## tuning

### 使い方
```
|tuning=ティックル,http://cw7.sakura.ne.jp/|
```
### 説明
製作者名及び製作者のホームページを指定します。  
ParaFla版では読込完了用の一変数でしたが、CW Editionではヘッダー扱いです。  

### 補足
「danoni_setting.js」に以下の記述を行うことでデフォルト値を指定できます。  
```javascript
// 譜面製作者名
const g_presetTuning = `name`;

// 譜面製作者URL
const g_presetTuningUrl = `https://www.google.co.jp/`;
```

ver2以前の場合は、「danoni_custom.js」（ユーザカスタムファイル）の
customTitleInit() に以下を追加することで、
製作者ホームページのデフォルト値を指定することができます。  
```javascript
if (g_headerObj.creatorUrl === location.href) {
	g_headerObj.creatorUrl = "http://(製作者ホームページのデフォルト値)";
}
```
この記述を入れた場合、製作者ホームページの省略が可能となります。
```
|tuning=ティックル|
```

### 関連項目
- [**makerView**](dos-h0050-makerView.html)  譜面別の制作者名表示設定 
- [releaseDate](dos-h0036-releaseDate.html)  作品公開日

### 更新履歴

|Version|変更内容|
|----|----|
|[v1.0.0<br>(v0.40.0)](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|初回実装|