[← 譜面ヘッダー仕様に戻る](dos_header.html)
## backBright
### 使い方
```
|backBright=true|  // 背景を明色扱いにする
```
### 説明
背景を強制的に明色扱い／暗色扱いにするかどうかを設定します。  
実際に背景色を変えるのではなく、それに付属するColorTypeを明色用、暗色用に切り替えるために使用します。  
デフォルトは`false`ですが、CSS内の`.title_base`クラスで指定されているcolorが明色かどうかで初期値が変わります。

|値|既定|内容|
|----|----|----|
|false|(*)|背景を暗色扱いにする|
|true||背景を明色扱いにする|

### 関連項目
- [**defaultColorgrd**](dos-h0061-defaultColorgrd.html)  自動グラデーション設定
- [**skinType**](dos-h0054-skinType.html)  スキン設定

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.2.0)|・初回実装|