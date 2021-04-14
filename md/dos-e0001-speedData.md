[← 譜面エフェクト仕様に戻る](dos_effect.html)
## 速度変化 ( speed_data/change, boost_data )
### 使い方
```
|speed_change=5104,-0.50,5242,0.25,5408,0.50,5464,0.75,5491,1.00|
```
**2つで1セット**。"speed_change"(5keyのみ"speed_data")が画面全体の速度変化(全体即時適用)、  
"boost_data"が指定フレーム以降の矢印の速度変化です。  
どちらも名前が異なるだけで、使い方は同じです。  
※ver8.0.0以降、キー種による"speed_data"と"speed_change"の区別が撤廃され、どちらでも使用できるようになりました。  

### 記述仕様
#### 速度変化
|番号|論理名|設定例|内容|
|----|----|----|----|
|1|Frame|1436|変更するタイミングのフレーム数を指定します。|
|2|Speed|1.5|速度の変更倍速を指定。0はストップ、マイナスは逆走。<br>逆走の場合、矢印が元の位置に戻るように留意してください。|

#### コメント
|番号|論理名|設定例|内容|
|----|----|----|----|
|1|Frame|200|フレーム数指定。指定は任意です。|
|2|Position|-|ハイフン固定。|
|3|Comment|＜コメント入力＞|コメント文を自由に入力できます。|

### 関連項目
- [displayUse](dos-h0057-displayUse.html)  Display項目の利用有無

### 更新履歴

|Version|変更内容|
|----|----|
|[v15.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.1.0)|・フレーム数、速度変化において数式指定方法を追加|
|[v8.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.0)|・キー種によるspeed_data, speed_changeの区別を撤廃|
|[v7.9.0](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.0)|・コメント行を実装|
|[v3.10.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.10.0)|・セット毎改行区切りに対応、改行区切り時は行末のカンマを任意に変更|
|[v1.0.0<br>(v0.39.0)](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)|・初回実装|
