[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# loadDos
### 概要
- 譜面データ（もしくは譜面ファイル）を読み込み、[g_rootObj](obj-v0001-g_rootObj.html)を上書きする。
- g_rootObjを上書きする際、データマージされると問題のある場合（例えば、譜面ファイルが複数あって、譜面番号が同じ場合）は
一度譜面データをクリアしてから上書き処理を行う。
- 再帰呼び出し時かつ譜面ファイル分割が有効な場合で、初期色設定もしくはゲージ個別設定が各個別の譜面ファイルに書かれていた場合、初期色設定とゲージ個別設定を再設定する処理を行う。

### 引数（括弧内はデフォルト値）

|引数|型|必須|指定内容|
|----|----|----|----|
|_afterFunc|function|*|処理後のコールバック関数|
|_scoreId|number|*|譜面番号|
|_cyclicFlg|boolean||再読込フラグ。譜面詳細情報取得用で、reloadDos関数を介して再帰的にloadDosを呼び出すときに使用する。|

### 返却値
- なし

### 関数の依存関係
- **loadDos**
  - [loadScript](fnc-c0010-loadScript.html)
  - reloadDos
  - resetBaseColorList
  - resetCustomGauge
  - getGaugeSetting

### 使用例
```javascript
// loadDos呼び出し後、loadSettingJsを呼び出す
loadDos(_ => loadSettingJs(), 0);
```

### 更新履歴

|Version|変更内容|
|----|----|
|[v21.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.1.0)|・譜面分割時に個別のカスタムゲージリストを取得する処理を追加|
|[v21.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.0.0)|・譜面分割時に個別のカラーリストを取得する処理を追加|
|[v12.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.0.0)|・譜面番号、再読込フラグを追加|
|[v11.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v11.3.0)|・引数を見直し、後続処理を指定できるよう変更|
|[v8.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v8.5.0)|・譜面をファイル分割した場合に、譜面番号を常時固定するかどうかの設定を追加|
|[v7.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v7.7.0)|・初回実装|