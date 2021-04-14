⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

[**<- v18**](Changelog-v18.html) | **v17** | [**v16 ->**](Changelog-v16.html)

## [Warning] 更新終了後の不具合情報
- [更新を終了したバージョンの不具合情報#v17](DeprecatedVersionBugs.html#v17) を参照

## v17.5.9 ([2021-02-12](https://github.com/cwtickle/danoniplus/releases/tag/v17.5.9))
- 🐞 createCss2Button関数にて右クリック拡張ができない場合がある問題を修正 ( PR [#970](https://github.com/cwtickle/danoniplus/pull/970) ) <- :boom: [**v17.5.0**](Changelog-v17.html#v1750-2020-10-17)
- 🐞 changeStyle関数のコードミスを修正 ( PR [#958](https://github.com/cwtickle/danoniplus/pull/958) ) <- :boom: [**v17.1.0**](Changelog-v17.html#v1710-2020-09-28)

## v17.5.8 ([2021-01-05](https://github.com/cwtickle/danoniplus/releases/tag/v17.5.8))
- 🐞 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、通常矢印の判定が優先されてしまう事象を修正 ( PR [#929](https://github.com/cwtickle/danoniplus/pull/929), [#930](https://github.com/cwtickle/danoniplus/pull/930), [#932](https://github.com/cwtickle/danoniplus/pull/932) ) <- :boom: **initial**

## v17.5.7 ([2020-12-30](https://github.com/cwtickle/danoniplus/releases/tag/v17.5.7))
- 🐞 一部のキーを押すと全押し状態になる問題を修正 ( PR [#924](https://github.com/cwtickle/danoniplus/pull/924) ) <- :boom: [**v16.0.0**](Changelog-v16.html#v1600-2020-08-06) 

## v17.5.6 ([2020-12-25](https://github.com/cwtickle/danoniplus/releases/tag/v17.5.6))
- 🐞 カスタムjs, スキンjsを二重読込している問題を修正 ( PR [#917](https://github.com/cwtickle/danoniplus/pull/917) ) <- :boom: [**v7.7.0**](Changelog-v7.html#v770-2019-08-25)
- 🐞 楽曲・画像読込チェックの待ち時間誤りを修正 ( PR [#915](https://github.com/cwtickle/danoniplus/pull/915) ) <- :boom: [**v10.1.1**](Changelog-v10.html#v1011-2019-11-11)

## v17.5.5 ([2020-12-21](https://github.com/cwtickle/danoniplus/releases/tag/v17.5.5))
- 🐞 曲終了直後にリトライキーを押すとALL0のリザルトが表示される問題を修正 ( PR [#908](https://github.com/cwtickle/danoniplus/pull/908) ) <- :boom: [**v0.67.x**](Changelog-v0.html#v067x-2018-11-17) 

## v17.5.4 ([2020-11-23](https://github.com/cwtickle/danoniplus/releases/tag/v17.5.4))
- 🐞 Display:Colorのボタンが無効化されていた場合にColorTypeの挙動により、Display:Colorの切り替えができてしまう問題を修正 ( PR [#892](https://github.com/cwtickle/danoniplus/pull/892) ) <- :boom: [**v14.0.2**](Changelog-v14.html#v1402-2020-04-29) 

## v17.5.3 ([2020-11-02](https://github.com/cwtickle/danoniplus/releases/tag/v17.5.3))
- 🐞 速度データ(speed_change)が空の場合、データがあると判断されてしまいspeed_changeが優先されてしまう問題を修正 ( PR [#884](https://github.com/cwtickle/danoniplus/pull/884) ) <- :boom: [**v8.0.0**](Changelog-v8.html#v800-2019-09-08) 

## v17.5.2 ([2020-10-31](https://github.com/cwtickle/danoniplus/releases/tag/v17.5.2))
- 🐞 複数曲搭載時に曲名の2段目がundefinedになる問題を修正 ( PR [#882](https://github.com/cwtickle/danoniplus/pull/882) ) <- :boom: [**v17.3.0**](Changelog-v17.html#v1730-2020-10-08)

----

## v17.5.1 ([2020-10-24](https://github.com/cwtickle/danoniplus/releases/tag/v17.5.1))
- 🐞 カンマのエスケープ文字の変換間違いを修正 ( Gitter [2020-10-21](https://gitter.im/danonicw/community?at=5f903fc0631a250ab2823b73), PR [#877](https://github.com/cwtickle/danoniplus/pull/877) ) <- :boom: [**v17.4.2**](Changelog-v17.html#v1742-2020-10-11)

## v17.5.0 ([2020-10-17](https://github.com/cwtickle/danoniplus/releases/tag/v17.5.0))
- ⭐ ボタン作成処理に右クリック処理、イベント引数を追加 ( PR [#871](https://github.com/cwtickle/danoniplus/pull/871) )
- 🛠️ 複数子要素を親要素へ追加する処理を集約 ( PR [#871](https://github.com/cwtickle/danoniplus/pull/871) )
- 🛠️ 長い名前の関数を全体的に見直し、その他コード整理 ( PR [#872](https://github.com/cwtickle/danoniplus/pull/872), [#873](https://github.com/cwtickle/danoniplus/pull/873) )

## v17.4.3 ([2020-10-12](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.3))
- 🐞 矢印塗りつぶし有、ステップゾーンをOFFにした場合に矢印塗りつぶし部分が残る問題を修正 ( PR [#866](https://github.com/cwtickle/danoniplus/pull/866), [#868](https://github.com/cwtickle/danoniplus/pull/868) ) <- :boom: [**v5.12.0**](Changelog-v5.html#v5120-2019-06-14)
- 🐞 DataSaveをOFFにしたとき、Reverseのstyleが反映されない問題を修正 ( PR [#867](https://github.com/cwtickle/danoniplus/pull/867) ) <- :boom: [**v17.0.1**](Changelog-v17.html#v1701-2020-09-27)

## v17.4.2 ([2020-10-11](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.2))
- 🛠️ コードの見直し ( PR [#861](https://github.com/cwtickle/danoniplus/pull/861) )
- 🐞 結果画面のショボーンのラベルID誤りを修正 ( PR [#860](https://github.com/cwtickle/danoniplus/pull/860) ) <- :boom: [**v17.2.0**](Changelog-v17.html#v1720-2020-10-03)
- 🐞 最後の矢印を取り忘れてクリアするとundefinedになる問題を修正 ( PR [#862](https://github.com/cwtickle/danoniplus/pull/862) ) <- :boom: [**v17.0.1**](Changelog-v17.html#v1701-2020-09-27)
- 🐞 strictモード有効化に伴い、初期化されていない変数を修正 ( PR [#864](https://github.com/cwtickle/danoniplus/pull/864) ) <- :boom: [**v17.4.0**](Changelog-v17.html#v1740-2020-10-09)

## v17.4.0 ([2020-10-09](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.0))
- 🛠️ strictモードを有効化 ( PR [#855](https://github.com/cwtickle/danoniplus/pull/855) )
- 🐞 strictモード有効化に伴い、初期化されていない変数を見直し ( PR [#856](https://github.com/cwtickle/danoniplus/pull/856) ) <- :boom: [**v17.4.0**](Changelog-v17.html#v1740-2020-10-09) <- [**v12.0.0**](Changelog-v12.html#v1200-2020-02-09)
- 🐞 カスタムゲージで一部未指定がある場合にボーダー値が反映されない問題を修正 ( PR [#857](https://github.com/cwtickle/danoniplus/pull/857) ) <- :boom: [**v17.3.0**](Changelog-v17.html#v1730-2020-10-08)
- 🐞 ツール値出力時、時間表示がおかしくなることがある問題を修正 ( PR [#858](https://github.com/cwtickle/danoniplus/pull/858) ) <- :boom: [**v12.0.0**](Changelog-v12.html#v1200-2020-02-09) <- [**v2.0.0**](Changelog-v2.html#v200-2019-01-18)

## v17.3.0 ([2020-10-08](https://github.com/cwtickle/danoniplus/releases/tag/v17.3.0))
- ⭐ タイトル文字のフォントと位置について2行目指定ができるように変更 ( PR [#851](https://github.com/cwtickle/danoniplus/pull/851) )
- 🛠️ レベル計算、階層スプライト、ゲージ設定周りのコード整理 ( PR [#852](https://github.com/cwtickle/danoniplus/pull/852), [#853](https://github.com/cwtickle/danoniplus/pull/853) )
- 🐞 tuningのみ指定があった場合に制作者リンクが出ない問題を修正 ( PR [#850](https://github.com/cwtickle/danoniplus/pull/850) ) <- :boom: [**v3.0.0**](Changelog-v3.html#v300-2019-02-25)

## v17.2.0 ([2020-10-03](https://github.com/cwtickle/danoniplus/releases/tag/v17.2.0))
- 🛠️ 制作者、アーティスト名リンクが未指定の場合、リンクを実行させないよう修正 ( PR [#846](https://github.com/cwtickle/danoniplus/pull/846) )
- 🛠️ HTMLを埋め込まない箇所を`Node.textContent`の記述に置き換え ( PR [#847](https://github.com/cwtickle/danoniplus/pull/847) )
- 🛠️ その他コード整理、CodeQLの適用 ( PR [#844](https://github.com/cwtickle/danoniplus/pull/844), [#848](https://github.com/cwtickle/danoniplus/pull/848) )

## v17.1.0 ([2020-09-28](https://github.com/cwtickle/danoniplus/releases/tag/v17.1.0))
- ⭐ ボタンクリック後の処理に対して処理を追加できる機能を実装 ( PR [#841](https://github.com/cwtickle/danoniplus/pull/841) )
- ⭐ ボタン及びラベルのスタイル一括変更関数を実装 ( PR [#841](https://github.com/cwtickle/danoniplus/pull/841) )
- 🐞 フェードイン時、フリーズアローの計算処理で止まる問題を修正 ( Gitter [2020-09-27](https://gitter.im/danonicw/community?at=5f7096740b5f3873c9f74f7e), PR [#842](https://github.com/cwtickle/danoniplus/pull/842) ) <- :boom: [**v17.0.1**](Changelog-v17.html#v1701-2020-09-27)

## v17.0.1 ([2020-09-27](https://github.com/cwtickle/danoniplus/releases/tag/v17.0.1))
- 🛠️ ラベル・ボタン・色付きオブジェクト作成用関数を作り直し ( Issue [#833](https://github.com/cwtickle/danoniplus/pull/833), PR [#834](https://github.com/cwtickle/danoniplus/pull/834) )
- 🛠️ コードの整理 ( PR [#835](https://github.com/cwtickle/danoniplus/pull/835), [#837](https://github.com/cwtickle/danoniplus/pull/837) )
- 🐞 user-selectがSafariブラウザのみ動作しない問題を修正 ( PR [#832](https://github.com/cwtickle/danoniplus/pull/832) ) <- :boom: [**v16.4.0**](Changelog-v16.html#v1640-2020-09-22)

[**<- v18**](Changelog-v18.html) | **v17** | [**v16 ->**](Changelog-v16.html)
