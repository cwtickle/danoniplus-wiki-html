⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

[**<- v6**](Changelog-v6.html) | **v5** | [**v4 ->**](Changelog-v4.html)

## [Warning] 更新終了後の不具合情報
- [更新を終了したバージョンの不具合情報#v5](DeprecatedVersionBugs.html#v5) を参照

## v5.12.17 ([2019-12-14](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.17))
- 🛠️ Localhost時にフレーム数を表示するように変更 ( PR [#561](https://github.com/cwtickle/danoniplus/pull/561) )
- 🛠️ ラベルのID重複を解消 ( PR [#545](https://github.com/cwtickle/danoniplus/pull/545), [#546](https://github.com/cwtickle/danoniplus/pull/546), [#562](https://github.com/cwtickle/danoniplus/pull/562) )
- 🛠️ fileでも起動可能なようにcrossorigin属性の付加条件を変更 ( PR [#564](https://github.com/cwtickle/danoniplus/pull/564) )

## v5.12.16 ([2019-11-11](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.16))
- 🐞 MacOS, iOS (Safari)においてWeb Audio APIが動作しない問題を修正 ( PR [#523](https://github.com/cwtickle/danoniplus/pull/523), [#525](https://github.com/cwtickle/danoniplus/pull/525), [#527](https://github.com/cwtickle/danoniplus/pull/527) ) <- :boom: **initial**

## v5.12.14 ([2019-10-12](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.14))
- 🐞 低速時かつフリーズアロー開始判定時にPF判定が早まる問題を修正 ( PR [#481](https://github.com/cwtickle/danoniplus/pull/481) ) <- :boom: [**v5.7.0**](Changelog-v5.html#v570-2019-06-01)

## v5.12.13 ([2019-10-08](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.13))
- 🐞 速度変化が同一フレームにあると正常に動作しなくなる不具合を修正 ( PR [#477](https://github.com/cwtickle/danoniplus/pull/477) ) <- :boom: **initial**

## v5.12.12 ([2019-10-06](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.12))
- 🐞 エスケープ文字の適用順序誤りを修正 ( PR [#472](https://github.com/cwtickle/danoniplus/pull/472), [#473](https://github.com/cwtickle/danoniplus/pull/473) ) <- :boom: [**v0.66.x**](Changelog-v0.html#v066x-2018-11-16)

## v5.12.11 ([2019-09-30](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.11))
- 🐞 エラーウィンドウが表示されない問題を修正 ( PR [#459](https://github.com/cwtickle/danoniplus/pull/459) ) <- :boom: [**v2.6.0**](Changelog-v2.html#v260-2019-02-10)

## v5.12.10 ([2019-09-23](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.10))
- 🐞 ロード画面でEnterを押すと複数回ロードが発生する問題を修正 ( PR [#432](https://github.com/cwtickle/danoniplus/pull/432) ) <- :boom: **initial**
- 🐞 メイン画面で曲中リトライキーを連打した場合に譜面がずれることがある問題を修正 ( PR [#433](https://github.com/cwtickle/danoniplus/pull/433) ) <- :boom: **initial**

## v5.12.9 ([2019-09-16](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.9))
- 🐞 ゲームオーバー時の200ミリ秒遅延により、ハイスコア表示がおかしくなることがある問題を修正 ( PR [#428](https://github.com/cwtickle/danoniplus/pull/428) ) <- :boom: **initial**

## v5.12.8 ([2019-09-15](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.8))
- 🐞 速度変化が補正込みで負のフレームにあるときの不具合を修正 ( PR [#426](https://github.com/cwtickle/danoniplus/pull/426) ) <- :boom: **initial**

## v5.12.7 ([2019-08-03](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.7))
- 🐞 back_data, mask_dataで0フレームが指定された場合に動作しないことがある問題を修正 ( PR [#388](https://github.com/cwtickle/danoniplus/pull/388) ) <- :boom: [**v4.2.0**](Changelog-v4.html#v420-2019-04-30), [**v0.65.x**](Changelog-v0.html#v065x-2018-11-16)

## v5.12.6 ([2019-07-21](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.6))
- 🐞 リザルト画面で、フェードアウト中にTitleBack/Retryするとフェードアウト状態が引き継がれてしまう問題を修正 ( PR [#384](https://github.com/cwtickle/danoniplus/pull/384) ) <- :boom: [**v0.68.x**](Changelog-v0.html#v068x-2018-11-17)

## v5.12.5 ([2019-07-08](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.5))
- 🐞 変更したキーコンフィグ内容が反映されないことがある問題を修正 ( PR [#365](https://github.com/cwtickle/danoniplus/pull/365) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03)

## v5.12.4 ([2019-07-06](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.4))
- 🐞 フェードイン時に個別加速が掛からない問題を修正 ( PR [#363](https://github.com/cwtickle/danoniplus/pull/363) ) <- :boom: **initial**

## v5.12.3 ([2019-06-26](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.3))
- 🐞 通常キー（キーコンフィグ保存済み）が1譜面目、独自キーが2譜面目の場合に譜面の読み込みやキーコンフィグの設定ができない問題を修正 ( PR [#355](https://github.com/cwtickle/danoniplus/pull/355) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03)
- 🐞 `danoni_setting.js` の `g_presetGaugeCustom` において0が指定できない問題を修正 ( PR [#355](https://github.com/cwtickle/danoniplus/pull/355) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03)

----

## v5.12.2 ([2019-06-18](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.2))
- 🐞 フリーズアローのみの譜面が再生できない問題を修正 ( PR [#343](https://github.com/cwtickle/danoniplus/pull/343) ) <- :boom: **initial**

## v5.12.1 ([2019-06-17](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.1))
- 🛠️ フリーズアローの枠外判定の修正・見直し（条件により止まってしまう問題の修正）( PR [#341](https://github.com/cwtickle/danoniplus/pull/341) )
- 🐞 矢印の内側を塗りつぶす機能 ( PR [#340](https://github.com/cwtickle/danoniplus/pull/340) ) で、全体色変化時に矢印内側を含む全体が塗りつぶされる問題を修正 ( PR [#341](https://github.com/cwtickle/danoniplus/pull/341) ) <- :boom: [**v5.12.0**](Changelog-v5.html#v5120-2019-06-14)

## v5.12.0 ([2019-06-14](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.0))
- ⭐️ 通常矢印の内側を塗りつぶす機能を追加 ( PR [#339](https://github.com/cwtickle/danoniplus/pull/339), [#340](https://github.com/cwtickle/danoniplus/pull/340) )

## v5.11.0 ([2019-06-10](https://github.com/cwtickle/danoniplus/releases/tag/v5.11.0))
- ⭐️ PageUp/PageDown/End/Homeをキーブロック対象に追加 ( PR [#336](https://github.com/cwtickle/danoniplus/pull/336) )
- ⭐️ キー毎にタイトルバック、リトライ用ショートカットキーの指定を行えるように変更 ( PR [#337](https://github.com/cwtickle/danoniplus/pull/337) )

## v5.10.0 ([2019-06-09](https://github.com/cwtickle/danoniplus/releases/tag/v5.10.0))
- ⭐️ フリーズアローの許容フレームを譜面ヘッダーから指定できるように変更 ( PR [#333](https://github.com/cwtickle/danoniplus/pull/333) )
- ⭐️ プレイ中のショートカットキーを設定できるように変更 ( PR [#334](https://github.com/cwtickle/danoniplus/pull/334) )

## v5.9.0 ([2019-06-09](https://github.com/cwtickle/danoniplus/releases/tag/v5.9.0))
- ⭐️ 特殊キーの折り返し位置（下段終了位置）を指定できるように変更 ( PR [#331](https://github.com/cwtickle/danoniplus/pull/331) )
- 🛠️ キーコンフィグ周りのコードを整理 ( PR [#331](https://github.com/cwtickle/danoniplus/pull/331) )

## v5.8.1 ([2019-06-08](https://github.com/cwtickle/danoniplus/releases/tag/v5.8.1))
- 🐞 ステップゾーン位置がずれている問題を修正 ( PR [#330](https://github.com/cwtickle/danoniplus/pull/330) ) <- :boom: **initial**

## v5.8.0 ([2019-06-01](https://github.com/cwtickle/danoniplus/releases/tag/v5.8.0))
- ⭐️ 譜面データのURIデコードに対応 ( PR [#328](https://github.com/cwtickle/danoniplus/pull/328) )
- ⭐️ 譜面データの&区切り可否の切替機能を追加 ( PR [#328](https://github.com/cwtickle/danoniplus/pull/328) )
- 🛠️ setVal関数のboolean対応 ( PR [#328](https://github.com/cwtickle/danoniplus/pull/328) )
- 🛠️ 外部dos読み込み処理中の&を|に置き換えるreplaceを削除 ( PR [#328](https://github.com/cwtickle/danoniplus/pull/328) )

## v5.7.0 ([2019-06-01](https://github.com/cwtickle/danoniplus/releases/tag/v5.7.0))
- ⭐️ フリーズアロー開始判定の実装 ( PR [#324](https://github.com/cwtickle/danoniplus/pull/324) )
- ⭐️ 見かけフレーム数(g_scoreObj.baseFrame)の実装 ( PR [#324](https://github.com/cwtickle/danoniplus/pull/324) )
- 🛠️ デフォルト背景画像描画のスクリプトを集約 ( PR [#325](https://github.com/cwtickle/danoniplus/pull/325) )

## v5.6.6 ([2019-05-31](https://github.com/cwtickle/danoniplus/releases/tag/v5.6.6))
- 🐞 歌詞表示のフェードイン・アウトのモーションが想定より早くなる問題を修正 ( PR [#321](https://github.com/cwtickle/danoniplus/pull/321) ) <- :boom: **initial**
- 🐞 判定基準位置が1フレーム手前になっている問題を修正 ( PR [#318](https://github.com/cwtickle/danoniplus/pull/318), [#323](https://github.com/cwtickle/danoniplus/pull/323) ) <- :boom: **initial**

## v5.6.1 ([2019-05-27](https://github.com/cwtickle/danoniplus/releases/tag/v5.6.1))
- 🐞 譜面変更ボタン(setDifficulty)のカスタム関数で条件により通過できない不具合を修正 ( PR [#317](https://github.com/cwtickle/danoniplus/pull/317) ) <- :boom: [**v5.6.0**](Changelog-v5.html#v560-2019-05-26)

## v5.6.0 ([2019-05-26](https://github.com/cwtickle/danoniplus/releases/tag/v5.6.0))
- ⭐️ 歌詞フェードイン・アウトの時間の可変対応 ( PR [#315](https://github.com/cwtickle/danoniplus/pull/315) )
- ⭐️ 歌詞データのフェードイン・アウトのデフォルト時間を30→60Frameに変更 ( PR [#315](https://github.com/cwtickle/danoniplus/pull/315) )
- ⭐️ 譜面変更ボタン(setDifficulty)に対してカスタム関数を追加 ( PR [#316](https://github.com/cwtickle/danoniplus/pull/316) )

## v5.4.0 ([2019-05-26](https://github.com/cwtickle/danoniplus/releases/tag/v5.4.0))
- ⭐️ 歌詞表示(word_data)の複数階層化に対応 ( PR [#311](https://github.com/cwtickle/danoniplus/pull/311), Issue [#307](https://github.com/cwtickle/danoniplus/pull/307) )

## v5.3.0 ([2019-05-26](https://github.com/cwtickle/danoniplus/releases/tag/v5.3.0))
- 🛠️ 曲名タイトルのline-heightの指定値が小さい場合に文字欠けする問題を修正 ( PR [#309](https://github.com/cwtickle/danoniplus/pull/309) )

## v5.2.2 ([2019-05-26](https://github.com/cwtickle/danoniplus/releases/tag/v5.2.2))
- 🐞 譜面ヘッダー：titlesizeを64以上に指定すると文字欠けが起こる問題を修正 ( PR [#308](https://github.com/cwtickle/danoniplus/pull/308) ) <- :boom: [**v3.5.0**](Changelog-v3.html#v350-2019-03-23)

## v5.2.1 ([2019-05-21](https://github.com/cwtickle/danoniplus/releases/tag/v5.2.1))
- 🐞 back_data, mask_dataのフレーム数が小さすぎる場合に画面が止まる問題を修正 ( PR [#305](https://github.com/cwtickle/danoniplus/pull/305) ) <- :boom: [**v2.4.0**](Changelog-v2.html#v240-2019-02-08) 
- 🐞 既存キーの譜面から特殊キーへ移るときにリバースの設定がリセットされない問題を修正 ( PR [#305](https://github.com/cwtickle/danoniplus/pull/305) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03)

## v5.2.0 ([2019-05-20](https://github.com/cwtickle/danoniplus/releases/tag/v5.2.0))
- ⭐️ 縦方向のスケーリングに対応 ( PR [#301](https://github.com/cwtickle/danoniplus/pull/301) )  
- ⭐️ 最低・最高速度を譜面ヘッダーから設定できるように変更 ( PR [#302](https://github.com/cwtickle/danoniplus/pull/302), issue [#300](https://github.com/cwtickle/danoniplus/pull/300) ) 
- 🐞 初期倍速が速度配列に存在しない場合に速度がundefinedとなる問題を修正 ( PR [#302](https://github.com/cwtickle/danoniplus/pull/302) ) <- :boom: [**v5.0.0**](Changelog-v5.html#v500-2019-05-16)

## v5.1.1 ([2019-05-19](https://github.com/cwtickle/danoniplus/releases/tag/v5.1.1))
- 🐞 LocalStorageが設定されていないキーのときにReverseが初期化されない問題を修正 ( PR [#299](https://github.com/cwtickle/danoniplus/pull/299) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03)

## v5.1.0 ([2019-05-18](https://github.com/cwtickle/danoniplus/releases/tag/v5.1.0))
- ⭐️ タイトル（デフォルト）の行別グラデーションに対応 ( PR [#297](https://github.com/cwtickle/danoniplus/pull/297) ) 
- ⭐️ 譜面ヘッダー「titlegrd」について、他の譜面ヘッダーと同様に「0x」「#」始まり両方のカラーコードに対応 ( PR [#297](https://github.com/cwtickle/danoniplus/pull/297) ) 

## v5.0.3 ([2019-05-18](https://github.com/cwtickle/danoniplus/releases/tag/v5.0.3))
- 🐞 LocalStorageのリバース設定が元に戻ってしまう問題を修正 ( PR [#296](https://github.com/cwtickle/danoniplus/pull/296) ) <- :boom: [**v5.0.0**](Changelog-v5.html#v500-2019-05-16)

## v5.0.2 ([2019-05-17](https://github.com/cwtickle/danoniplus/releases/tag/v5.0.2))
- 🐞 特殊キーが既存キーと同一の場合に、設定画面で止まる問題を修正 ( PR [#295](https://github.com/cwtickle/danoniplus/pull/295) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03) 

## v5.0.1 ([2019-05-17](https://github.com/cwtickle/danoniplus/releases/tag/v5.0.1))
- 🛠️ 音量設定の 0.25% を廃止
- 🐞 設定画面のゲージ設定において、カーソルを動かすと詳細表示が1つずつずれる問題を修正 ( PR [#294](https://github.com/cwtickle/danoniplus/pull/294) , Issue [#293](https://github.com/cwtickle/danoniplus/pull/293) ) <- :boom: [**v5.0.0**](Changelog-v5.html#v500-2019-05-16) 
- 🐞 音量設定のカーソル方向が逆になっていた問題を修正 ( PR [#294](https://github.com/cwtickle/danoniplus/pull/294) ) <- :boom: [**v5.0.0**](Changelog-v5.html#v500-2019-05-16) 

## v5.0.0 ([2019-05-16](https://github.com/cwtickle/danoniplus/releases/tag/v5.0.0))
- 🛠️ 設定画面のスクリプトを整理 ( PR [#291](https://github.com/cwtickle/danoniplus/pull/291) ) 

[**<- v6**](Changelog-v6.html) | **v5** | [**v4 ->**](Changelog-v4.html)