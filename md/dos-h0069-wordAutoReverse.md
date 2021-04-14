[← 譜面ヘッダー仕様に戻る](dos_header.html)
## wordAutoReverse

### 使い方
```
|wordAutoReverse=OFF|
```
### 説明
ver15.3.0より、Reverse時に歌詞表示を条件付きで反転する機能を実装しましたが、  
back/mask_dataとの兼ね合いや、word_dataの歌詞以外の使われ方により  
意図せず反転されてしまうケースがあるため、作品個別にこの自動制御ができるようにします。  

|値|既定|内容|
|----|----|----|
|auto|*|Reverse時に歌詞表示を条件付きで反転する|
|OFF||Reverse時に歌詞表示を反転しない|
|ON||Reverse時に条件を満たさなくても歌詞を反転する　※|

※スクロール拡張（Cross, Splitなど）を設定している場合や、  
　wordRev_dataが含まれている場合は反転しません。  
　11keyなど本来適用しないキーや、歌詞が2段になっているケースが反転可能です。  

### 補足
- 作品全体に適用する場合は、`danoni_setting.js`でも設定が可能です。  
その場合の設定値は、`g_presetWordAutoReverse`です。（適用できる値は同じ）

### 関連項目
- [stepYR](dos-h0049-stepYR.html)  ステップゾーン(下)のY座標現位置からの差分
- [bottomWordSet](dos-h0059-bottomWordSet.html)  下側の歌詞表示位置をステップゾーン位置に連動させる設定
- [歌詞表示 (word_data)](dos-e0003-wordData.html)(★)  

### 更新履歴

|Version|変更内容|
|----|----|
|[v15.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.4.0)|初回実装|