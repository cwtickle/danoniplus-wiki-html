# 主要オブジェクトのプロパティ
- 矢印・フリーズアローが持つ属性値のプロパティです。  
v17まではオブジェクトのgetAttributeにて取得します。（型変換必要）  
v18以降は`g_attrObj.オブジェクトid名.プロパティ名`で取得できます。（型変換不要）

## 矢印 (Arrow) / フリーズアロー(FrzArrow)共通

|プロパティ名|初期設定値|意味|
|----|----|----|
|cnt|arrivalFrame [frameNum] + 1|ステップゾーン到達までの残フレーム数。<br>フレーム毎に1ずつ減算。<br>ステップゾーン到達フレーム数は速度変化等により変化するため、フレーム毎に管理した値を初期値としている。|
|boostCnt|motionFrame [frameNum]|Motionオプション(Boost, Brake)を設定した場合に使用。<br>g_workObj.motionOnFramesにBoost, Brakeを適用した場合の矢印軌道がフレーム毎に格納されており、ステップゾーン到達から逆算したフレーム数を指定する。<br>`cnt`同様にフレーム毎に1ずつ減算するが、ストップ時は（動きが止まるため）減算しない。|
|boostSpd|boostSpd * scrollDir|スクロール方向付き個別加速の倍速。|
|y|-|矢印・フリーズアローの現Y座標|
|prevY|-|矢印・フリーズアローの1フレーム前のY座標|

## フリーズアロー(FrzArrow)固有

|プロパティ名|初期設定値|意味|
|----|----|----|
|isMoving|true|フリーズアローの状態を管理する変数。<br>`true`：移動中<br>`false`：ヒット時（フリーズアロー押下中）<br>を表す。|
|frzBarLength|frzLength|フリーズアローのバーの長さ。<br>ヒット中はバーの長さが速度に応じて小さくなる。<br>フリーズアローをスルーしたときに、フリーズアローを消去するための条件としても使用している。|
|keyUpFrame|0|フリーズアローヒット時に手を離したフレーム数。<br>このフレーム数が一定以上を超えると、NG判定となる。|
|dividePos|0 or 1|スクロール方向。通常時は`0`, リバース時は`1`が入る。<br>スクロール方向が変わると開始矢印と終端矢印が逆転し、表示位置計算を変える必要があるため設定している。|
|judgEndFlg|false|判定済フラグ。判定が終わったら`true`となる。|
|dir|1 or -1|スクロール方向。通常時は`1`, リバース時は`-1`。|
|barY|-|フリーズアローバーのY座標|
|btmY|-|フリーズアロー(後発矢印)のY座標|
