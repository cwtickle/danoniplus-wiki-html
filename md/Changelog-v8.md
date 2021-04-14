⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

[**<- v9**](Changelog-v9.html) | **v8** | [**v7 ->**](Changelog-v7.html)

## [Warning] 更新終了後の不具合情報
- [更新を終了したバージョンの不具合情報#v8](DeprecatedVersionBugs.html#v8) を参照

## v8.7.10 ([2019-12-14](https://github.com/cwtickle/danoniplus/releases/tag/v8.7.10))
- 🛠️ Localhost時にフレーム数を表示するように変更 ( PR [#561](https://github.com/cwtickle/danoniplus/pull/561) )
- 🛠️ ラベルのID重複を解消 ( PR [#545](https://github.com/cwtickle/danoniplus/pull/545), [#546](https://github.com/cwtickle/danoniplus/pull/546), [#562](https://github.com/cwtickle/danoniplus/pull/562) )
- 🛠️ fileでも起動可能なようにcrossorigin属性の付加条件を変更 ( PR [#564](https://github.com/cwtickle/danoniplus/pull/564) )

## v8.7.9 ([2019-11-11](https://github.com/cwtickle/danoniplus/releases/tag/v8.7.9))
- 🐞 MacOS, iOS (Safari)においてWeb Audio APIが動作しない問題を修正 ( PR [#523](https://github.com/cwtickle/danoniplus/pull/523), [#525](https://github.com/cwtickle/danoniplus/pull/525), [#527](https://github.com/cwtickle/danoniplus/pull/527) ) <- :boom: **initial**

## v8.7.7 ([2019-10-14](https://github.com/cwtickle/danoniplus/releases/tag/v8.7.7))
- 🐞 背景・マスクモーションでオールクリアが使用できない問題を修正 ( PR [#488](https://github.com/cwtickle/danoniplus/pull/488) ) <- :boom: [**v7.7.0**](Changelog-v7.html#v770-2019-08-25)

## v8.7.6 ([2019-10-13](https://github.com/cwtickle/danoniplus/releases/tag/v8.7.6))
- 🐞 ダミーIDの譜面ヘッダー誤りを修正 ( PR [#483](https://github.com/cwtickle/danoniplus/pull/483) ) <- :boom: [**v6.0.0**](Changelog-v6.html#v600-2019-06-22)
- 🐞 ダミー矢印/フリーズアロー用カスタム関数が定義できない問題を修正 ( PR [#485](https://github.com/cwtickle/danoniplus/pull/485) ) <- :boom: [**v6.1.0**](Changelog-v6.html#v610-2019-06-22)

## v8.7.4 ([2019-10-12](https://github.com/cwtickle/danoniplus/releases/tag/v8.7.4))
- 🐞 低速時かつフリーズアロー開始判定時にPF判定が早まる問題を修正 ( PR [#481](https://github.com/cwtickle/danoniplus/pull/481) ) <- :boom: [**v5.7.0**](Changelog-v5.html#v570-2019-06-01)

----

## v8.7.3 ([2019-10-08](https://github.com/cwtickle/danoniplus/releases/tag/v8.7.3))
- 🐞 速度変化が同一フレームにあると正常に動作しなくなる不具合を修正 ( PR [#477](https://github.com/cwtickle/danoniplus/pull/477) ) <- :boom: **initial**

## v8.7.2 ([2019-10-06](https://github.com/cwtickle/danoniplus/releases/tag/v8.7.2))
- 🐞 エスケープ文字の適用順序誤りを修正 ( PR [#472](https://github.com/cwtickle/danoniplus/pull/472), [#473](https://github.com/cwtickle/danoniplus/pull/473) ) <- :boom: [**v0.66.x**](Changelog-v0.html#v066x-2018-11-16)

## v8.7.1 ([2019-10-05](https://github.com/cwtickle/danoniplus/releases/tag/v8.7.1))
- 🐞 FPSが小数の場合にタイマーが作動しない問題を修正 ( PR [#470](https://github.com/cwtickle/danoniplus/pull/470) ) <- :boom: [**v8.6.3**](Changelog-v8.html#v863-2019-10-02)

## v8.7.0 ([2019-10-03](https://github.com/cwtickle/danoniplus/releases/tag/v8.7.0))
- ⭐️ ローカルストレージ（作品別）のキーからscoreIdを除去 ( PR [#467](https://github.com/cwtickle/danoniplus/pull/467) )
- 🛠️ リザルトコピーのURLからscoreIdを除去 ( PR [#468](https://github.com/cwtickle/danoniplus/pull/468) )

## v8.6.3 ([2019-10-02](https://github.com/cwtickle/danoniplus/releases/tag/v8.6.3))
- 🛠️ 最初の読込時のオブジェクト削除をカット、ローディング文字のみ削除するように変更 ( PR [#464](https://github.com/cwtickle/danoniplus/pull/464) )
- 🛠️ ローカルmp3の読込失敗時のエラーメッセージを追加 ( PR [#464](https://github.com/cwtickle/danoniplus/pull/464) )
- 🛠️ FPS値の変数化に対応 ( PR [#465](https://github.com/cwtickle/danoniplus/pull/465) )

## v8.6.2 ([2019-10-01](https://github.com/cwtickle/danoniplus/releases/tag/v8.6.2))
- 🐞 譜面変更時にゲージ設定が初期値に設定されてしまう問題を修正 ( PR [#462](https://github.com/cwtickle/danoniplus/pull/462) ) <- :boom: [**v8.5.2**](Changelog-v8.html#v852-2019-09-29)

## v8.6.1 ([2019-09-30](https://github.com/cwtickle/danoniplus/releases/tag/v8.6.1))
- 🛠️ ファイル読込に失敗した場合のメッセージを追加 ( Issue [#458](https://github.com/cwtickle/danoniplus/pull/458), PR [#459](https://github.com/cwtickle/danoniplus/pull/459), [#460](https://github.com/cwtickle/danoniplus/pull/460) )
- 🐞 エラーウィンドウが表示されない問題を修正 ( PR [#459](https://github.com/cwtickle/danoniplus/pull/459) ) <- :boom: [**v2.6.0**](Changelog-v2.html#v260-2019-02-10)

## v8.6.0 ([2019-09-29](https://github.com/cwtickle/danoniplus/releases/tag/v8.6.0))
- 🛠️ コード整理（本来booleanで定義すべき変数の型変更、定数化）( PR [#455](https://github.com/cwtickle/danoniplus/pull/455) )

## v8.5.2 ([2019-09-29](https://github.com/cwtickle/danoniplus/releases/tag/v8.5.2))
- 🛠️ ゲージ設定周りのコード整理 ( PR [#453](https://github.com/cwtickle/danoniplus/pull/453) )
- 🛠️ サンプルHTMLの見直し（HTML5の記述に対応していないブラウザに警告表示）( PR [#452](https://github.com/cwtickle/danoniplus/pull/452) )
- 🐞 クエリで譜面番号が指定されていた場合に、初期速度が1譜面目の設定になる問題を修正 ( PR [#453](https://github.com/cwtickle/danoniplus/pull/453) ) <- :boom: [**v7.3.0**](Changelog-v7.html#v730-2019-07-20)

## v8.5.1 ([2019-09-28](https://github.com/cwtickle/danoniplus/releases/tag/v8.5.1))
- 🛠️ 外部の譜面ファイル内の譜面データを一時クリアする条件を「譜面ファイル分割時」「譜面番号固定時」に限定するよう修正 ( PR [#450](https://github.com/cwtickle/danoniplus/pull/450) )

## v8.5.0 ([2019-09-28](https://github.com/cwtickle/danoniplus/releases/tag/v8.5.0))
- ⭐️ 譜面毎のファイル分割に対応 ( Issue [#446](https://github.com/cwtickle/danoniplus/pull/446), PR [#447](https://github.com/cwtickle/danoniplus/pull/447), [#448](https://github.com/cwtickle/danoniplus/pull/448) )
- ⭐️ 譜面をファイル分割した場合に、譜面番号を常時固定するかどうかの設定を追加 ( PR [#447](https://github.com/cwtickle/danoniplus/pull/447) )
- 🛠️ 譜面読込時に前回読込を行ったデータをクリアするよう変更 ( PR [#447](https://github.com/cwtickle/danoniplus/pull/447) )
- 🛠️ 画像のプリロードを二重に行わないよう変更 ( PR [#447](https://github.com/cwtickle/danoniplus/pull/447) )
- 🐞 クエリで譜面番号が指定されていた場合に、キー数が異なることがある問題を修正 ( PR [#447](https://github.com/cwtickle/danoniplus/pull/447) ) <- :boom: [**v7.7.0**](Changelog-v7.html#v770-2019-08-25)

## v8.4.0 ([2019-09-26](https://github.com/cwtickle/danoniplus/releases/tag/v8.4.0))
- ⭐️ 譜面変更用のセレクターについて、キー別フィルターを追加 ( PR [#444](https://github.com/cwtickle/danoniplus/pull/444) )

## v8.3.0 ([2019-09-26](https://github.com/cwtickle/danoniplus/releases/tag/v8.3.0))
- ⭐️ 譜面変更用のセレクターを実装 ( PR [#441](https://github.com/cwtickle/danoniplus/pull/441) )
- 🛠️ 曲中ショートカット移動後のkeyUpイベントを無効化 ( PR [#442](https://github.com/cwtickle/danoniplus/pull/442) )

## v8.2.0 ([2019-09-24](https://github.com/cwtickle/danoniplus/releases/tag/v8.2.0))
- ⭐️ 曲名（複数行）を1行で表示する場合に間を空白で埋めない（全角で埋める）設定を追加 ( PR [#437](https://github.com/cwtickle/danoniplus/pull/437) )
- ⭐️ 制作者表示の複数化に対応（リザルトコピー）( PR [#438](https://github.com/cwtickle/danoniplus/pull/438) )
- ⭐️ 設定・結果画面への制作者名表示有無設定を追加 ( PR [#438](https://github.com/cwtickle/danoniplus/pull/438) )
- ⭐️ 譜面別データ(LocalStorage)に制作者名を付加できるように変更 ( PR [#439](https://github.com/cwtickle/danoniplus/pull/439) )

## v8.1.0 ([2019-09-23](https://github.com/cwtickle/danoniplus/releases/tag/v8.1.0))
- 🛠️ タイトル画面の「Dancing☆Onigiri」の文字をbacktitle_dataの前面に来るように変更 ( PR [#435](https://github.com/cwtickle/danoniplus/pull/435) )

## v8.0.4 ([2019-09-23](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.4))
- 🐞 ロード画面でEnterを押すと複数回ロードが発生する問題を修正 ( PR [#432](https://github.com/cwtickle/danoniplus/pull/432) ) <- :boom: **initial**
- 🐞 メイン画面で曲中リトライキーを連打した場合に譜面がずれることがある問題を修正 ( PR [#433](https://github.com/cwtickle/danoniplus/pull/433) ) <- :boom: **initial**

## v8.0.3 ([2019-09-22](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.3))
- 🐞 fadeFrameが譜面数に到達しない場合にプレイが止まる問題を修正 ( PR [#430](https://github.com/cwtickle/danoniplus/pull/430) ) <- :boom: [**v8.0.0**](Changelog-v8.html#v800-2019-09-08)

## v8.0.2 ([2019-09-16](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.2))
- 🐞 ゲームオーバー時の200ミリ秒遅延により、ハイスコア表示がおかしくなることがある問題を修正 ( PR [#428](https://github.com/cwtickle/danoniplus/pull/428) ) <- :boom: **initial**

## v8.0.1 ([2019-09-15](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.1))
- 🐞 速度変化が補正込みで負のフレームにあるときの不具合を修正 ( PR [#426](https://github.com/cwtickle/danoniplus/pull/426) ) <- :boom: **initial**

## v8.0.0 ([2019-09-08](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.0))
- ⭐️ タイトル／リザルトモーションの音楽同期対応 ( PR [#419](https://github.com/cwtickle/danoniplus/pull/419), [#423](https://github.com/cwtickle/danoniplus/pull/423) )
- ⭐️ リザルトモーションを譜面別に作成できるように対応 ( PR [#419](https://github.com/cwtickle/danoniplus/pull/419) )
- ⭐️ 楽曲のフェードアウト長を指定できるように変更 ( Issue [#413](https://github.com/cwtickle/danoniplus/pull/413), PR [#420](https://github.com/cwtickle/danoniplus/pull/420) )
- ⭐️ 速度変化表記 (speed_data/change)の統一 ( Issue [#416](https://github.com/cwtickle/danoniplus/pull/416), PR [#421](https://github.com/cwtickle/danoniplus/pull/421) )
- ⭐️ ステップゾーン(下)位置を変更できる設定を追加 ( PR [#424](https://github.com/cwtickle/danoniplus/pull/424) )

[**<- v9**](Changelog-v9.html) | **v8** | [**v7 ->**](Changelog-v7.html)
