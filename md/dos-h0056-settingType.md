[← 譜面ヘッダー仕様に戻る](dos_header.html)
## settingType
### 使い方
```
|settingType=original|
|settingType=(..)special|
|settingType=(..)setting/extra| -> settingフォルダ内の danoni_setting_extra.js を参照
```
### 説明
適用する共通設定名を指定します。  
未指定の場合、jsフォルダ内の`danoni_setting.js`が適用されます。  
上記1番目の場合、`danoni_setting_original.js`となり、2番目の場合は作品ページと同じ場所にある`danoni_setting_special.js`が読み込まれます。

### 補足
- カレントとサブディレクトリの指定により、細かい設定が可能です。
```
// 作品フォルダ上のサブフォルダ：「setting」にある danoni_setting.js を参照 
|settingType=(..)setting/|

// 作品フォルダ上のサブフォルダ：「setting」にある danoni_setting_extra.js を参照 
|settingType=(..)setting/extra|

// javascriptフォルダにある danoni_setting_extra.js を参照 
|settingType=extra|

// specialフォルダにある danoni_setting_extra.js を参照 
|settingType=../special/extra|
```

- カレント＋サブディレクトリ指定を組み合わせる場合、必ずスラッシュ`/`を入れてください。  
(入れる入れないで、意味が変わります)
```
// 作品フォルダ上のサブフォルダ：「setting」にある danoni_setting.js を参照 
|settingType=(..)setting/|

// 作品フォルダ上にある danoni_setting_setting.js を参照 
|settingType=(..)setting|
```

### 関連項目
- [**settingUse**](dos-h0035-settingUse.html)  設定項目の利用有無
- [displayUse](dos-h0057-displayUse.html)  Display項目の利用有無
- [**customjs**](dos-h0019-customjs.html)  カスタムjsファイルの指定
- [**skinType**](dos-h0054-skinType.html)  スキン設定

### 更新履歴

|Version|変更内容|
|----|----|
|[v19.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.3.0)|・カレント＋サブディレクトリ指定に対応|
|[v10.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v10.0.0)|・初回実装|