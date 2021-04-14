⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

[**<- v5**](Changelog-v5.html) | **v4** | [**v3 ->**](Changelog-v3.html)

## [Warning] 更新終了後の不具合情報
- [更新を終了したバージョンの不具合情報#v4](DeprecatedVersionBugs.html#v4) を参照

## v4.10.22 ([2019-10-08](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.22))
- 🐞 速度変化が同一フレームにあると正常に動作しなくなる不具合を修正 ( PR [#477](https://github.com/cwtickle/danoniplus/pull/477) ) <- :boom: **initial**

## v4.10.21 ([2019-10-06](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.21))
- 🐞 エスケープ文字の適用順序誤りを修正 ( PR [#472](https://github.com/cwtickle/danoniplus/pull/472), [#473](https://github.com/cwtickle/danoniplus/pull/473) ) <- :boom: [**v0.66.x**](Changelog-v0.html#v066x-2018-11-16)

## v4.10.20 ([2019-09-30](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.20))
- 🐞 エラーウィンドウが表示されない問題を修正 ( PR [#459](https://github.com/cwtickle/danoniplus/pull/459) ) <- :boom: [**v2.6.0**](Changelog-v2.html#v260-2019-02-10)

## v4.10.19 ([2019-09-23](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.19))
- 🐞 ロード画面でEnterを押すと複数回ロードが発生する問題を修正 ( PR [#432](https://github.com/cwtickle/danoniplus/pull/432) ) <- :boom: **initial**
- 🐞 メイン画面で曲中リトライキーを連打した場合に譜面がずれることがある問題を修正 ( PR [#433](https://github.com/cwtickle/danoniplus/pull/433) ) <- :boom: **initial**

## v4.10.18 ([2019-09-16](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.18))
- 🐞 ゲームオーバー時の200ミリ秒遅延により、ハイスコア表示がおかしくなることがある問題を修正 ( PR [#428](https://github.com/cwtickle/danoniplus/pull/428) ) <- :boom: **initial**

## v4.10.17 ([2019-09-15](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.17))
- 🐞 速度変化が補正込みで負のフレームにあるときの不具合を修正 ( PR [#426](https://github.com/cwtickle/danoniplus/pull/426) ) <- :boom: **initial**

## v4.10.16 ([2019-08-03](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.16))
- 🐞 back_data, mask_dataで0フレームが指定された場合に動作しないことがある問題を修正 ( PR [#388](https://github.com/cwtickle/danoniplus/pull/388) ) <- :boom: [**v4.2.0**](Changelog-v4.html#v420-2019-04-30), [**v0.65.x**](Changelog-v0.html#v065x-2018-11-16)

## v4.10.15 ([2019-07-21](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.15))
- 🐞 リザルト画面で、フェードアウト中にTitleBack/Retryするとフェードアウト状態が引き継がれてしまう問題を修正 ( PR [#384](https://github.com/cwtickle/danoniplus/pull/384) ) <- :boom: [**v0.68.x**](Changelog-v0.html#v068x-2018-11-17)

## v4.10.14 ([2019-07-08](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.14))
- 🐞 変更したキーコンフィグ内容が反映されないことがある問題を修正 ( PR [#365](https://github.com/cwtickle/danoniplus/pull/365) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03)

## v4.10.13 ([2019-07-06](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.13))
- 🐞 フェードイン時に個別加速が掛からない問題を修正 ( PR [#363](https://github.com/cwtickle/danoniplus/pull/363) ) <- :boom: **initial**

## v4.10.12 ([2019-06-27](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.12))
- 🐞 [#355](https://github.com/cwtickle/danoniplus/pull/355) にて直す必要のない条件文を再修正 <- :boom: [**v4.10.11**](Changelog-v4.html#v41011-2019-06-26)

## v4.10.11 ([2019-06-26](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.11))
- 🐞 通常キー（キーコンフィグ保存済み）が1譜面目、独自キーが2譜面目の場合に譜面の読み込みやキーコンフィグの設定ができない問題を修正 ( PR [#355](https://github.com/cwtickle/danoniplus/pull/355) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03)
- 🐞 `danoni_setting.js` の `g_presetGaugeCustom` において0が指定できない問題を修正 ( PR [#355](https://github.com/cwtickle/danoniplus/pull/355) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03)

## v4.10.10 ([2019-06-18](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.10))
- 🛠️ フリーズアローの枠外判定の修正・見直し（条件により止まってしまう問題の修正）( PR [#341](https://github.com/cwtickle/danoniplus/pull/341) )
- 🐞 フリーズアローのみの譜面が再生できない問題を修正 ( PR [#343](https://github.com/cwtickle/danoniplus/pull/343) ) <- :boom: **initial**

## v4.10.9 ([2019-05-31](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.9))
- 🐞 判定基準位置が1フレーム手前になっている問題を修正 ( PR [#318](https://github.com/cwtickle/danoniplus/pull/318), [#323](https://github.com/cwtickle/danoniplus/pull/323) ) <- :boom: **initial**

## v4.10.5 ([2019-05-26](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.5))
- 🐞 譜面ヘッダー：titlesizeを64以上に指定すると文字欠けが起こる問題を修正 ( PR [#308](https://github.com/cwtickle/danoniplus/pull/308) ) <- :boom: [**v3.5.0**](Changelog-v3.html#v350-2019-03-23)

## v4.10.4 ([2019-05-21](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.4))
- 🐞 back_data, mask_dataのフレーム数が小さすぎる場合に画面が止まる問題を修正 ( PR [#305](https://github.com/cwtickle/danoniplus/pull/305) ) <- :boom: [**v2.4.0**](Changelog-v2.html#v240-2019-02-08) 
- 🐞 既存キーの譜面から特殊キーへ移るときにリバースの設定がリセットされない問題を修正 ( PR [#305](https://github.com/cwtickle/danoniplus/pull/305) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03)

## v4.10.3 ([2019-05-19](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.3))
- 🐞 LocalStorageが設定されていないキーのときにReverseが初期化されない問題を修正 ( PR [#299](https://github.com/cwtickle/danoniplus/pull/299) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03)

## v4.10.2 ([2019-05-17](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.2))
- 🐞 特殊キーが既存キーと同一の場合に、設定画面で止まる問題を修正 ( PR [#295](https://github.com/cwtickle/danoniplus/pull/295) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03) 

----

## v4.10.1 ([2019-05-16](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.1))
- 🐞 fadeFrame指定あり・endFrameが無指定のときにendFrameが優先されない場合がある問題を修正 ( PR [#290](https://github.com/cwtickle/danoniplus/pull/290) ) <- :boom: [**v4.10.0**](Changelog-v4.html#v4100-2019-05-15) 

## v4.10.0 ([2019-05-15](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.0))
- ⭐️ 曲中リトライ以外のタイミングで曲の再読み込みを行う仕様に変更 ( PR [#288](https://github.com/cwtickle/danoniplus/pull/288) )  
- ⭐️ fadeFrameとendFrameが同時指定された場合、endFrameの時間を優先するように変更 ( PR [#289](https://github.com/cwtickle/danoniplus/pull/289) ) 
- 🛠️ ローディングバーについて、Canvas描画からdiv要素へ変更 ( PR [#288](https://github.com/cwtickle/danoniplus/pull/288) )

## v4.9.1 ([2019-05-12](https://github.com/cwtickle/danoniplus/releases/tag/v4.9.1))
- 🐞 Display画面からEnterキーで開始すると画面が止まる問題を修正 ( PR [#287](https://github.com/cwtickle/danoniplus/pull/287) ) <- :boom: [**v4.0.0**](Changelog-v4.html#v400-2019-04-25)

## v4.9.0 ([2019-05-11](https://github.com/cwtickle/danoniplus/releases/tag/v4.9.0))
- 🛠️ タイトル画面において、Maker, Artistが空のときに空ウィンドウを表示しないように修正 ( PR [#285](https://github.com/cwtickle/danoniplus/pull/285) ) 
- 🛠️ キーコンフィグ画面において、別キーモード時にデータ保存しない旨のメッセージを追加  ( PR [#285](https://github.com/cwtickle/danoniplus/pull/285) ) 

## v4.8.1 ([2019-05-11](https://github.com/cwtickle/danoniplus/releases/tag/v4.8.1))
- 🐞 ライフ回復・ダメージ量計算でフリーズアローのカウントが間違っていたのを修正 ( PR [#284](https://github.com/cwtickle/danoniplus/pull/284) ) <- :boom: [**v0.72.x**](Changelog-v0.html#v072x-2018-11-20)

## v4.8.0 ([2019-05-10](https://github.com/cwtickle/danoniplus/releases/tag/v4.8.0))
- ⭐️ 11key譜面を11Lkeyとしてプレイできるモードを追加 ( PR [#282](https://github.com/cwtickle/danoniplus/pull/282) , Issue [#281](https://github.com/cwtickle/danoniplus/pull/281) 関連 )  
- ⭐️ 別キープレイを許可するかどうかのフラグ（譜面ヘッダー）を追加 ( PR [#282](https://github.com/cwtickle/danoniplus/pull/282) ) 
- ⭐️ 11key, 11Lkeyのキーコンパターンの見直し（おにぎりが上段（5key側）に来るパターンを削除）( PR [#282](https://github.com/cwtickle/danoniplus/pull/282) )
- 🐞 独自キー(keyExtraList)を指定した作品で、複数譜面時に譜面選択できない問題を修正 <- :boom: [**v4.7.0**](Changelog-v4.html#v470-2019-05-05)
 
## v4.7.0 ([2019-05-05](https://github.com/cwtickle/danoniplus/releases/tag/v4.7.0))
- ⭐️ タイトルモーション(backtitle_data)において、キーワード指定によりループやフレームジャンプが行えるように変更 ( PR [#279](https://github.com/cwtickle/danoniplus/pull/279) ) 

## v4.6.2 ([2019-05-04](https://github.com/cwtickle/danoniplus/releases/tag/v4.6.2))
- 🐞 タイトルバック時に速度、ゲージ、リバース設定が初期化されることがある問題を修正 ( PR [#278](https://github.com/cwtickle/danoniplus/pull/278) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03) 

## v4.6.1 ([2019-05-03](https://github.com/cwtickle/danoniplus/releases/tag/v4.6.1))
- 🐞 キーコンフィグ(ローカル保存中データ)を使用する際、Shuffle配列がコピーされない可能性がある問題を修正 ( PR [#277](https://github.com/cwtickle/danoniplus/pull/277) ) <- :boom: [**v4.6.0**](Changelog-v4.html#v460-2019-05-03) 

## v4.6.0 ([2019-05-03](https://github.com/cwtickle/danoniplus/releases/tag/v4.6.0))
- ⭐️ (ドメイン別)キー毎にリバース、キーコンフィグを自動保存する機能を実装 ( PR [#272](https://github.com/cwtickle/danoniplus/pull/272), [#274](https://github.com/cwtickle/danoniplus/pull/274), [#275](https://github.com/cwtickle/danoniplus/pull/275) ) 
- ⭐️ キーコンフィグ画面において、変更・自動保存色を設定 ( PR [#272](https://github.com/cwtickle/danoniplus/pull/272) ) 
- ⭐️ ローカルストレージ保存有無ボタンの追加 ( PR [#274](https://github.com/cwtickle/danoniplus/pull/274) )

## v4.4.1 ([2019-05-02](https://github.com/cwtickle/danoniplus/releases/tag/v4.4.1))
- 🐞 Volumeのカーソル位置をLocalStorageから読み込んだ値に合わせるように修正 ( PR [#270](https://github.com/cwtickle/danoniplus/pull/270) ) <- :boom: [**v4.1.0**](Changelog-v4.html#v410-2019-04-29)
- 🐞 startFrameがundefined以外でかつ、未指定の場合にエラーとなる問題を修正 ( PR [#271](https://github.com/cwtickle/danoniplus/pull/271) ) <- :boom: [**v3.13.1**](Changelog-v3.html#v3131-2019-04-21)

## v4.4.0 ([2019-05-01](https://github.com/cwtickle/danoniplus/releases/tag/v4.4.0))
- ⭐️ タイトル画面に対して背景表示をつける機能 (backtitle_data) を追加 ( PR [#267](https://github.com/cwtickle/danoniplus/pull/267) ) 
- ⭐️ ローカルストレージを削除(初期化)するボタンを追加 ( PR [#268](https://github.com/cwtickle/danoniplus/pull/268) )

## v4.3.2 ([2019-05-01](https://github.com/cwtickle/danoniplus/releases/tag/v4.3.2))
- 🐞 スコア算出方法を独自に決めている場合、ハイスコアの差分が正しく反映されない問題を修正 ( PR [#265](https://github.com/cwtickle/danoniplus/pull/265) ) <- :boom: [**v4.3.0**](Changelog-v4.html#v430-2019-04-30)
- 🐞 ライフの初期値が設定の方法により異なることがある問題を修正 ( PR [#265](https://github.com/cwtickle/danoniplus/pull/265) ) <- :boom: [**v4.3.0**](Changelog-v4.html#v430-2019-04-30)

## v4.3.1 ([2019-05-01](https://github.com/cwtickle/danoniplus/releases/tag/v4.3.1))
- 🐞 ハイスコアの初期化忘れを修正 ( PR [#263](https://github.com/cwtickle/danoniplus/pull/263) ) <- :boom: [**v4.3.0**](Changelog-v4.html#v430-2019-04-30)

## v4.3.0 ([2019-04-30](https://github.com/cwtickle/danoniplus/releases/tag/v4.3.0))
- ⭐️ ハイスコア機能の実装 ( PR [#261](https://github.com/cwtickle/danoniplus/pull/261), Issue [#205](https://github.com/cwtickle/danoniplus/pull/205) )

## v4.2.1 ([2019-04-30](https://github.com/cwtickle/danoniplus/releases/tag/v4.2.1))
- 🐞 マスク表示(mask_data)で、背景表示(back_data)より深度が大きいものを指定した場合、プレイ時に止まる問題を修正 ( PR [#260](https://github.com/cwtickle/danoniplus/pull/260) ) <- :boom: [**v4.2.0**](Changelog-v4.html#v420-2019-04-30)

## v4.2.0 ([2019-04-30](https://github.com/cwtickle/danoniplus/releases/tag/v4.2.0))
- ⭐️ 画面全体にマスクを設定するためのデータ(mask_data)を実装 ( PR [#258](https://github.com/cwtickle/danoniplus/pull/258) ) 

## v4.1.1 ([2019-04-29](https://github.com/cwtickle/danoniplus/releases/tag/v4.1.1))
- 🐞 Display画面からプレイ開始できない問題を修正 ( PR [#257](https://github.com/cwtickle/danoniplus/pull/257) ) <- :boom: [**v4.0.0**](Changelog-v4.html#v400-2019-04-25) 

## v4.1.0 ([2019-04-29](https://github.com/cwtickle/danoniplus/releases/tag/v4.1.0))
- ⭐️ ローカルストレージ(作品別)に「Adjustment」「Volume」を追加 ( PR [#255](https://github.com/cwtickle/danoniplus/pull/255), Issue [#205](https://github.com/cwtickle/danoniplus/pull/205) )

## v4.0.1 ([2019-04-27](https://github.com/cwtickle/danoniplus/releases/tag/v4.0.1))
- 🛠️ back_dataでX/Y座標の整数値制限を緩和（小数が使えるように）( PR [#254](https://github.com/cwtickle/danoniplus/pull/254) ) 
- 🐞 back_dataでOpacityが機能していない問題を修正 ( PR [#254](https://github.com/cwtickle/danoniplus/pull/254) ) <- :boom: [**v0.65.x**](Changelog-v0.html#v065x-2018-11-16)

## v4.0.0 ([2019-04-25](https://github.com/cwtickle/danoniplus/releases/tag/v4.0.0))
- ⭐️ 譜面別の複数曲読込に対応 ( PR [#252](https://github.com/cwtickle/danoniplus/pull/252) )  
- ⭐️ 譜面別に曲名を複数表示できるように変更 ( PR [#252](https://github.com/cwtickle/danoniplus/pull/252) ) 

[**<- v5**](Changelog-v5.html) | **v4** | [**v3 ->**](Changelog-v3.html)
