⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

[**<- v8**](Changelog-v8.html) | **v7** | [**v6 ->**](Changelog-v6.html)

## [Warning] 更新終了後の不具合情報
- [更新を終了したバージョンの不具合情報#v7](DeprecatedVersionBugs.html#v7) を参照

## v7.9.13 ([2019-10-14](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.13))
- 🐞 背景・マスクモーションでオールクリアが使用できない問題を修正 ( PR [#488](https://github.com/cwtickle/danoniplus/pull/488) ) <- :boom: [**v7.7.0**](Changelog-v7.html#v770-2019-08-25)

## v7.9.12 ([2019-10-13](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.12))
- 🐞 ダミーIDの譜面ヘッダー誤りを修正 ( PR [#483](https://github.com/cwtickle/danoniplus/pull/483) ) <- :boom: [**v6.0.0**](Changelog-v6.html#v600-2019-06-22)
- 🐞 ダミー矢印/フリーズアロー用カスタム関数が定義できない問題を修正 ( PR [#485](https://github.com/cwtickle/danoniplus/pull/485) ) <- :boom: [**v6.1.0**](Changelog-v6.html#v610-2019-06-22)

## v7.9.10 ([2019-10-12](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.10))
- 🐞 低速時かつフリーズアロー開始判定時にPF判定が早まる問題を修正 ( PR [#481](https://github.com/cwtickle/danoniplus/pull/481) ) <- :boom: [**v5.7.0**](Changelog-v5.html#v570-2019-06-01)

## v7.9.9 ([2019-10-08](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.9))
- 🐞 速度変化が同一フレームにあると正常に動作しなくなる不具合を修正 ( PR [#477](https://github.com/cwtickle/danoniplus/pull/477) ) <- :boom: **initial**

## v7.9.8 ([2019-10-06](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.8))
- 🐞 エスケープ文字の適用順序誤りを修正 ( PR [#472](https://github.com/cwtickle/danoniplus/pull/472), [#473](https://github.com/cwtickle/danoniplus/pull/473) ) <- :boom: [**v0.66.x**](Changelog-v0.html#v066x-2018-11-16)

## v7.9.7 ([2019-09-30](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.7))
- 🐞 エラーウィンドウが表示されない問題を修正 ( PR [#459](https://github.com/cwtickle/danoniplus/pull/459) ) <- :boom: [**v2.6.0**](Changelog-v2.html#v260-2019-02-10)

## v7.9.6 ([2019-09-29](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.6))
- 🐞 クエリで譜面番号が指定されていた場合に、初期速度が1譜面目の設定になる問題を修正 ( PR [#453](https://github.com/cwtickle/danoniplus/pull/453) ) <- :boom: [**v7.3.0**](Changelog-v7.html#v730-2019-07-20)

## v7.9.5 ([2019-09-28](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.5))
- 🛠️ 画像のプリロードを二重に行わないよう変更 ( PR [#447](https://github.com/cwtickle/danoniplus/pull/447) )
- 🐞 クエリで譜面番号が指定されていた場合に、キー数が異なることがある問題を修正 ( PR [#447](https://github.com/cwtickle/danoniplus/pull/447) ) <- :boom: [**v7.7.0**](Changelog-v7.html#v770-2019-08-25)

## v7.9.4 ([2019-09-23](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.4))
- 🐞 ロード画面でEnterを押すと複数回ロードが発生する問題を修正 ( PR [#432](https://github.com/cwtickle/danoniplus/pull/432) ) <- :boom: **initial**
- 🐞 メイン画面で曲中リトライキーを連打した場合に譜面がずれることがある問題を修正 ( PR [#433](https://github.com/cwtickle/danoniplus/pull/433) ) <- :boom: **initial**

## v7.9.3 ([2019-09-16](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.3))
- 🐞 ゲームオーバー時の200ミリ秒遅延により、ハイスコア表示がおかしくなることがある問題を修正 ( PR [#428](https://github.com/cwtickle/danoniplus/pull/428) ) <- :boom: **initial**

## v7.9.2 ([2019-09-15](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.2))
- 🐞 速度変化が補正込みで負のフレームにあるときの不具合を修正 ( PR [#426](https://github.com/cwtickle/danoniplus/pull/426) ) <- :boom: **initial**

----

## v7.9.1 ([2019-09-03](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.1))
- 🛠️ 速度変化においてコメント文を実装 ( PR [#411](https://github.com/cwtickle/danoniplus/pull/411) )
- 🐞 色変化・歌詞表示のコメント行にカンマが入ったときの不具合を修正 ( PR [#411](https://github.com/cwtickle/danoniplus/pull/411) ) <- :boom: [**v7.9.0**](Changelog-v7.html#v790-2019-09-02)

## v7.9.0 ([2019-09-02](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.0))
- ⭐️ クリア失敗時のリザルトモーションを実装 ( PR [#409](https://github.com/cwtickle/danoniplus/pull/409) )
- ⭐️ 背景・マスクモーション、色変化、歌詞表示でコメント文を実装 ( PR [#408](https://github.com/cwtickle/danoniplus/pull/408) )

## v7.8.2 ([2019-09-01](https://github.com/cwtickle/danoniplus/releases/tag/v7.8.2))
- 🐞 キーコンフィグの別パターンが選択できない問題を修正 ( PR [#406](https://github.com/cwtickle/danoniplus/pull/406) ) <- :boom: [**v7.7.0**](Changelog-v7.html#v770-2019-08-25)

## v7.8.1 ([2019-08-31](https://github.com/cwtickle/danoniplus/releases/tag/v7.8.1))
- 🛠️ 設定画面のAdjustmentによらず、見た目の曲時間を表示するように変更 ( PR [#404](https://github.com/cwtickle/danoniplus/pull/404) )

## v7.8.0 ([2019-08-30](https://github.com/cwtickle/danoniplus/releases/tag/v7.8.0))
- ⭐️ 楽曲の終了判定タイミングを秒単位からフレーム単位に変更 ( PR [#402](https://github.com/cwtickle/danoniplus/pull/402) )
- ⭐️ リザルトモーションをDisplay:Backgroundと連動してON/OFFする仕様に変更 ( PR [#402](https://github.com/cwtickle/danoniplus/pull/402) )
- ⭐️ リザルトモーションを譜面データ同様に、毎回読み直す仕様に変更 ( PR [#402](https://github.com/cwtickle/danoniplus/pull/402) )
- 🛠️ 設定画面で設定したAdjustmentを楽曲終了位置に加算するように変更 ( PR [#402](https://github.com/cwtickle/danoniplus/pull/402) )
- 🛠️ リザルトモーションで0フレームを指定した場合に、結果画面が一瞬表示される事象を修正 ( PR [#402](https://github.com/cwtickle/danoniplus/pull/402) )
- 🛠️ 結果画面のDisplay表示処理の見直し ( PR [#402](https://github.com/cwtickle/danoniplus/pull/402) )

## v7.7.1 ([2019-08-25](https://github.com/cwtickle/danoniplus/releases/tag/v7.7.1))
- 🐞 複数譜面時に2譜面目以降（初期選択譜面以外）が読み込めない問題を修正 ( PR [#400](https://github.com/cwtickle/danoniplus/pull/400) ) <- :boom: [**v7.7.0**](Changelog-v7.html#v770-2019-08-25)

## v7.7.0 ([2019-08-25](https://github.com/cwtickle/danoniplus/releases/tag/v7.7.0))
- ⭐️ 譜面読込画面に入ったときに譜面データを再読込できるように変更 ( PR [#397](https://github.com/cwtickle/danoniplus/pull/397) )
- ⭐️ 歌詞表示・背景/マスクモーションにおいて同一フレームの複数同時描画に対応 ( PR [#398](https://github.com/cwtickle/danoniplus/pull/398) )
- ⭐️ 背景/マスクモーションにおいて、深度に「ALL」を指定することで、全てのオブジェクトを一斉クリアできるように対応 ( PR [#398](https://github.com/cwtickle/danoniplus/pull/398) )

## v7.6.0 ([2019-08-18](https://github.com/cwtickle/danoniplus/releases/tag/v7.6.0))
- ⭐️ タイトル・リザルトモーションのジャンプで確率でジャンプ先を変えられるように変更 ( PR [#393](https://github.com/cwtickle/danoniplus/pull/393), Issue [#392](https://github.com/cwtickle/danoniplus/pull/392) )
- ⭐️ サンプル用HTMLを新規に作成 ( PR [#394](https://github.com/cwtickle/danoniplus/pull/394) )
- 🐞 タイトル・リザルトモーションでループカウンターが機能していない問題を修正 ( PR [#393](https://github.com/cwtickle/danoniplus/pull/393) ) <- :boom: [**v6.3.0**](Changelog-v6.html#v630-2019-06-27)

## v7.5.1 ([2019-08-03](https://github.com/cwtickle/danoniplus/releases/tag/v7.5.1))
- 🛠️ back_data, mask_dataで0フレームが指定された場合、ステップゾーンやライフゲージの表示より早く表示されるように変更 ( PR [#388](https://github.com/cwtickle/danoniplus/pull/388) )
- 🐞 back_data, mask_dataで0フレームが指定された場合に動作しないことがある問題を修正 ( PR [#388](https://github.com/cwtickle/danoniplus/pull/388) ) <- :boom: [**v4.2.0**](Changelog-v4.html#v420-2019-04-30), [**v0.65.x**](Changelog-v0.html#v065x-2018-11-16)

## v7.5.0 ([2019-07-29](https://github.com/cwtickle/danoniplus/releases/tag/v7.5.0))
- ⭐️ 譜面ヘッダー：preloadImages（事前読み込み画像）の複数まとめ記述の実装 ( PR [#386](https://github.com/cwtickle/danoniplus/pull/386) )

## v7.4.0 ([2019-07-21](https://github.com/cwtickle/danoniplus/releases/tag/v7.4.0))
- ⭐️ 初期矢印色・初期フリーズアロー色について、カラーコードの左パディング機能を実装 ( PR [#383](https://github.com/cwtickle/danoniplus/pull/383) )
- ⭐️ F5キーのキーブロックを解除 ( PR [#383](https://github.com/cwtickle/danoniplus/pull/383) )
- ⭐️ リザルト画面へ移行後に楽曲フェードアウトできるように変更 ( PR [#384](https://github.com/cwtickle/danoniplus/pull/384) )
- 🐞 リザルト画面で、フェードアウト中にTitleBack/Retryするとフェードアウト状態が引き継がれてしまう問題を修正 ( PR [#384](https://github.com/cwtickle/danoniplus/pull/384) ) <- :boom: [**v0.68.x**](Changelog-v0.html#v068x-2018-11-17)

## v7.3.1 ([2019-07-21](https://github.com/cwtickle/danoniplus/releases/tag/v7.3.1))
- 🐞 Display画面へ遷移したときにボタンアニメーションが解除されない問題を修正 ( PR [#381](https://github.com/cwtickle/danoniplus/pull/381) ) <- :boom: [**v7.3.0**](Changelog-v7.html#v730-2019-07-20)

## v7.3.0 ([2019-07-20](https://github.com/cwtickle/danoniplus/releases/tag/v7.3.0))
- ⭐️ キーコンフィグ画面のボタン配置を見直し ( PR [#377](https://github.com/cwtickle/danoniplus/pull/377) )
  - キーコンフィグ画面におけるボタンアニメーションを廃止
  - キーコンフィグパターン変更について逆回しボタンを追加
  - 現在選択しているキーコンフィグパターンと、別キーモード状態を表示するように変更
- ⭐️ デフォルトで選択状態にする譜面をURLで指定できる機能を実装 ( PR [#378](https://github.com/cwtickle/danoniplus/pull/378) )
- ⭐️ 色変化の過去バージョン互換対応 ( PR [#379](https://github.com/cwtickle/danoniplus/pull/379) )
- 🐞 特殊キーを複数譜＆複数キー指定していた場合で、片方のキーのみキーコンフィグ設定を保存していた場合に、もう片方のキーのキーコンフィグが表示できないことがある問題を修正 ( PR [#377](https://github.com/cwtickle/danoniplus/pull/377) ) <- :boom: [**v6.6.0**](Changelog-v6.html#v660-2019-07-08)

## v7.2.0 ([2019-07-15](https://github.com/cwtickle/danoniplus/releases/tag/v7.2.0))
- ⭐️ 画面遷移用ボタンにアニメーションを導入 ( PR [#375](https://github.com/cwtickle/danoniplus/pull/375) )
- ⭐️ Escキーをキーコンフィグ割り当てキーから除外 ( PR [#375](https://github.com/cwtickle/danoniplus/pull/375) )

## v7.1.1 ([2019-07-12](https://github.com/cwtickle/danoniplus/releases/tag/v7.1.1))
- 🐞 矢印・フリーズアローのCSSモーションがデフォルトOFFになっていた問題を修正 ( PR [#374](https://github.com/cwtickle/danoniplus/pull/374) ) <- :boom: [**v7.1.0**](Changelog-v7.html#v710-2019-07-12)

## v7.1.0 ([2019-07-12](https://github.com/cwtickle/danoniplus/releases/tag/v7.1.0))
- ⭐️ フリーズアローヒット時の個別色変化のタイミングを変更 ( PR [#369](https://github.com/cwtickle/danoniplus/pull/369) , Issue [#354](https://github.com/cwtickle/danoniplus/pull/354) )
- ⭐️ ボタン色の見直し 及び ボタン色を個別指定できるように変更 ( PR [#370](https://github.com/cwtickle/danoniplus/pull/370) )
- ⭐️ 矢印・フリーズアローのCSSモーションのON/OFFボタンを追加 ( PR [#371](https://github.com/cwtickle/danoniplus/pull/371) )
- ⭐️ 歌詞表示（word_data）の3番目の要素を省略できるように変更（4番目未指定の場合）( PR [#372](https://github.com/cwtickle/danoniplus/pull/372) )

## v7.0.0 ([2019-07-08](https://github.com/cwtickle/danoniplus/releases/tag/v7.0.0))
- ⭐️ 矢印・フリーズアローにCSSモーション機能を実装 ( PR [#367](https://github.com/cwtickle/danoniplus/pull/367) )
- ⭐️ キーブロック対象にEscapeキーを追加 ( PR [#368](https://github.com/cwtickle/danoniplus/pull/368) )

[**<- v8**](Changelog-v8.html) | **v7** | [**v6 ->**](Changelog-v6.html)
