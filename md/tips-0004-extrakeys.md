[← Tips Indexに戻る](tips-index.html)
# カスタムキーテンプレート
- 比較的利用頻度の多い多鍵(カスタムキー)のテンプレートを明記します。

## 23key
### 譜面データ本体
```
|keyExtraList=23|
|color23=3,3,3,3,4,4,4,4,0,1,0,1,0,1,0,2,0,1,0,1,0,1,0|
|chara23=aleft,adown,aup,aright,bleft,bdown,bup,bright,left,leftdia,down,space,up,rightdia,right,oni,sleft,sleftdia,sdown,sspace,sup,srightdia,sright|
|pos23=0,1,2,3,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26|
|div23=12|
|stepRtn23=0,-90,90,180,0,-90,90,180,0,30,60,90,120,150,180,onigiri,0,30,60,90,120,150,180|
|keyCtrl23=87/0,69/0,51/52,82/0,85/0,73/0,56/57,79/0,90/0,83/0,88/0,68/0,67/0,70/0,86/0,32/0,78/0,74/0,77/0,75/0,188/0,76/0,190/0|
|blank23=52.5|
|shuffle23=0,0,0,0,1,1,1,1,2,2,2,2,2,2,2,3,4,4,4,4,4,4,4|
|assist23=Left::1,1,1,1,0,0,0,0,1,1,1,1,1,1,1,0,0,0,0,0,0,0,0/Right::0,0,0,0,1,1,1,1,0,0,0,0,0,0,0,0,1,1,1,1,1,1,1|
```
### Dancing☆Onigiriエディター (CW Edition対応)
```json
{
    "23": {
      "id": 23,
      "num": 23,
      "keys": ["KeyW","KeyE","Digit3","KeyR","KeyZ","KeyS","KeyX","KeyD","KeyC","KeyF","KeyV","KeyG","KeyN","KeyJ","KeyM","KeyK","Comma","KeyL","Period","KeyU","KeyI","Digit8","KeyO"],
      "alternativeKeys": ["", "", "Digit4", "", "", "", "", "", "", "", "", "KeyH", "", "", "", "", "", "", "", "", "", "Digit9", ""],
      "noteNames": ["aleft_data", "adown_data", "aup_data", "aright_data", "left_data", "leftdia_data", "down_data", "space_data", "up_data", "rightdia_data", "right_data", "oni_data", "sleft_data", "sleftdia_data", "sdown_data", "sspace_data", "sup_data", "srightdia_data", "sright_data", "bleft_data", "bdown_data", "bup_data", "bright_data"],
      "freezeNames": ["afrzLeft_data", "afrzDown_data", "afrzUp_data", "afrzRight_data", "frzLeft_data", "frzLdia_data", "frzDown_data", "frzSpace_data", "frzUp_data", "frzRdia_data", "frzRight_data", "foni_data", "sfrzLeft_data", "sfrzLdia_data", "sfrzDown_data", "sfrzSpace_data", "sfrzUp_data", "sfrzRdia_data", "sfrzRight_data", "bfrzLeft_data", "bfrzDown_data", "bfrzUp_data", "bfrzRight_data"],
      "colorGroup": [2, 2, 2, 2, 0, 1, 0, 1, 0, 1, 0, 2, 0, 1, 0, 1, 0, 1, 0, 2, 2, 2, 2]
    }
}
```

## 動作確認バージョン
- ソース初期より利用可能

## ページ作成者
- ティックル

## 関連項目
- [キーの仕様について](keys.html)