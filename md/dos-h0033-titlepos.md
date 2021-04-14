[← 譜面ヘッダー仕様に戻る](dos_header.html)
## titlepos
[ver3.x以降]

### 使い方
```
|titlepos=-5,10|
|titlepos=5,10$30,0|
```
### 説明
デフォルトの曲名表示を使用した場合に、  
タイトル文字の位置をX座標, Y座標の順で調整できます。  
単位はpxです。  
customTitleUseがfalseに設定されているとき、この値は無視されます。  

ver17.3.0より、$区切りで2行目の位置を調整できるようになりました。  
1行目の中央位置を基準にx, y座標の順に指定します。  
y座標についてはtitlelineheightとの同時適用が可能です。

### タイトル曲名文字(デフォルトデザイン)の設定箇所について
![dos-h0030-01.png](./wiki/dos-h0030-01.png)

### 関連項目
- [**titlesize**](dos-h0030-titlesize.html)  文字サイズ
- [**titlefont**](dos-h0031-titlefont.html)  フォント
- [**titlelineheight**](dos-h0034-titlelineheight.html)  複数行の際の行間

### 更新履歴

|Version|変更内容|
|----|----|
|[v17.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.3.0)|・2行目の位置設定を追加|
|[v3.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.2.0)|・初回実装|