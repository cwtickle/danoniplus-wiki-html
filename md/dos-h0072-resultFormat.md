[← 譜面ヘッダー仕様に戻る](dos_header.html)
## resultFormat

### 使い方
```
|resultFormat=【#danoni[hashTag]】[musicTitle]([keyLabel]) /[maker] /Rank:[rank]/Score:[score]/Playstyle:[playStyle]/[arrowJdg]/[frzJdg]/[combo] [url]|
```
### 説明
リザルトデータ（Twitter貼り付け用データ）のフォーマット変更を行います。  
指定しない場合は、従来のリザルトデータが反映されます。  
※曲名、譜面名や判定数など、スコアを特定できないデータを外さないよう注意してください。

#### リザルトデータ用変数

|フォーマット変数|置き換え先データ|
|----|----|
|[hashTag]|ハッシュタグ|
|[musicTitle]|曲名|
|[keyLabel]|譜面名ラベル（キー数、譜面名、Shuffle）|
|[maker]|譜面製作者名|
|[rank]|ランク|
|[score]|スコア|
|[playStyle]|オプション設定|
|[arrowJdg]|矢印判定数（イイ～ウワァン）|
|[frzJdg]|フリーズアロー判定数（キター、イクナイ）|
|[maxCombo]|最大コンボ数、フリーズコンボ数|
|[url]|scoreId付きURL|

### 補足
- 上記以外のリザルトデータ用変数は共通設定ファイル内(g_presetResultVals)にて定義可能です。
- フォーマット中で特殊文字を利用する際は、特殊文字のルールに従います。

### 関連項目
- [共通設定ファイル仕様](dos_setting.html) 
- [譜面データにおける特殊文字の取り扱い](SpecialCharacters.html) 

### 更新履歴

|Version|変更内容|
|----|----|
|[v16.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v16.2.1)|初回実装|