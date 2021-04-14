[← 譜面エフェクト仕様に戻る](dos_effect.html)

## 矢印・フリーズアローモーション ( arrowMotion_data, frzMotion_data )
### 使い方
```
|arrowMotion_data=
300,20,toRight,toLeft
900,20,none
|
|frzMotion_data=
300,20,toRight,toLeft
900,20,
|
```
4つで1セット。"arrowMotion_data"が矢印用、"frzMotion_data"がフリーズアロー用です。     
どちらも名前が異なるだけで、使い方は同じです。  

### 記述仕様

|番号|論理名|設定例|内容|
|----|----|----|----|
|1|Frame|1436|変更するタイミングのフレーム数を指定します。|
|2|ColorNo|20|矢印やフリーズアローなど、変更する対象オブジェクト（矢印番号）を指定。後述します。|
|3|styleName|toRight|animation属性を記載したCSSクラス名（上スクロール用）※|
|4|styleName|toLeft|animation属性を記載したCSSクラス名（下スクロール用）※|

※省略可能です。モーションを消す場合は`none`を指定するか、空にします。  
　3番目のCSSクラス名を指定し、4番目のCSSクラス名を省略した場合は、  
　両方とも3番目のCSSクラスになります。

### 矢印番号
色変化と同様に、対象を示す矢印番号を指定します。仕様は下記の通りです。  
ver21以降は20個以上のキーに対応しました。  
個別に指定する場合は基本、1000以上の矢印番号を使用してください。

|矢印番号|論理名|内容|
|----|----|----|
|0～19 or 1000以上|矢印(個別)|ステップゾーンの左から右、上から下の順に並べたときに何番目の矢印かを指定します。<br>スタートは0からです。<br>矢印を個別に適用する際に使います。<br>キー毎のパターン0が基準です。それ以外のパターンは、ソースの中で自動選定されます。|
|20～24|矢印グループ1～5|setColorで1～5番目に指定した矢印群を指定。|

### 指定するCSSクラスについて
- 対応するCSSクラスをCSSファイル上に指定します。  
- animationに関する属性を設定したCSSクラスにします。  
ただし`animation-duration`属性は自動で設定されるため、設定不要です。
- 設定するkeyframesでは、必ず終了時(100％)に座標位置が元の位置(`translateX`, `translateY`がそれぞれ`0px`)になるようにして下さい。
```css
/* motionDataで指定するCSSクラス */
.toSpin {
    animation-name: spinY;
}
/* Y軸回転 */
@keyframes spinY {
	0% {
		transform: rotateY(0deg);
	}
	100% {
		transform: rotateY(360deg);
	}
}
```

### 関連項目
- [displayUse](dos-h0057-displayUse.html)  Display項目の利用有無

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.0.0)|・20個以上のキーに対応|
|[v7.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v7.0.0)|・初回実装|