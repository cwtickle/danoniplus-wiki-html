⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

[**<- v7**](Changelog-v7.html) | **v6** | [**v5 ->**](Changelog-v5.html)

## [Warning] 更新終了後の不具合情報
- [更新を終了したバージョンの不具合情報#v6](DeprecatedVersionBugs.html#v6) を参照

## v6.6.13 ([2019-10-13](https://github.com/cwtickle/danoniplus/releases/tag/v6.6.13))
- 🐞 ダミーIDの譜面ヘッダー誤りを修正 ( PR [#483](https://github.com/cwtickle/danoniplus/pull/483) ) <- :boom: [**v6.0.0**](Changelog-v6.html#v600-2019-06-22)
- 🐞 ダミー矢印/フリーズアロー用カスタム関数が定義できない問題を修正 ( PR [#485](https://github.com/cwtickle/danoniplus/pull/485) ) <- :boom: [**v6.1.0**](Changelog-v6.html#v610-2019-06-22)

## v6.6.11 ([2019-10-12](https://github.com/cwtickle/danoniplus/releases/tag/v6.6.11))
- 🐞 低速時かつフリーズアロー開始判定時にPF判定が早まる問題を修正 ( PR [#481](https://github.com/cwtickle/danoniplus/pull/481) ) <- :boom: [**v5.7.0**](Changelog-v5.html#v570-2019-06-01)

## v6.6.10 ([2019-10-08](https://github.com/cwtickle/danoniplus/releases/tag/v6.6.10))
- 🐞 速度変化が同一フレームにあると正常に動作しなくなる不具合を修正 ( PR [#477](https://github.com/cwtickle/danoniplus/pull/477) ) <- :boom: **initial**

## v6.6.9 ([2019-10-06](https://github.com/cwtickle/danoniplus/releases/tag/v6.6.9))
- 🐞 エスケープ文字の適用順序誤りを修正 ( PR [#472](https://github.com/cwtickle/danoniplus/pull/472), [#473](https://github.com/cwtickle/danoniplus/pull/473) ) <- :boom: [**v0.66.x**](Changelog-v0.html#v066x-2018-11-16)

## v6.6.8 ([2019-09-30](https://github.com/cwtickle/danoniplus/releases/tag/v6.6.8))
- 🐞 エラーウィンドウが表示されない問題を修正 ( PR [#459](https://github.com/cwtickle/danoniplus/pull/459) ) <- :boom: [**v2.6.0**](Changelog-v2.html#v260-2019-02-10)

## v6.6.7 ([2019-09-23](https://github.com/cwtickle/danoniplus/releases/tag/v6.6.7))
- 🐞 ロード画面でEnterを押すと複数回ロードが発生する問題を修正 ( PR [#432](https://github.com/cwtickle/danoniplus/pull/432) ) <- :boom: **initial**
- 🐞 メイン画面で曲中リトライキーを連打した場合に譜面がずれることがある問題を修正 ( PR [#433](https://github.com/cwtickle/danoniplus/pull/433) ) <- :boom: **initial**

## v6.6.6 ([2019-09-16](https://github.com/cwtickle/danoniplus/releases/tag/v6.6.6))
- 🐞 ゲームオーバー時の200ミリ秒遅延により、ハイスコア表示がおかしくなることがある問題を修正 ( PR [#428](https://github.com/cwtickle/danoniplus/pull/428) ) <- :boom: **initial**

## v6.6.5 ([2019-09-15](https://github.com/cwtickle/danoniplus/releases/tag/v6.6.5))
- 🐞 速度変化が補正込みで負のフレームにあるときの不具合を修正 ( PR [#426](https://github.com/cwtickle/danoniplus/pull/426) ) <- :boom: **initial**

## v6.6.4 ([2019-08-18](https://github.com/cwtickle/danoniplus/releases/tag/v6.6.4))
- 🐞 タイトル・リザルトモーションでループカウンターが機能していない問題を修正 ( PR [#393](https://github.com/cwtickle/danoniplus/pull/393) ) <- :boom: [**v6.3.0**](Changelog-v6.html#v630-2019-06-27)

## v6.6.3 ([2019-08-03](https://github.com/cwtickle/danoniplus/releases/tag/v6.6.3))
- 🛠️ back_data, mask_dataで0フレームが指定された場合、ステップゾーンやライフゲージの表示より早く表示されるように変更 ( PR [#388](https://github.com/cwtickle/danoniplus/pull/388) )
- 🐞 back_data, mask_dataで0フレームが指定された場合に動作しないことがある問題を修正 ( PR [#388](https://github.com/cwtickle/danoniplus/pull/388) ) <- :boom: [**v4.2.0**](Changelog-v4.html#v420-2019-04-30), [**v0.65.x**](Changelog-v0.html#v065x-2018-11-16)

## v6.6.2 ([2019-07-21](https://github.com/cwtickle/danoniplus/releases/tag/v6.6.2))
- 🐞 リザルト画面で、フェードアウト中にTitleBack/Retryするとフェードアウト状態が引き継がれてしまう問題を修正 ( PR [#384](https://github.com/cwtickle/danoniplus/pull/384) ) <- :boom: [**v0.68.x**](Changelog-v0.html#v068x-2018-11-17)

## v6.6.1 ([2019-07-18](https://github.com/cwtickle/danoniplus/releases/tag/v6.6.1))
- 🐞 特殊キーを複数譜＆複数キー指定していた場合で、片方のキーのみキーコンフィグ設定を保存していた場合に、もう片方のキーのキーコンフィグが表示できないことがある問題を修正 ( PR [#377](https://github.com/cwtickle/danoniplus/pull/377) ) <- :boom: [**v6.6.0**](Changelog-v6.html#v660-2019-07-08)

----

## v6.6.0 ([2019-07-08](https://github.com/cwtickle/danoniplus/releases/tag/v6.6.0))
- ⭐️ 特殊キー(keyExtraList指定キー)に対してリバース、キーコンフィグ保存に対応 ( PR [#365](https://github.com/cwtickle/danoniplus/pull/365) )
- 🐞 変更したキーコンフィグ内容が反映されないことがある問題を修正 ( PR [#365](https://github.com/cwtickle/danoniplus/pull/365) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03)

## v6.5.1 ([2019-07-06](https://github.com/cwtickle/danoniplus/releases/tag/v6.5.1))
- 🐞 フェードイン時に個別加速が掛からない問題を修正 ( PR [#363](https://github.com/cwtickle/danoniplus/pull/363) ) <- :boom: **initial**
- 🐞 譜面ヘッダー(frzAttempt)が機能せず、フリーズアローを離したときの許容フレーム数が実質ゼロだった問題を修正 ( PR [#363](https://github.com/cwtickle/danoniplus/pull/363) ) <- :boom: [**v6.0.0**](Changelog-v6.html#v600-2019-06-22)

## v6.5.0 ([2019-06-30](https://github.com/cwtickle/danoniplus/releases/tag/v6.5.0))
- ⭐️ ライフ上限値の設定を追加 ( PR [#361](https://github.com/cwtickle/danoniplus/pull/361), Issue [#150](https://github.com/cwtickle/danoniplus/pull/150) )
- ⭐️ ライフ制ゲージ（Original, Light, NoRecovery）の設定を譜面ヘッダーから設定できるように変更 ( PR [#361](https://github.com/cwtickle/danoniplus/pull/361) )
- 🛠️ Gaugeオプションの「No Recovery」を「NoRecovery」に表記変更 ( PR [#361](https://github.com/cwtickle/danoniplus/pull/361) )

## v6.4.0 ([2019-06-28](https://github.com/cwtickle/danoniplus/releases/tag/v6.4.0))
- ⭐️ タイトルに対してマスクモーション(masktitle_data)を実装 ( PR [#359](https://github.com/cwtickle/danoniplus/pull/359) )
- ⭐️ タイトル・リザルトのマスクモーションについて、既存のボタンを有効にするかどうかの設定を追加 ( PR [#359](https://github.com/cwtickle/danoniplus/pull/359) )

## v6.3.0 ([2019-06-27](https://github.com/cwtickle/danoniplus/releases/tag/v6.3.0))
- ⭐️ リバース用背景・マスクモーション(backRev_data, maskRev_data)の実装 ( PR [#357](https://github.com/cwtickle/danoniplus/pull/357) )
- ⭐️ リザルトモーション(backresult_data, maskresult_data)の実装 ( PR [#357](https://github.com/cwtickle/danoniplus/pull/357) )

## v6.2.1 ([2019-06-26](https://github.com/cwtickle/danoniplus/releases/tag/v6.2.1))
- 🐞 通常キー（キーコンフィグ保存済み）が1譜面目、独自キーが2譜面目の場合に譜面の読み込みやキーコンフィグの設定ができない問題を修正 ( PR [#355](https://github.com/cwtickle/danoniplus/pull/355) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03)
- 🐞 `danoni_setting.js` の `g_presetGaugeCustom` において0が指定できない問題を修正 ( PR [#355](https://github.com/cwtickle/danoniplus/pull/355) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03)

## v6.2.0 ([2019-06-23](https://github.com/cwtickle/danoniplus/releases/tag/v6.2.0))
- ⭐️ 配点と最大スコアを変数化し、danoni_custom/setting.jsから変更できるように対応 ( PR [#350](https://github.com/cwtickle/danoniplus/pull/350) )
- 🐞 ダミーフリーズアロー用関数の一部引数間違いを修正 ( PR [#353](https://github.com/cwtickle/danoniplus/pull/353) ) <- :boom: [**v6.1.0**](Changelog-v6.html#v610-2019-06-22)

## v6.1.0 ([2019-06-22](https://github.com/cwtickle/danoniplus/releases/tag/v6.1.0))
- ⭐️ ダミー矢印・フリーズアローに対してS-Random/S-Random+を実装 ( PR [#348](https://github.com/cwtickle/danoniplus/pull/348) )
- ⭐️ ダミーフリーズアローに対してカスタム判定用関数を追加 ( PR [#348](https://github.com/cwtickle/danoniplus/pull/348) )
- 🛠️ 自動判定処理周りのコードを整理 ( PR [#348](https://github.com/cwtickle/danoniplus/pull/348) )

## v6.0.0 ([2019-06-22](https://github.com/cwtickle/danoniplus/releases/tag/v6.0.0))
- ⭐️ ダミー矢印・フリーズアロー機能の実装 ( PR [#346](https://github.com/cwtickle/danoniplus/pull/346) )
- 🛠️ メイン処理を中心にコードを整理・見直し ( PR [#346](https://github.com/cwtickle/danoniplus/pull/346) )

[**<- v7**](Changelog-v7.html) | **v6** | [**v5 ->**](Changelog-v5.html)
