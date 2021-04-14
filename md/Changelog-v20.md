⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

[**<- v21**](Changelog-v21.html) | **v20** | [**v19 ->**](Changelog-v19.html)

## v20.5.3 ([2021-04-07](https://github.com/cwtickle/danoniplus/releases/tag/v20.5.3))
- 🐞 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まる問題を修正
 ( PR [#1044](https://github.com/cwtickle/danoniplus/pull/1044), Gitter [2021-04-06](https://gitter.im/danonicw/community?at=606c808592a3431fd67b1640) ) <- :boom: [**v3.1.0**](Changelog-v3.html#v310-2019-02-26)
----

## v20.5.2 ([2021-03-09](https://github.com/cwtickle/danoniplus/releases/tag/v20.5.2))
- 🐞 グラデーション文字列にdeg/radなどが入っているときに文字が表示されない問題を修正 ( PR [#1014](https://github.com/cwtickle/danoniplus/pull/1014) ) <- :boom: [**v20.5.1**](Changelog-v20.html#v2051-2021-03-06)

## v20.5.1 ([2021-03-06](https://github.com/cwtickle/danoniplus/releases/tag/v20.5.1))
- 🛠️ Base64エンコードした曲データを直接デコードするよう変更 ( PR [#1009](https://github.com/cwtickle/danoniplus/pull/1009) )
- 🛠️ キーコンフィグ、グラデーション周りのコード整理 ( PR [#1006](https://github.com/cwtickle/danoniplus/pull/1006), [#1007](https://github.com/cwtickle/danoniplus/pull/1007), [#1008](https://github.com/cwtickle/danoniplus/pull/1008) )

## v20.4.0 ([2021-02-27](https://github.com/cwtickle/danoniplus/releases/tag/v20.4.0))
- ⭐ タイトル画面、ロード画面(iOSのみ)のショートカットキーを追加 ( PR [#1002](https://github.com/cwtickle/danoniplus/pull/1002) )
- 🛠️ ショートカットキーでキーコンフィグ画面へ移動した場合、0.5秒の待ち時間を設けるよう変更 ( PR [#1002](https://github.com/cwtickle/danoniplus/pull/1002) )
- 🛠️ clearWindow関数にキーを押した状態の初期化処理、背景再描画処理を統合 ( PR [#1002](https://github.com/cwtickle/danoniplus/pull/1002), [#1003](https://github.com/cwtickle/danoniplus/pull/1003) ) 
- 🛠️ setShortcutEvent関数にcreateScTextCommon関数を包含するよう変更 ( PR [#1002](https://github.com/cwtickle/danoniplus/pull/1002) )

## v20.3.1 ([2021-02-24](https://github.com/cwtickle/danoniplus/releases/tag/v20.3.1))
- ⭐ 設定名、結果画面用の省略名を置き換える機能を実装 ( PR [#995](https://github.com/cwtickle/danoniplus/pull/995) )
- 🛠️ 譜面選択リストにあるキー別フィルターボタンのID重複を解消 ( PR [#994](https://github.com/cwtickle/danoniplus/pull/994) )
- 🛠️ MacOSのキー表示関係、ランク表示部分、その他コード重複部分を見直し ( PR [#994](https://github.com/cwtickle/danoniplus/pull/994), [#996](https://github.com/cwtickle/danoniplus/pull/996), [#998](https://github.com/cwtickle/danoniplus/pull/998), [#1000](https://github.com/cwtickle/danoniplus/pull/1000) )
- 🛠️ フォントリスト取得関数にて優先フォントが指定できるよう変更 ( PR [#994](https://github.com/cwtickle/danoniplus/pull/994) )
- 🐞 タイトル文字、譜面名のフォントサイズに関する不具合の修正 ( PR [#997](https://github.com/cwtickle/danoniplus/pull/997) ) <- :boom: [**v20.1.2**](Changelog-v20.html#v2012-2021-02-14) 

## v20.2.1 ([2021-02-20](https://github.com/cwtickle/danoniplus/releases/tag/v20.2.1))
- 🛠️ KeyConfig画面のTo Settingsボタンの表示部にg_lblNameObjを適用 ( PR [#986](https://github.com/cwtickle/danoniplus/pull/986) )
- 🛠️ ショートカット表示部分のフォーマット方法を拡張 ( PR [#987](https://github.com/cwtickle/danoniplus/pull/987) )
- 🛠️ imgタグ生成時においてcrossOrigin属性を付与するよう変更 ( PR [#988](https://github.com/cwtickle/danoniplus/pull/988) )
- 🐞 preloadFile関数において画像ファイル以外が指定された場合の問題を修正 ( PR [#989](https://github.com/cwtickle/danoniplus/pull/989) ) <- :boom: [**v18.5.0**](Changelog-v18.html#v1850-2020-12-20) 

## v20.2.0 ([2021-02-16](https://github.com/cwtickle/danoniplus/releases/tag/v20.2.0))
- ⭐ ボタン・ショートカットキー有効化までのフレーム数設定を実装 ( PR [#982](https://github.com/cwtickle/danoniplus/pull/982) )
- ⭐ 11ikeyに方向表示が異なるキーパターンを追加 ( PR [#936](https://github.com/cwtickle/danoniplus/pull/936) )
- 🛠️ キーコンフィグ画面以外の戻るボタンのショートカットキーにShift+Tabを追加割り当て ( PR [#981](https://github.com/cwtickle/danoniplus/pull/981) )
- 🛠️ MacOS/iPadOSにおいてメイン画面、キーコンフィグ画面の割り当てキーを一部変更 ( PR [#981](https://github.com/cwtickle/danoniplus/pull/981) )
- 🐞 MacOS/iPadOSにおいて結果画面のCopyResultのショートカットキーを押した後、
他のキーを押すとCopyResultが動いてしまう問題を修正 ( PR [#981](https://github.com/cwtickle/danoniplus/pull/981) ) <- :boom: [**v19.5.0**](Changelog-v19.html#v1950-2021-02-09) 
- 🐞 対象が無いときにショートカットキーを使うとエラーになることがある問題を修正 ( PR [#983](https://github.com/cwtickle/danoniplus/pull/983) ) <- :boom: [**v19.5.0**](Changelog-v19.html#v1950-2021-02-09)

## v20.1.2 ([2021-02-14](https://github.com/cwtickle/danoniplus/releases/tag/v20.1.2))
- ⭐ タイトル文字、譜面名のフォントサイズの自動設定方法を改善 ( PR [#975](https://github.com/cwtickle/danoniplus/pull/975) )
- 🛠️ Adjustment設定のショートカットにテンキーの「+」「-」を追加で割り当て ( PR [#973](https://github.com/cwtickle/danoniplus/pull/973) )

## v20.0.0 ([2021-02-12](https://github.com/cwtickle/danoniplus/releases/tag/v20.0.0))
- ⭐ ボタン処理を画面移動系とそれ以外に分離 ( PR [#970](https://github.com/cwtickle/danoniplus/pull/970) )
- ⭐ ボタンの割り込み処理を本体処理より前に挿入できるよう変更 ( PR [#970](https://github.com/cwtickle/danoniplus/pull/970) )
- ⭐ 右クリック操作の無いボタンに対して処理を追加できるように変更 ( PR [#970](https://github.com/cwtickle/danoniplus/pull/970) )
- 🛠️ 古い関数・変数の整理、単独変数のオブジェクト集約 ( PR [#971](https://github.com/cwtickle/danoniplus/pull/971) )
- 🛠️ 判定周りのコード整理 ( PR [#969](https://github.com/cwtickle/danoniplus/pull/969) )

[**<- v21**](Changelog-v21.html) | **v20** | [**v19 ->**](Changelog-v19.html)
