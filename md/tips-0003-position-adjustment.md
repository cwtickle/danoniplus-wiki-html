[← Tips Indexに戻る](tips-index.html)
# 画面の位置調整方法
- ステップゾーン、判定キャラクタ、歌詞表示位置(一部)を変更できます。  
変更できるのはいずれもY座標のみです。

## 方法
### 1. ステップゾーン
- 譜面ヘッダー「stepY」「stepYR」を使用します。（関連項目を参照してください）

![dos-h0014-01.png](./wiki/dos-h0014-01.png)

### 2. 判定キャラクタ、コンボ、Fast/Slow表示
- 譜面ヘッダー「arrowJdgY」「frzJdgY」を使用します。（関連項目を参照してください）
- 判定キャラクタ、コンボ、Fast/Slow表示そのものを非表示にしたい場合は、  
下記の譜面ヘッダーを指定してください。
```
|judgmentUse=false|  // 判定キャラクタ、コンボ
|fastSlowUse=false|  // Fast/Slow表示
```

### 3. 歌詞表示
- 歌詞表示の位置そのものの変更はできませんが、  
「stepYR」の値に合わせて位置を追随させる設定が可能です。  
譜面ヘッダー「bottomWordSet」を使用します。（関連項目を参照してください）

![dos-h0059-01.png](./wiki/dos-h0059-01.png)

## 動作確認バージョン
- v11以降で利用できます。

## ページ作成者
- ティックル

## 関連項目
- [stepY](dos-h0014-stepY.html)  ステップゾーンのY座標位置
- [stepYR](dos-h0049-stepYR.html)  ステップゾーン(下)のY座標現位置からの差分
- [arrowJdgY / frzJdgY](dos-h0058-jdgY.html)  判定キャラクタのY座標位置
- [displayUse](dos-h0057-displayUse.html)  Display項目の利用有無
- [bottomWordSet](dos-h0059-bottomWordSet.html)  下側の歌詞表示位置をステップゾーン位置に連動させる設定