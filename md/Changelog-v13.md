⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

[**<- v14**](Changelog-v14.html) | **v13** | [**v12 ->**](Changelog-v12.html)

## [Warning] 更新終了後の不具合情報
- [更新を終了したバージョンの不具合情報#v13](DeprecatedVersionBugs.html#v13) を参照

## v13.6.8 ([2020-07-02](https://github.com/cwtickle/danoniplus/releases/tag/v13.6.8))
- 🛠️ バージョン比較用のリンクをSecurity Policyに変更 ( Issue [#759](https://github.com/cwtickle/danoniplus/pull/759), PR [#760](https://github.com/cwtickle/danoniplus/pull/760) )

## v13.6.7 ([2020-06-27](https://github.com/cwtickle/danoniplus/releases/tag/v13.6.7))
- 🐞 カスタムゲージ使用時にクリア失敗時のリザルトモーションが使用できない問題を修正 ( Issue [#749](https://github.com/cwtickle/danoniplus/pull/749), PR [#751](https://github.com/cwtickle/danoniplus/pull/751) ) <- :boom: [**v9.4.0**](Changelog-v9.html#v940-2019-10-20)

## v13.6.6 ([2020-06-21](https://github.com/cwtickle/danoniplus/releases/tag/v13.6.6))
- 🛠️ プレイ中に他のキーイベントが呼ばれないようにするよう変更 ( PR [#741](https://github.com/cwtickle/danoniplus/pull/741) )

## v13.6.5 ([2020-06-18](https://github.com/cwtickle/danoniplus/releases/tag/v13.6.5))
- 🐞 通常キーであらかじめデフォルトセットされているキーコンフィグパターンと異なるキーを割り当てた際、初回保存時のみそのキーがリセットされる問題を修正 ( PR [#738](https://github.com/cwtickle/danoniplus/pull/738) ) <- :boom: [**v6.6.0**](Changelog-v6.html#v660-2019-07-08)

## v13.6.4 ([2020-05-24](https://github.com/cwtickle/danoniplus/releases/tag/v13.6.4))
- 🐞 特殊キーの後に通常キーの譜面があると譜面選択できない問題を修正 ( PR [#729](https://github.com/cwtickle/danoniplus/pull/729) ) <- :boom: [**v4.6.2**](Changelog-v4.html#v462-2019-05-04)

## v13.6.3 ([2020-05-13](https://github.com/cwtickle/danoniplus/releases/tag/v13.6.3))
- 🛠️ バージョン比較用リンクを作成 ( PR [#711](https://github.com/cwtickle/danoniplus/pull/711) )

## v13.6.2 ([2020-05-04](https://github.com/cwtickle/danoniplus/releases/tag/v13.6.2))
- 🐞 フリーズ始点判定有効時、シャキン以下の判定関数に差分フレーム数としてマイナス値が渡せていない問題を修正 ( PR [#684](https://github.com/cwtickle/danoniplus/pull/684) ) <- :boom: [**v5.7.0**](Changelog-v5.html#v570-2019-06-01)

## v13.6.1 ([2020-04-29](https://github.com/cwtickle/danoniplus/releases/tag/v13.6.1))
- 🐞 キーコンフィグ画面で、割り当てキーがundefinedとなる場合がある問題を修正 ( PR [#668](https://github.com/cwtickle/danoniplus/pull/668) ) <- :boom: [**v13.3.1**](Changelog-v13.html#v1331-2020-04-12)

----

## v13.6.0 ([2020-04-25](https://github.com/cwtickle/danoniplus/releases/tag/v13.6.0))
- ⭐ 開始/終了フレームなどを指定するstartFrame, fadeFrame, endFrameについて
疑似タイマー表記に対応 ( PR [#660](https://github.com/cwtickle/danoniplus/pull/660) )

## v13.5.1 ([2020-04-16](https://github.com/cwtickle/danoniplus/releases/tag/v13.5.1))
- ⭐ 判定表示、Hidden+/Sudden+の境界線表示の透明度を調整する「Opacity」を実装 ( PR [#656](https://github.com/cwtickle/danoniplus/pull/656), [#658](https://github.com/cwtickle/danoniplus/pull/658) )
- ⭐ Hidden+, Sudden+で表示する境界線のDisplay設定(FilterLine)を追加 ( PR [#655](https://github.com/cwtickle/danoniplus/pull/655) )
- 🛠️ 厳密等価演算子が使用されていない箇所を修正 ( PR [#654](https://github.com/cwtickle/danoniplus/pull/654) )

## v13.4.0 ([2020-04-15](https://github.com/cwtickle/danoniplus/releases/tag/v13.4.0))
- ⭐ Hidden+とSudden+を同時適用する「Hid&Sud+」を実装 ( PR [#649](https://github.com/cwtickle/danoniplus/pull/649) )
- ⭐ Display:JudgmentをJudgment(判定キャラクタ)、FastSlow、Score(判定数)に分離 ( PR [#650](https://github.com/cwtickle/danoniplus/pull/650) )
- ⭐ Displayオプションのデフォルト無効化設定を追加 ( PR [#650](https://github.com/cwtickle/danoniplus/pull/650) )
- 🛠️ Hidden+, Sudden+適用時、適用するフィルターが片方しかない場合
もう片方のフィルターの境界線を非表示にするよう変更 ( PR [#649](https://github.com/cwtickle/danoniplus/pull/649) )
- 🛠️ Hidden+, Sudden+で使用するショートカットキーをDisplay画面に表示するよう変更 ( PR [#649](https://github.com/cwtickle/danoniplus/pull/649) )
- 🛠️ Shuffle機能を使用した場合のTweet表示を一部変更 ( PR [#649](https://github.com/cwtickle/danoniplus/pull/649) )

## v13.3.1 ([2020-04-12](https://github.com/cwtickle/danoniplus/releases/tag/v13.3.1))
- ⭐ 既定のキーに対して最低1つの代替キーを設定するよう変更 ( PR [#645](https://github.com/cwtickle/danoniplus/pull/645) )
- ⭐ フリーズアロー色の補完について、矢印色を優先してセットした場合の適用ルールを一部変更 ( PR [#644](https://github.com/cwtickle/danoniplus/pull/644) )
- 🐞 キーコンフィグ画面で代替キーの無効化ができない問題を修正 ( PR [#647](https://github.com/cwtickle/danoniplus/pull/647) ) <- :boom: [**v10.3.0**](Changelog-v10.html#v1030-2019-12-01)

## v13.2.1 ([2020-04-11](https://github.com/cwtickle/danoniplus/releases/tag/v13.2.1))
- 🐞 設定画面（フェードイン表示）、キーコンフィグ画面（カラータイプ）のid重複を修正 ( PR [#642](https://github.com/cwtickle/danoniplus/pull/642) ) <- :boom: [**v3.12.0**](Changelog-v3.html#v3120-2019-04-21), [**v0.76.x**](Changelog-v0.html#v076x-2018-11-24)

## v13.2.0 ([2020-04-04](https://github.com/cwtickle/danoniplus/releases/tag/v13.2.0))
- ⭐ Appearance設定に「Hidden+」「Sudden+」を追加 ( PR [#640](https://github.com/cwtickle/danoniplus/pull/640) )

## v13.1.1 ([2020-03-30](https://github.com/cwtickle/danoniplus/releases/tag/v13.1.1))
- ⭐ 従来のfrzColor補完ができる設定を追加 ( PR [#636](https://github.com/cwtickle/danoniplus/pull/636) )
- 🛠️ フリーズアロー(矢印)塗りつぶし色を6桁カラーコードで指定した場合、
透明度が100％になるように変更 ( PR [#636](https://github.com/cwtickle/danoniplus/pull/636) )
- 🛠️ danoni_setting(-template).js について、最終更新日を追加 ( PR [#637](https://github.com/cwtickle/danoniplus/pull/637) )
- 🛠️ 一部変数のconstをletに変更 ( PR [#638](https://github.com/cwtickle/danoniplus/pull/638) )

## v13.0.0 ([2020-03-29](https://github.com/cwtickle/danoniplus/releases/tag/v13.0.0))
- ⭐ 矢印塗りつぶし部分の初期色に対してグラデーション他に対応 ( PR [#626](https://github.com/cwtickle/danoniplus/pull/626) )
- ⭐ フリーズアロー初期色 (frzColor)が未定義の場合、
矢印初期色 (setColor) の値から適用する形式に変更 ( PR [#633](https://github.com/cwtickle/danoniplus/pull/633) )
- ⭐ フリーズアロー(矢印)の塗りつぶし部分に対する初期色設定を追加 ( PR [#634](https://github.com/cwtickle/danoniplus/pull/634) )
- 🛠️ 自動グラデーション設定 (defaultColorgrd) が有効のとき、
フリーズアロー失敗時の色がグラデーションしないように変更 ( PR [#633](https://github.com/cwtickle/danoniplus/pull/633) )

[**<- v14**](Changelog-v14.html) | **v13** | [**v12 ->**](Changelog-v12.html)
