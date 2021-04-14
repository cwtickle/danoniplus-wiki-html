[← 譜面ヘッダー仕様に戻る](dos_header.html)
## defaultColorgrd

### 使い方
```
|defaultColorgrd=true|
|defaultColorgrd=true,#000066|
```
### 説明
譜面ヘッダー：setColor, frzColor 及び color_data, acolor_dataで指定するカラーコードについて、  
単独のカラーコードを指定した場合に自動で線形グラデーションにするかどうかを設定します。  
※titlegrd, titlearrowgrdは対象外です。

ver18.2.0より、自動グラデーションの中継色を設定できるようになりました。  
ver21.2.0より、自動グラデーションの中継色の既定値が [backBright](dos-h0081-backBright.html) や 背景状況により変わるようになりました。  
明色用と判断した場合は、既定値が #111111 に変わります。

|番号|設定例|内容|
|----|----|----|
|1|true|自動で線形グラデーションにするかどうかの設定 (既定：false)|
|2|#000066|自動グラデーションにする際の中継色の設定（既定：#eeeeee [暗色], #111111 [明色]）|

#### 変更イメージ
```
|setColor=#ffff99| // 単独のカラーコード
|setColor=to right:#ffff99:#eeeeee:#ffff99@linear-gradient| // trueにするとこの効果と同じになる
```

|値|既定|内容|
|----|----|----|
|false|*|指定なし|
|true||単独カラーコード指定を線形グラデーションに自動変更する|

### 関連項目
- [**setColor**](dos-h0003-setColor.html) (*, ★)  矢印色
- [**frzColor**](dos-h0004-frzColor.html) (*, ★)  フリーズアロー色
- [backBright](dos-h0081-backBright.html)  背景の明暗状態
- [色変化 (acolor_data, color_data)](dos-e0002-colorData.html)(★)  
- [グラデーション仕様](dos-c0001-gradation.html) 

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.2.0)|・自動グラデーションにする際の中継色のデフォルト値適用条件を変更|
|[v18.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.2.0)|・自動グラデーションにする際の中継色を実装|
|[v12.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.0.0)|・初回実装|