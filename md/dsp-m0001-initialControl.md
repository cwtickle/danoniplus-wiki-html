[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

# タイトル前処理
### 概要
- 外部jsファイルの読込やローカルストレージの読込、レベル計算用のデータ取得などを行う。
- 原則、この処理は1度のみ行われる。

### 処理の流れ
1. danoni_main.jsが配置されているパスを取得 ( **current** 関数 )
2. 下記のファイルを読込 ( [**loadScript**](fnc-c0010-loadScript.html) 関数 )
    - 1.で取得したパスをルートパスとして読み込む。

|フォルダ|ファイル名|必須|備考|
|----|----|----|----|
|js/lib|danoni_localbinary.js|(*)|ローカル時のみ必須、svgデータ|
|js/lib|danoni_constants.js|*|定数管理ファイル|
|js/lib|danoni_legacy_function.js||過去の関数群。必須ではないがカスタムJsで利用している場合は必要|

3. ルートdiv要素(divRoot), 背景の描画(divBack)、Now Loading表示を行う  
 ( **initialControl** 関数 )
4. 譜面の読込オプションの設定を行う。パラメータの詳細は[こちら](HowtoMake#参考その他の設定) ( **initialControl** 関数 )

|設定名|必須|備考|
|----|----|----|
|enableAmpersandSplit||譜面データ内の主要区切り文字。デフォルトは`&`と`\|`両方を区切り文字として扱う。|
|enableDecodeURI||譜面データをURIデコードするかどうかを設定します。|

5. 作品別ローカルストレージの読み込みを行う ( **loadLocalStorage** 関数 )
    - Adjustment, Volume, Appearance, Opacityの設定があれば適用、無ければ初期化を行う。
    - ハイスコア情報があればそのまま、無ければ初期化を行う。

6. HTML埋め込み、もしくは外部ファイルより譜面データを読み込む ( [**loadDos**](fnc-c0011-loadDos.html) 関数 )  
読み込んだ譜面データを分解し、`&key=value`を`g_rootObj.key=value;`の形式に変換する ( **dosConvert** 関数 )  
7. 共通設定ファイル (デフォルト：danoni_setting.js) があれば、取り込みする ( **loadSettingJs** 関数 )
8. URLのクエリに`scoreId`が含まれていれば、譜面番号を取得する ( **initAfterDosLoaded** 関数 )
9. CSSファイル読込前に必要な譜面ヘッダーを読み込んだ後、CSSファイルを読み込む ( **preheaderConvert**, **importCssFile** 関数 )
10. 譜面ヘッダー、特殊キー情報の取り込み処理を行う ( **headerConvert**, **keysConvert** 関数 )  
このタイミングで g_headerObj 及び g_keyObj が初期化される。
11. CSSファイル内の背景情報を取得するために再描画を行う ( **initAfterDosLoaded** 関数 )
12. スキンCSSファイル、プリロード指定したファイルを読み込む ( **initAfterDosLoaded** 関数 )
13. customJsファイル、譜面情報取得のため譜面全データの読込 ( **loadCustomJs**, [**loadDos**](fnc-c0011-loadDos.html), **reloadDos** 関数 )  
このタイミングで g_detailObj が初期化される。

以上の処理が完了後、タイトル画面描画を行う ( **titleinit** 関数 )
