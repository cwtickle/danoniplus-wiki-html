⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

[**<- v20**](Changelog-v20.html) | **v19** | [**v18** ->](Changelog-v18.html)

## v19.5.7 ([2021-04-07](https://github.com/cwtickle/danoniplus/releases/tag/v19.5.7))
- 🐞 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まる問題を修正
 ( PR [#1044](https://github.com/cwtickle/danoniplus/pull/1044), Gitter [2021-04-06](https://gitter.im/danonicw/community?at=606c808592a3431fd67b1640) ) <- :boom: [**v3.1.0**](Changelog-v3.html#v310-2019-02-26)

## v19.5.6 ([2021-03-06](https://github.com/cwtickle/danoniplus/releases/tag/v19.5.6))
- 🛠️ Base64エンコードした曲データを直接デコードするよう変更 ( PR [#1009](https://github.com/cwtickle/danoniplus/pull/1009) )

## v19.5.5 ([2021-02-20](https://github.com/cwtickle/danoniplus/releases/tag/v19.5.5))
- 🛠️ KeyConfig画面のTo Settingsボタンの表示部にg_lblNameObjを適用 ( PR [#986](https://github.com/cwtickle/danoniplus/pull/986) )
- 🛠️ imgタグ生成時においてcrossOrigin属性を付与するよう変更 ( PR [#988](https://github.com/cwtickle/danoniplus/pull/988) )
- 🐞 preloadFile関数において画像ファイル以外が指定された場合の問題を修正 ( PR [#989](https://github.com/cwtickle/danoniplus/pull/989) ) <- :boom: [**v18.5.0**](Changelog-v18.html#v1850-2020-12-20) 

## v19.5.4 ([2021-02-16](https://github.com/cwtickle/danoniplus/releases/tag/v19.5.4))
- 🛠️ キーコンフィグ画面以外の戻るボタンのショートカットキーにShift+Tabを追加割り当て ( PR [#981](https://github.com/cwtickle/danoniplus/pull/981) )
- 🛠️ MacOS/iPadOSにおいてメイン画面、キーコンフィグ画面の割り当てキーを一部変更 ( PR [#981](https://github.com/cwtickle/danoniplus/pull/981) )
- 🐞 MacOS/iPadOSにおいて結果画面のCopyResultのショートカットキーを押した後、
他のキーを押すとCopyResultが動いてしまう問題を修正 ( PR [#981](https://github.com/cwtickle/danoniplus/pull/981) ) <- :boom: [**v19.5.0**](Changelog-v19.html#v1950-2021-02-09)
- 🐞 対象が無いときにショートカットキーを使うとエラーになることがある問題を修正 ( PR [#983](https://github.com/cwtickle/danoniplus/pull/983) ) <- :boom: [**v19.5.0**](Changelog-v19.html#v1950-2021-02-09)

## v19.5.3 ([2021-02-13](https://github.com/cwtickle/danoniplus/releases/tag/v19.5.3))
- 🛠️ Adjustment設定のショートカットにテンキーの「+」「-」を追加で割り当て ( PR [#973](https://github.com/cwtickle/danoniplus/pull/973) )
----

## v19.5.2 ([2021-02-12](https://github.com/cwtickle/danoniplus/releases/tag/v19.5.2))
- 🛠️ ショートカット表示部分などで使用している共通文字を定数化・変数化 ( PR [#968](https://github.com/cwtickle/danoniplus/pull/968) )
- 🛠️ ResultViewで利用している g_resultMsgObj を廃止し、resultViewText関数へ置き換え ( PR [#968](https://github.com/cwtickle/danoniplus/pull/968) )
- 🐞 createCss2Button関数にて右クリック拡張ができない場合がある問題を修正 ( PR [#970](https://github.com/cwtickle/danoniplus/pull/970) ) <- :boom: [**v17.5.0**](Changelog-v17.html#v1750-2020-10-17)

## v19.5.0 ([2021-02-09](https://github.com/cwtickle/danoniplus/releases/tag/v19.5.0))
- ⭐ 画面別ショートカットキーを実装 ( PR [#964](https://github.com/cwtickle/danoniplus/pull/964) )
- 🛠️ Ready? の文字幅を画面幅に合わせるよう変更 ( PR [#966](https://github.com/cwtickle/danoniplus/pull/966) ) 
- 🐞 譜面明細画面でデータ出力ボタンを押した後、譜面選択できない問題を修正 ( PR [#965](https://github.com/cwtickle/danoniplus/pull/965) ) <- :boom: [**v19.3.0**](Changelog-v19.html#v1930-2021-01-30)

## v19.4.1 ([2021-02-06](https://github.com/cwtickle/danoniplus/releases/tag/v19.4.1))
- ⭐ 作品htmlの配置場所の変更に対応 ( PR [#955](https://github.com/cwtickle/danoniplus/pull/955), [#959](https://github.com/cwtickle/danoniplus/pull/959) )
- ⭐ 8keyにおいてEnterおにぎりを左側にするモードと12keyモードを実装 ( PR [#957](https://github.com/cwtickle/danoniplus/pull/957) )
- 🐞 changeStyle関数のコードミスを修正 ( PR [#958](https://github.com/cwtickle/danoniplus/pull/958) ) <- :boom: [**v17.1.0**](Changelog-v17.html#v1710-2020-09-28)

## v19.3.0 ([2021-01-30](https://github.com/cwtickle/danoniplus/releases/tag/v19.3.0))
- ⭐ ラベルテキスト及び説明文を danoni_constants.js へ移動・集約 ( PR [#946](https://github.com/cwtickle/danoniplus/pull/946) )
- ⭐ musicFolderのカレントディレクトリ指定に対応 ( Issue [#935](https://github.com/cwtickle/danoniplus/pull/935), PR [#948](https://github.com/cwtickle/danoniplus/pull/948) )
- ⭐ settingType, skinType, customjsについてカレント＋サブディレクトリ指定に対応 ( Issue [#935](https://github.com/cwtickle/danoniplus/pull/935), PR [#949](https://github.com/cwtickle/danoniplus/pull/949) )
- ⭐ danoni_setting.js 側でデフォルトスキン・デフォルトカスタムJs指定に対応 ( PR [#950](https://github.com/cwtickle/danoniplus/pull/950) )
- ⭐ Ready? 文字を直接書き換える設定を追加 ( PR [#946](https://github.com/cwtickle/danoniplus/pull/946) )
- 🛠️ 各譜面の譜面情報を出力する「データ出力」を押したとき、メッセージが出るように変更 ( PR [#946](https://github.com/cwtickle/danoniplus/pull/946) )

## v19.2.0 ([2021-01-20](https://github.com/cwtickle/danoniplus/releases/tag/v19.2.0))
- ⭐ タイトルの背景矢印の透明度を指定できるように変更 ( Gitter [2021-01-18](https://gitter.im/danonicw/community?at=60058b1d5562a61e9ab284a6), PR [#942](https://github.com/cwtickle/danoniplus/pull/942) )
- ⭐ グラデーションで色名を指定する場合に、透明度を合わせて指定できるよう変更 ( PR [#943](https://github.com/cwtickle/danoniplus/pull/943) )
- ⭐ グラデーションの角度単位にrad, grad, turnが使えるよう変更 ( PR [#943](https://github.com/cwtickle/danoniplus/pull/943) )
- 🛠️ リストのいずれかに部分一致検索（大小文字問わず）する処理を統一 ( PR [#943](https://github.com/cwtickle/danoniplus/pull/943) )

## v19.1.0 ([2021-01-18](https://github.com/cwtickle/danoniplus/releases/tag/v19.1.0))
- ⭐ danoni_setting.jsにカスタムゲージリストを追加 ( PR [#940](https://github.com/cwtickle/danoniplus/pull/940) )

## v19.0.0 ([2021-01-17](https://github.com/cwtickle/danoniplus/releases/tag/v19.0.0))
- ⭐ ゲージ設定(Gauge)のゲージ種・譜面別の入力補完に対応 ( PR [#937](https://github.com/cwtickle/danoniplus/pull/937) )
- 🛠️ コード整理、非推奨関数をlegacy_functionへ移動 ( PR [#926](https://github.com/cwtickle/danoniplus/pull/926), [#934](https://github.com/cwtickle/danoniplus/pull/934), [#938](https://github.com/cwtickle/danoniplus/pull/938) )

[**<- v20**](Changelog-v20.html) | **v19** | [**v18** ->](Changelog-v18.html)
