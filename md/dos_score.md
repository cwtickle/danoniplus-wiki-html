# 譜面本体仕様
譜面データは、譜面ヘッダーと譜面本体、画面効果データ(フッター)の3つから構成されます。  
譜面本体の仕様はParaFlaソースのものとほぼ同一です。  

ここでは譜面本体の仕様を記述しています。  
Noは上から下、左から右になるように割り振っています。パターン1基準。  

## 5key
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|left_data|frzLeft_data|0|
|1|上|down_data|frzDown_data|0|
|2|上|up_data|frzUp_data|0|
|3|上|right_data|frzRight_data|0|
|4|上|space_data|frzSpace_data|2|

## 7key
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|left_data|frzLeft_data|0|
|1|上|leftdia_data|frzLdia_data|1|
|2|上|down_data|frzDown_data|0|
|3|上|space_data|frzSpace_data|2|
|4|上|up_data|frzUp_data|0|
|5|上|rightdia_data|frzRdia_data|1|
|6|上|right_data|frzRight_data|0|

## 7ikey
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|left_data|frzLeft_data|2|
|1|上|leftdia_data|frzLdia_data|2|
|2|上|down_data|frzDown_data|2|
|3|上|space_data|frzSpace_data|0|
|4|上|up_data|frzUp_data|0|
|5|上|rightdia_data|frzRdia_data|0|
|6|上|right_data|frzRight_data|0|


## 8key
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|left_data|frzLeft_data|0|
|1|上|leftdia_data|frzLdia_data|1|
|2|上|down_data|frzDown_data|0|
|3|上|space_data|frzSpace_data|2|
|4|上|up_data|frzUp_data|0|
|5|上|rightdia_data|frzRdia_data|1|
|6|上|right_data|frzRight_data|0|
|7|上|sleft_data|sfrzLeft_data|2|

## 9Akey(DP)
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|left_data|frzLeft_data|0|
|1|上|down_data|frzDown_data|0|
|2|上|up_data|frzUp_data|0|
|3|上|right_data|frzRight_data|0|
|4|上|space_data|frzSpace_data|2|
|5|上|sleft_data|sfrzLeft_data|3|
|6|上|sdown_data|sfrzDown_data|3|
|7|上|sup_data|sfrzUp_data|3|
|8|上|sright_data|sfrzRight_data|3|

## 9Bkey
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|left_data|frzLeft_data|1|
|1|上|down_data|frzDown_data|0|
|2|上|up_data|frzUp_data|1|
|3|上|right_data|frzRight_data|0|
|4|上|space_data|frzSpace_data|2|
|5|上|sleft_data|sfrzLeft_data|0|
|6|上|sdown_data|sfrzDown_data|1|
|7|上|sup_data|sfrzUp_data|0|
|8|上|sright_data|sfrzRight_data|1|

## 9ikey
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|sleft_data|sfrzLeft_data|0|
|1|上|sdown_data|sfrzDown_data|0|
|2|上|sup_data|sfrzUp_data|0|
|3|上|sright_data|sfrzRight_data|0|
|4|下|left_data|frzLeft_data|2|
|5|下|down_data|frzDown_data|2|
|6|下|up_data|frzUp_data|2|
|7|下|right_data|frzRight_data|2|
|8|下|space_data|frzSpace_data|2|


## 11key, 11Lkey
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|sleft_data|sfrzLeft_data|3|
|1|上|sdown_data|sfrzDown_data|3|
|2|上|sup_data|sfrzUp_data|3|
|3|上|sright_data|sfrzRight_data|3|
|4|下|left_data|frzLeft_data|0|
|5|下|leftdia_data|frzLdia_data|1|
|6|下|down_data|frzDown_data|0|
|7|下|space_data|frzSpace_data|2|
|8|下|up_data|frzUp_data|0|
|9|下|rightdia_data|frzRdia_data|1|
|10|下|right_data|frzRight_data|0|

## 11Wkey
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|sleft_data|sfrzLeft_data|2|
|1|上|sdown_data|sfrzDown_data|3|
|2|上|sup_data|sfrzUp_data|3|
|3|上|sright_data|sfrzRight_data|2|
|4|下|left_data|frzLeft_data|0|
|5|下|leftdia_data|frzLdia_data|1|
|6|下|down_data|frzDown_data|0|
|7|下|space_data|frzSpace_data|2|
|8|下|up_data|frzUp_data|0|
|9|下|rightdia_data|frzRdia_data|1|
|10|下|right_data|frzRight_data|0|


## 11ikey
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|left_data|frzLeft_data|0|
|1|上|down_data|frzDown_data|0|
|2|上|gor_data|frzGor_data|2|
|3|上|up_data|frzUp_data|0|
|4|上|right_data|frzRight_data|0|
|5|上|space_data|frzSpace_data|2|
|6|上|sleft_data|sfrzLeft_data|3|
|7|上|sdown_data|sfrzDown_data|3|
|8|上|siyo_data|sfrzIyo_data|2|
|9|上|sup_data|sfrzUp_data|3|
|10|上|sright_data|sfrzRight_data|3|

## 12key
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|sleft_data|sfrzLeft_data|3|
|1|上|sdown_data|sfrzDown_data|3|
|2|上|sup_data|sfrzUp_data|3|
|3|上|sright_data|sfrzRight_data|3|
|4|下|oni_data|foni_data|2|
|5|下|left_data|frzLeft_data|0|
|6|下|leftdia_data|frzLdia_data|1|
|7|下|down_data|frzDown_data|0|
|8|下|space_data|frzSpace_data|1|
|9|下|up_data|frzUp_data|0|
|10|下|rightdia_data|frzRdia_data|1|
|11|下|right_data|frzRight_data|0|

## 13key(TP)
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|tleft_data|tfrzLeft_data|4|
|1|上|tdown_data|tfrzDown_data|4|
|2|上|tup_data|tfrzUp_data|4|
|3|上|tright_data|tfrzRight_data|4|
|4|下|left_data|frzLeft_data|0|
|5|下|down_data|frzDown_data|0|
|6|下|up_data|frzUp_data|0|
|7|下|right_data|frzRight_data|0|
|8|下|space_data|frzSpace_data|2|
|9|下|sleft_data|sfrzLeft_data|3|
|10|下|sdown_data|sfrzDown_data|3|
|11|下|sup_data|sfrzUp_data|3|
|12|下|sright_data|sfrzRight_data|3|

## 14key
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|sleftdia_data|sfrzLdia_data|4|
|1|上|sleft_data|sfrzLeft_data|3|
|2|上|sdown_data|sfrzDown_data|3|
|3|上|sup_data|sfrzUp_data|3|
|4|上|sright_data|sfrzRight_data|3|
|5|上|srightdia_data|sfrzRdia_data|4|
|6|下|oni_data|foni_data|2|
|7|下|left_data|frzLeft_data|0|
|8|下|leftdia_data|frzLdia_data|1|
|9|下|down_data|frzDown_data|0|
|10|下|space_data|frzSpace_data|1|
|11|下|up_data|frzUp_data|0|
|12|下|rightdia_data|frzRdia_data|1|
|13|下|right_data|frzRight_data|0|

## 14ikey
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|gor_data|frzGor_data|2|
|1|上|space_data|frzSpace_data|2|
|2|上|iyo_data|frzIyo_data|2|
|3|上|left_data|frzLeft_data|3|
|4|上|down_data|frzDown_data|3|
|5|上|up_data|frzUp_data|3|
|6|上|right_data|frzRight_data|3|
|7|下|sleft_data|sfrzLeft_data|0|
|8|下|sleftdia_data|sfrzLdia_data|1|
|9|下|sdown_data|sfrzDown_data|0|
|10|下|sspace_data|sfrzSpace_data|2|
|11|下|sup_data|sfrzUp_data|0|
|12|下|srightdia_data|sfrzRdia_data|1|
|13|下|sright_data|sfrzRight_data|0|

## 15Akey, 15Bkey
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|sleft_data|sfrzLeft_data|3|
|1|上|sdown_data|sfrzDown_data|3|
|2|上|sup_data|sfrzUp_data|3|
|3|上|sright_data|sfrzRight_data|3|
|4|上|tleft_data|tfrzLeft_data|4|
|5|上|tdown_data|tfrzDown_data|4|
|6|上|tup_data|tfrzUp_data|4|
|7|上|tright_data|tfrzRight_data|4|
|8|下|left_data|frzLeft_data|0|
|9|下|leftdia_data|frzLdia_data|1|
|10|下|down_data|frzDown_data|0|
|11|下|space_data|frzSpace_data|2|
|12|下|up_data|frzUp_data|0|
|13|下|rightdia_data|frzRdia_data|1|
|14|下|right_data|frzRight_data|0|

## 16ikey
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|gor_data|frzGor_data|2|
|1|上|space_data|frzSpace_data|2|
|2|上|iyo_data|frzIyo_data|2|
|3|上|left_data|frzLeft_data|3|
|4|上|down_data|frzDown_data|3|
|5|上|up_data|frzUp_data|3|
|6|上|right_data|frzRight_data|3|
|7|下|sleft_data|sfrzLeft_data|1|
|8|下|sdown_data|sfrzDown_data|0|
|9|下|sup_data|sfrzUp_data|1|
|10|下|sright_data|sfrzRight_data|0|
|11|下|aspace_data|afrzSpace_data|2|
|12|下|aleft_data|afrzLeft_data|0|
|13|下|adown_data|afrzDown_data|1|
|14|下|aup_data|afrzUp_data|0|
|15|下|aright_data|afrzRight_data|1|

## 17key
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|aleft_data|afrzLeft_data|0|
|1|上|bleft_data|bfrzLeft_data|1|
|2|上|adown_data|afrzDown_data|0|
|3|上|bdown_data|bfrzDown_data|1|
|4|上|aup_data|afrzUp_data|0|
|5|上|bup_data|bfrzUp_data|1|
|6|上|aright_data|afrzRight_data|0|
|7|上|bright_data|bfrzRight_data|1|
|8|上|space_data|frzSpace_data|2|
|9|上|cleft_data|cfrzLeft_data|3|
|10|上|dleft_data|dfrzLeft_data|4|
|11|上|cdown_data|cfrzDown_data|3|
|12|上|ddown_data|dfrzDown_data|4|
|13|上|cup_data|cfrzUp_data|3|
|14|上|dup_data|dfrzUp_data|4|
|15|上|cright_data|cfrzRight_data|3|
|16|上|dright_data|dfrzRight_data|4|

## 23key
|No|位置|矢印データ名|フリーズアローデータ名|色グループ|
|----|----|----|----|----|
|0|上|aleft_data|afrzLeft_data|3|
|1|上|adown_data|afrzDown_data|3|
|2|上|aup_data|afrzUp_data|3|
|3|上|aright_data|afrzRight_data|3|
|4|上|bleft_data|bfrzLeft_data|4|
|5|上|bdown_data|bfrzDown_data|4|
|6|上|bup_data|bfrzUp_data|4|
|7|上|bright_data|bfrzRight_data|4|
|8|下|left_data|frzLeft_data|0|
|9|下|leftdia_data|frzLdia_data|1|
|10|下|down_data|frzDown_data|0|
|11|下|space_data|frzSpace_data|1|
|12|下|up_data|frzUp_data|0|
|13|下|rightdia_data|frzRdia_data|1|
|14|下|right_data|frzRight_data|0|
|15|下|oni_data|foni_data|2|
|16|下|sleft_data|sfrzLeft_data|0|
|17|下|sleftdia_data|sfrzLdia_data|1|
|18|下|sdown_data|sfrzDown_data|0|
|19|下|sspace_data|sfrzSpace_data|1|
|20|下|sup_data|sfrzUp_data|0|
|21|下|srightdia_data|sfrzRdia_data|1|
|22|下|sright_data|sfrzRight_data|0|
