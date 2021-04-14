⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

[**<- v17**](Changelog-v17.html) | **v16** | [**v15 ->**](Changelog-v15.html)

## [Warning] 更新終了後の不具合情報
- [更新を終了したバージョンの不具合情報#v16](DeprecatedVersionBugs.html#v16) を参照

## v16.4.10 ([2021-01-05](https://github.com/cwtickle/danoniplus/releases/tag/v16.4.10))
- 🐞 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、
通常矢印の判定が優先されてしまう事象を修正 ( PR [#929](https://github.com/cwtickle/danoniplus/pull/929), [#930](https://github.com/cwtickle/danoniplus/pull/930), [#932](https://github.com/cwtickle/danoniplus/pull/932) ) <- :boom: **initial**

## v16.4.9 ([2020-12-30](https://github.com/cwtickle/danoniplus/releases/tag/v16.4.9))
- 🐞 一部のキーを押すと全押し状態になる問題を修正 ( PR [#924](https://github.com/cwtickle/danoniplus/pull/924) ) <- :boom: [**v16.0.0**](Changelog-v16.html#v1600-2020-08-06)

## v16.4.8 ([2020-12-25](https://github.com/cwtickle/danoniplus/releases/tag/v16.4.8))
- 🐞 カスタムjs, スキンjsを二重読込している問題を修正 ( PR [#917](https://github.com/cwtickle/danoniplus/pull/917) ) <- :boom: [**v7.7.0**](Changelog-v7.html#v770-2019-08-25)
- 🐞 楽曲・画像読込チェックの待ち時間誤りを修正 ( PR [#915](https://github.com/cwtickle/danoniplus/pull/915) ) <- :boom: [**v10.1.1**](Changelog-v10.html#v1011-2019-11-11)

## v16.4.7 ([2020-12-21](https://github.com/cwtickle/danoniplus/releases/tag/v16.4.7))
- 🐞 曲終了直後にリトライキーを押すとALL0のリザルトが表示される問題を修正 ( PR [#908](https://github.com/cwtickle/danoniplus/pull/908) ) <- :boom: [**v0.67.x**](Changelog-v0.html#v067x-2018-11-17)

## v16.4.6 ([2020-11-23](https://github.com/cwtickle/danoniplus/releases/tag/v16.4.6))
- 🐞 Display:Colorのボタンが無効化されていた場合にColorTypeの挙動により、Display:Colorの切り替えができてしまう問題を修正 ( PR [#892](https://github.com/cwtickle/danoniplus/pull/892) ) <- :boom: [**v14.0.2**](Changelog-v14.html#v1402-2020-04-29) 

## v16.4.5 ([2020-11-02](https://github.com/cwtickle/danoniplus/releases/tag/v16.4.5))
- 🐞 速度データ(speed_change)が空の場合、データがあると判断されてしまいspeed_changeが優先されてしまう問題を修正 ( PR [#884](https://github.com/cwtickle/danoniplus/pull/884) ) <- :boom: [**v8.0.0**](Changelog-v8.html#v800-2019-09-08) 

## v16.4.4 ([2020-10-16](https://github.com/cwtickle/danoniplus/releases/tag/v16.4.4))
- 🐞 矢印塗りつぶし有、ステップゾーンをOFFにした場合に矢印塗りつぶし部分が残る問題を修正 ( PR [#866](https://github.com/cwtickle/danoniplus/pull/866) ) <- :boom: [**v5.12.0**](Changelog-v5.html#v5120-2019-06-14)

## v16.4.3 ([2020-10-09](https://github.com/cwtickle/danoniplus/releases/tag/v16.4.3))
- 🛠️ danoni_main.jsに対してstrictモードを解除
- 🐞 tuningのみ指定があった場合に制作者リンクが出ない問題を修正 ( PR [#850](https://github.com/cwtickle/danoniplus/pull/850) ) <- :boom: [**v3.0.0**](Changelog-v3.html#v300-2019-02-25)
- 🐞 ツール値出力時、時間表示がおかしくなることがある問題を修正 ( PR [#858](https://github.com/cwtickle/danoniplus/pull/858) ) <- :boom: [**v12.0.0**](Changelog-v12.html#v1200-2020-02-09) <- [**v2.0.0**](Changelog-v2.html#v200-2019-01-18)

## v16.4.1 ([2020-09-27](https://github.com/cwtickle/danoniplus/releases/tag/v16.4.1))
- 🐞 user-selectがSafariブラウザのみ動作しない問題を修正 ( PR [#832](https://github.com/cwtickle/danoniplus/pull/832) ) <- :boom: [**v16.4.0**](Changelog-v16.html#v1640-2020-09-22)

----

## v16.4.0 ([2020-09-22](https://github.com/cwtickle/danoniplus/releases/tag/v16.4.0))
- ⭐ 結果画面のCLEARED / FAILED表示に対する遅延フレーム設定を実装 ( Issue [#824](https://github.com/cwtickle/danoniplus/pull/824), PR [#828](https://github.com/cwtickle/danoniplus/pull/828) )
- 🛠️ 結果画面周りのコード整理 ( PR [#825](https://github.com/cwtickle/danoniplus/pull/825), [#829](https://github.com/cwtickle/danoniplus/pull/829), [#830](https://github.com/cwtickle/danoniplus/pull/830) )
- 🛠️ 設定画面（フェードイン）のコード整理 ( PR [#826](https://github.com/cwtickle/danoniplus/pull/826) )
- 🛠️ 非推奨関数を削除 ( PR [#827](https://github.com/cwtickle/danoniplus/pull/827), [#829](https://github.com/cwtickle/danoniplus/pull/829) )

## v16.3.0 ([2020-09-05](https://github.com/cwtickle/danoniplus/releases/tag/v16.3.0))
- ⭐ Ready表示のアニメーション変更、先頭色変更に対応 ( PR [#820](https://github.com/cwtickle/danoniplus/pull/820) )
- 🛠️ Ready表示の遅延フレーム設定について、
プレイ中のフェードイン有効時は無効にするよう変更 ( Issue [#819](https://github.com/cwtickle/danoniplus/pull/819), PR [#820](https://github.com/cwtickle/danoniplus/pull/820) )
- 🛠️ Ready表示部分をカスタム関数の前に生成するよう変更 ( PR [#820](https://github.com/cwtickle/danoniplus/pull/820) )
- 🛠️ リザルトデータについてフリーズアローが無い場合、表記を略すように変更 ( Issue [#817](https://github.com/cwtickle/danoniplus/pull/817), PR [#818](https://github.com/cwtickle/danoniplus/pull/818) )

## v16.2.1 ([2020-08-25](https://github.com/cwtickle/danoniplus/releases/tag/v16.2.1))
- ⭐ 20個以上のキーに対する色変化（単発矢印・個別）に対応 ( Issue [#807](https://github.com/cwtickle/danoniplus/pull/807), PR [#812](https://github.com/cwtickle/danoniplus/pull/812) )
- ⭐ リザルトデータのフォーマット機能を実装 ( Issue [#809](https://github.com/cwtickle/danoniplus/pull/809), PR [#813](https://github.com/cwtickle/danoniplus/pull/813) )
- 🐞 リトライ時に稀に早回しになる不具合を修正、キーリピートを無効化 ( PR [#810](https://github.com/cwtickle/danoniplus/pull/810) ) <- :boom: [**v4.0.0**](Changelog-v4.html#v400-2019-04-25)
- 🐞 キー変換処理が抜けていた部分を修正 ( PR [#811](https://github.com/cwtickle/danoniplus/pull/811) ) <- :boom: [**v11.2.0**](Changelog-v11.html#v1120-2020-01-04)

## v16.1.0 ([2020-08-22](https://github.com/cwtickle/danoniplus/releases/tag/v16.1.0))
- ⭐ リザルトデータのクリップボードコピー機能を実装 ( Issue [#803](https://github.com/cwtickle/danoniplus/pull/803), PR [#804](https://github.com/cwtickle/danoniplus/pull/804) )
- 🛠️ CapsLockキーの無効化設定及び無効キーのメッセージを追加 ( Gitter [2020-08-17](https://gitter.im/danonicw/community?at=5f3a8e4a60892e0c69794df8), Issue [#805](https://github.com/cwtickle/danoniplus/pull/805), PR [#806](https://github.com/cwtickle/danoniplus/pull/806) )
- 🛠️ Applicationキーがキーコンフィグ画面、メイン画面で反応しないよう変更 ( PR [#806](https://github.com/cwtickle/danoniplus/pull/806) )

## v16.0.4 ([2020-08-14](https://github.com/cwtickle/danoniplus/releases/tag/v16.0.4))
- 🐞 テンキー一式、atmarkキーが反応しない問題を修正 ( PR [#799](https://github.com/cwtickle/danoniplus/pull/799), [#801](https://github.com/cwtickle/danoniplus/pull/801) ) <- :boom: [**v16.0.0**](Changelog-v16.html#v1600-2020-08-06)

## v16.0.2 ([2020-08-09](https://github.com/cwtickle/danoniplus/releases/tag/v16.0.2))
- 🐞 セミコロンキーが反応しない問題を修正 ( Issue [#796](https://github.com/cwtickle/danoniplus/pull/796), PR [#797](https://github.com/cwtickle/danoniplus/pull/797) ) <- :boom: [**v16.0.0**](Changelog-v16.html#v1600-2020-08-06)

## v16.0.1 ([2020-08-07](https://github.com/cwtickle/danoniplus/releases/tag/v16.0.1))
- 🐞 Shift+Deleteキーの組み合わせが利かない問題を修正 ( Issue [#792](https://github.com/cwtickle/danoniplus/pull/792), PR [#793](https://github.com/cwtickle/danoniplus/pull/793) ) <- :boom: [**v16.0.0**](Changelog-v16.html#v1600-2020-08-06)

## v16.0.0 ([2020-08-06](https://github.com/cwtickle/danoniplus/releases/tag/v16.0.0))
- ⭐ プレイ画面範囲の横幅・位置調整機能を追加 ( Issue [#789](https://github.com/cwtickle/danoniplus/pull/789), PR [#790](https://github.com/cwtickle/danoniplus/pull/790) )
- 🛠️ `KeyboardEvent.keyCode`を`KeyboardEvent.code`へ置き換え ( Issue [#737](https://github.com/cwtickle/danoniplus/pull/737), PR [#783](https://github.com/cwtickle/danoniplus/pull/783) )
- 🛠️ ライフ初期値を小数第2位まで内部的に持つよう変更 ( Issue [#787](https://github.com/cwtickle/danoniplus/pull/787), PR [#788](https://github.com/cwtickle/danoniplus/pull/788) )

[**<- v17**](Changelog-v17.html) | **v16** | [**v15 ->**](Changelog-v15.html)
