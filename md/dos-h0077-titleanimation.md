[← 譜面ヘッダー仕様に戻る](dos_header.html)
## titleanimation
### 使い方
```
|titleanimation=upToDown,120,0,linear$spinY,120,0|
```
### 説明
タイトル文字のアニメーション方法を設定します。$区切りで2行目の設定を行えます。  
なお、このタイトル文字のアニメーションは`lblmusicTitle`の子div要素に適用します。  
このため、`lblmusicTitle`に対して直接CSSアニメーションをつけた場合は、両方の設定が反映されます。  
ご注意ください。

|番号|設定例|内容|
|----|----|----|
|1|upToDown|アニメーション名|
|2|120|アニメーションフレーム数|
|3|0|アニメーション開始遅延フレーム数（既定：0フレーム）|
|4|linear|アニメーション方法（既定：ease）|

### 関連項目
- [customTitleAnimationUse](dos-h0078-customTitleAnimationUse.html)  タイトル文字のアニメーション有無設定
- [titlegrd / titlearrowgrd](dos-h0032-titlegrd.html)  グラデーション
- [titleanimationclass](dos-h0079-titleanimationclass.html)  タイトル文字のアニメーションクラス設定


### 更新履歴

|Version|変更内容|
|----|----|
|[v18.9.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.9.0)|・4番目の要素（アニメーション方法）を追加|
|[v18.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.5.0)|・初回実装|