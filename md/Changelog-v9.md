⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

[**<- v10**](Changelog-v10.html) | **v9** | [**v8 ->**](Changelog-v8.html)

## [Warning] 更新終了後の不具合情報
- [更新を終了したバージョンの不具合情報#v9](DeprecatedVersionBugs.html#v9) を参照

## v9.4.27 ([2021-01-05](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.27))
- 🐞 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、通常矢印の判定が優先されてしまう事象を修正 ( PR [#929](https://github.com/cwtickle/danoniplus/pull/929), [#930](https://github.com/cwtickle/danoniplus/pull/930), [#932](https://github.com/cwtickle/danoniplus/pull/932) ) <- :boom: **initial**

## v9.4.26 ([2020-12-25](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.26))
- 🐞 カスタムjs, スキンjsを二重読込している問題を修正 ( PR [#917](https://github.com/cwtickle/danoniplus/pull/917) ) <- :boom: [**v7.7.0**](Changelog-v7.html#v770-2019-08-25)
- 🐞 楽曲・画像読込チェックの待ち時間誤りを修正 ( PR [#915](https://github.com/cwtickle/danoniplus/pull/915) ) <- :boom: [**v9.4.5**](Changelog-v9.html#v945-2019-11-11)

## v9.4.25 ([2020-12-21](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.25))
- 🐞 曲終了直後にリトライキーを押すとALL0のリザルトが表示される問題を修正 ( PR [#908](https://github.com/cwtickle/danoniplus/pull/908) ) <- :boom: [**v0.67.x**](Changelog-v0.html#v067x-2018-11-17) 

## v9.4.24 ([2020-11-02](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.24))
- 🐞 速度データ(speed_change)が空の場合、データがあると判断されてしまいspeed_changeが優先されてしまう問題を修正 ( PR [#884](https://github.com/cwtickle/danoniplus/pull/884) ) <- :boom: [**v8.0.0**](Changelog-v8.html#v800-2019-09-08) 

## v9.4.23 ([2020-10-17](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.23))
- 🛠️ ローカルで直接ファイルを開いた場合のみ、内蔵のsvgデータを使うよう変更

## v9.4.22 ([2020-10-16](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.22))
- 🐞 矢印塗りつぶし有、ステップゾーンをOFFにした場合に矢印塗りつぶし部分が残る問題を修正 ( PR [#866](https://github.com/cwtickle/danoniplus/pull/866) ) <- :boom: [**v5.12.0**](Changelog-v5.html#v5120-2019-06-14)

## v9.4.21 ([2020-10-09](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.21))
- 🛠️ danoni_main.jsに対してstrictモードを解除
- 🐞 tuningのみ指定があった場合に制作者リンクが出ない問題を修正 ( PR [#850](https://github.com/cwtickle/danoniplus/pull/850) ) <- :boom: [**v3.0.0**](Changelog-v3.html#v300-2019-02-25)

## v9.4.19 ([2020-08-24](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.19))
- 🐞 リトライ時に稀に早回しになる不具合を修正、キーリピートを無効化 ( PR [#810](https://github.com/cwtickle/danoniplus/pull/810) ) <- :boom: [**v4.0.0**](Changelog-v4.html#v400-2019-04-25)
- 🐞 キー変換処理が抜けていた部分を修正 ( PR [#811](https://github.com/cwtickle/danoniplus/pull/811) ) <- :boom: [**v11.2.0**](Changelog-v11.html#v1120-2020-01-04)

## v9.4.18 ([2020-08-22](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.18))
- 🛠️ Applicationキーがキーコンフィグ画面、メイン画面で反応しないよう変更 ( PR [#806](https://github.com/cwtickle/danoniplus/pull/806) )

## v9.4.17 ([2020-07-02](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.17))
- 🛠️ バージョン比較用のリンクをSecurity Policyに変更 ( Issue [#759](https://github.com/cwtickle/danoniplus/pull/759), PR [#760](https://github.com/cwtickle/danoniplus/pull/760) )

## v9.4.16 ([2020-06-27](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.16))
- 🐞 カスタムゲージ使用時にクリア失敗時のリザルトモーションが使用できない問題を修正 ( Issue [#749](https://github.com/cwtickle/danoniplus/pull/749), PR [#751](https://github.com/cwtickle/danoniplus/pull/751) ) <- :boom: [**v9.4.0**](Changelog-v9.html#v940-2019-10-20)

## v9.4.15 ([2020-06-21](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.15))
- 🛠️ プレイ中に他のキーイベントが呼ばれないようにするよう変更 ( PR [#741](https://github.com/cwtickle/danoniplus/pull/741) )
- 🐞 バージョンチェック用リンクにより画面エラーが表示される問題を修正 <- :boom: [**v9.4.12**](Changelog-v9.html#v9412-2020-05-13)
- 🐞 MacOS, iOS (Safari)で音楽データがテキストデータの場合にエラーが表示される問題を修正 <- :boom: [**v9.4.5**](Changelog-v9.html#v945-2019-11-11)

## v9.4.14 ([2020-06-18](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.14))
- 🐞 通常キーであらかじめデフォルトセットされているキーコンフィグパターンと異なるキーを割り当てた際、初回保存時のみそのキーがリセットされる問題を修正 ( PR [#738](https://github.com/cwtickle/danoniplus/pull/738) ) <- :boom: [**v6.6.0**](Changelog-v6.html#v660-2019-07-08)

## v9.4.13 ([2020-05-24](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.13))
- 🐞 特殊キーの後に通常キーの譜面があると譜面選択できない問題を修正 ( PR [#729](https://github.com/cwtickle/danoniplus/pull/729) ) <- :boom: [**v4.6.2**](Changelog-v4.html#v462-2019-05-04)

## v9.4.12 ([2020-05-13](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.12))
- 🛠️ バージョン比較用リンクを作成 ( PR [#711](https://github.com/cwtickle/danoniplus/pull/711) )

## v9.4.11 ([2020-05-04](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.11))
- 🛠️ 警告メッセージを常に再作成し手前に来るよう変更 ( PR [#665](https://github.com/cwtickle/danoniplus/pull/665) )
- 🛠️ 警告メッセージエリアの最大長を設定し、超過した場合はスクロールするよう変更 ( PR [#670](https://github.com/cwtickle/danoniplus/pull/670) )
- 🐞 フリーズ始点判定有効時、シャキン以下の判定関数に差分フレーム数としてマイナス値が渡せていない問題を修正 ( PR [#684](https://github.com/cwtickle/danoniplus/pull/684) ) <- :boom: [**v5.7.0**](Changelog-v5.html#v570-2019-06-01)

## v9.4.10 ([2020-04-16](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.10))
- 🛠️ 厳密等価演算子が使用されていない箇所を修正 ( PR [#654](https://github.com/cwtickle/danoniplus/pull/654) )

## v9.4.9 ([2020-04-11](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.9))
- 🐞 設定画面（フェードイン表示）、キーコンフィグ画面（カラータイプ）のid重複を修正 ( PR [#642](https://github.com/cwtickle/danoniplus/pull/642) ) <- :boom: [**v3.12.0**](Changelog-v3.html#v3120-2019-04-21), [**v0.76.x**](Changelog-v0.html#v076x-2018-11-24)

## v9.4.8 ([2020-01-04](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.8))
- 🐞 ロード画面でブロックすべきキーコントロールがブロックされない問題を修正 ( PR [#581](https://github.com/cwtickle/danoniplus/pull/581) ) <- :boom: [**v8.0.4**](Changelog-v8.html#v804-2019-09-23)
- 🐞 譜面名未指定のときにリザルトコピー時のクレジットがundefinedになる問題を修正 ( PR [#583](https://github.com/cwtickle/danoniplus/pull/583) ) <- :boom: [**v8.2.0**](Changelog-v8.html#v820-2019-09-24)
- 🐞 結果画面（曲名）のid重複を修正 ( PR [#567](https://github.com/cwtickle/danoniplus/pull/567) ) <- :boom: [**v3.5.0**](Changelog-v3.html#v350-2019-03-23)

## v9.4.6 ([2019-12-14](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.6))
- 🛠️ Localhost時にフレーム数を表示するように変更 ( PR [#561](https://github.com/cwtickle/danoniplus/pull/561) )
- 🛠️ ラベルのID重複を解消 ( PR [#545](https://github.com/cwtickle/danoniplus/pull/545), [#546](https://github.com/cwtickle/danoniplus/pull/546), [#562](https://github.com/cwtickle/danoniplus/pull/562) )
- 🛠️ fileでも起動可能なようにcrossorigin属性の付加条件を変更 ( PR [#564](https://github.com/cwtickle/danoniplus/pull/564) )

## v9.4.5 ([2019-11-11](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.5))
- 🐞 MacOS, iOS (Safari)においてWeb Audio APIが動作しない問題を修正 ( PR [#523](https://github.com/cwtickle/danoniplus/pull/523), [#525](https://github.com/cwtickle/danoniplus/pull/525), [#527](https://github.com/cwtickle/danoniplus/pull/527) ) <- :boom: **initial**
- 🐞 MacOS, iOS (Safari)でAppearanceが動作しない問題を修正 ( PR [#523](https://github.com/cwtickle/danoniplus/pull/523) ) <- :boom: **initial**

----

## v9.4.3 ([2019-10-25](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.3))
- 🛠️ 設定画面で表示されるゲージ詳細の表記を見直し ( PR [#508](https://github.com/cwtickle/danoniplus/pull/508) )
- 🛠️ カスタムゲージ設定利用時で、デフォルト以外を選択したときに結果画面にその内容が反映されるように変更 ( PR [#508](https://github.com/cwtickle/danoniplus/pull/508) )

## v9.4.2 ([2019-10-21](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.2))
- 🐞 Ready?の遅延フレーム設定でAdjustmentが反映されていない問題を修正 ( PR [#504](https://github.com/cwtickle/danoniplus/pull/504) ) <- :boom: [**v9.3.0**](Changelog-v9.html#v930-2019-10-20)
- 🐞 カスタムゲージ利用時、gaugeSuddenDeathが未定義の場合に設定が反映されない問題を修正 ( PR [#505](https://github.com/cwtickle/danoniplus/pull/505) ) <- :boom: [**v9.4.0**](Changelog-v9.html#v940-2019-10-20)

## v9.4.1 ([2019-10-21](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.1))
- 🛠️ 設定画面で表示されるゲージ詳細のライフ初期値を整数で表示するよう変更 ( PR [#501](https://github.com/cwtickle/danoniplus/pull/501) )
- 🐞 個別色変化時にフリーズアロー(AA)ヒット時の色が変わらない問題を修正 ( PR [#500](https://github.com/cwtickle/danoniplus/pull/500) ) <- :boom: [**v9.2.0**](Changelog-v9.html#v920-2019-10-19)

## v9.4.0 ([2019-10-20](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.0))
- ⭐️ カスタムゲージ設定の実装 ( PR [#496](https://github.com/cwtickle/danoniplus/pull/496) )
- 🛠️ ゲージ設定詳細のデザインを変更 ( PR [#496](https://github.com/cwtickle/danoniplus/pull/496) )
- 🛠️ ライフ/ノルマ制の区分と回復・ダメージ量の固定/変動区分を分離 ( PR [#496](https://github.com/cwtickle/danoniplus/pull/496) )

## v9.3.0 ([2019-10-20](https://github.com/cwtickle/danoniplus/releases/tag/v9.3.0))
- ⭐️ キーコンフィグ画面からDisplay画面にも戻れるように対応 ( PR [#494](https://github.com/cwtickle/danoniplus/pull/494) )
- ⭐️ Ready表示の遅延フレーム設定を追加 ( Issue [#491](https://github.com/cwtickle/danoniplus/pull/491), PR [#495](https://github.com/cwtickle/danoniplus/pull/495) )
- ⭐️ リバース用の歌詞表示（wordRev_data）を実装 ( PR [#497](https://github.com/cwtickle/danoniplus/pull/497) )

## v9.2.0 ([2019-10-19](https://github.com/cwtickle/danoniplus/releases/tag/v9.2.0))
- ⭐️ フリーズアローヒット部分の描画方法を変更し、Hidden適用時でもヒット部分がわかるように変更 ( PR [#492](https://github.com/cwtickle/danoniplus/pull/492) )
- ⭐️ フリーズアローバーの透明度を常時75％に変更 ( PR [#492](https://github.com/cwtickle/danoniplus/pull/492) )
- 🛠️ メイン画面のフレームカウント条件を見直し ( PR [#492](https://github.com/cwtickle/danoniplus/pull/492) )
- 🛠️ 矢印描画で対応していたIE/Edge互換設定の撤去 ( PR [#492](https://github.com/cwtickle/danoniplus/pull/492) )

## v9.1.0 ([2019-10-15](https://github.com/cwtickle/danoniplus/releases/tag/v9.1.0))
- 🛠️ 2譜面目以降で矢印・背景・マスクモーションが未指定の場合、1譜面目のデータを読み込むように変更 ( PR [#487](https://github.com/cwtickle/danoniplus/pull/487) )
- 🐞 背景・マスクモーションでオールクリアが使用できない問題を修正 ( PR [#488](https://github.com/cwtickle/danoniplus/pull/488) ) <- :boom: [**v7.7.0**](Changelog-v7.html#v770-2019-08-25)

## v9.0.3 ([2019-10-13](https://github.com/cwtickle/danoniplus/releases/tag/v9.0.3))
- 🐞 ダミーIDの譜面ヘッダー誤りを修正 ( PR [#483](https://github.com/cwtickle/danoniplus/pull/483) ) <- :boom: [**v6.0.0**](Changelog-v6.html#v600-2019-06-22)
- 🐞 ダミー矢印/フリーズアロー用カスタム関数が定義できない問題を修正 ( PR [#485](https://github.com/cwtickle/danoniplus/pull/485) ) <- :boom: [**v6.1.0**](Changelog-v6.html#v610-2019-06-22)

## v9.0.1 ([2019-10-12](https://github.com/cwtickle/danoniplus/releases/tag/v9.0.1))
- 🐞 低速時かつフリーズアロー開始判定時にPF判定が早まる問題を修正 ( PR [#481](https://github.com/cwtickle/danoniplus/pull/481) ) <- :boom: [**v5.7.0**](Changelog-v5.html#v570-2019-06-01)

## v9.0.0 ([2019-10-08](https://github.com/cwtickle/danoniplus/releases/tag/v9.0.0))
- ⭐️ Appearanceオプションの実装 ( Issue [#475](https://github.com/cwtickle/danoniplus/pull/475), PR [#476](https://github.com/cwtickle/danoniplus/pull/476) )
- ⭐️ Appearance有効/無効設定の追加 ( PR [#476](https://github.com/cwtickle/danoniplus/pull/476) )

[**<- v10**](Changelog-v10.html) | **v9** | [**v8 ->**](Changelog-v8.html)
