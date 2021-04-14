[← Tips Indexに戻る](tips-index.html)
# 背景の表示方法
- 背景の表示方法はいくつかあります。

## 方法
### 1. 背景スキンを利用した背景表示方法
- ここでは、スキン名を「**backgroundTest**」とします。  
この場合、「skin」フォルダに「danoni_skin_**backgroundTest**.css」  
というファイルを作る必要があります。  

- 手軽に実装するため、今回は「skin」フォルダにある  
「danoni_skin_background.css」を利用します。  
「danoni_skin_background.css」をコピーして、  
「danoni_skin_**backgroundTest**.css」を作成してください。

- 「danoni_skin_**backgroundTest**.css」を開いて、background-imageの行のコメントを外します。  
背景ファイルのあるパスを指定しておきます。  
下記は、「background」フォルダを新規に作成し、  
その中に「back123.png」という名前の背景画像を配置する例です。
```css
@charset "UTF-8";
/* 背景 */
#divBack {
	background: linear-gradient(#000000, #222222); /* 背景が使用できない場合の代替 */
	background-image: url("../background/back123.png");
}
```

- 次に、譜面ファイル側でこの背景スキンを利用するための設定を行います。
譜面データ側で、譜面ヘッダー「skinType」の2要素目に、今回作成した背景スキンを指定してください。
```
|skinType=default,backgroundTest|
```
- またこのとき、canvas要素を入れないでください。
canvas要素を入れないことで、背景用div要素(divBack)が適用されるようになります。
```html
<div id="canvas-frame" style="width:600px;">
   <!-- <canvas id="layer0" width="600" height="500"></canvas> コメントアウト -->
   <!-- <canvas id="layer1" width="600" height="500"></canvas> コメントアウト -->
</div>
```

### 2. 譜面データ（back_data）を利用した背景表示方法
- メイン画面のみ背景を表示したい場合に使用する方法です。  
「background」フォルダを新規に作成し、その中に「back123.png」という名前の背景画像を配置する例です。
```
|back_data=
0,0,../background/back123.png,,0,0,600,500
|
```
- この場合、背景サイズをゲームの縦横サイズ（この場合は600x500）  
に合わせる必要があります。  
（画像の拡大・縮小が行われるため）

## 動作確認バージョン
- v11以降で利用できます。

## ページ作成者
- ティックル

## 関連項目
- [譜面の作成概要](HowtoMake.html)
- [**skinType**](dos-h0054-skinType.html)  スキン設定
- [背景・マスクモーション (back_data, mask_data)](dos-e0004-animationData.html)