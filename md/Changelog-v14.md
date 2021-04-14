⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

[**<- v15**](Changelog-v15.html) | **v14** | [**v13 ->**](Changelog-v13.html)

## v14.5.20 ([2021-04-07](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.20))
- 🐞 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まる問題を修正
 ( PR [#1044](https://github.com/cwtickle/danoniplus/pull/1044), Gitter [2021-04-06](https://gitter.im/danonicw/community?at=606c808592a3431fd67b1640) ) <- :boom: [**v3.1.0**](Changelog-v3.html#v310-2019-02-26)

## v14.5.19 ([2021-03-06](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.19))
- 🛠️ Base64エンコードした曲データを直接デコードするよう変更 ( PR [#1009](https://github.com/cwtickle/danoniplus/pull/1009) )

## v14.5.18 ([2021-02-20](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.18))
- 🛠️ imgタグ生成時においてcrossOrigin属性を付与するよう変更 ( PR [#988](https://github.com/cwtickle/danoniplus/pull/988) )

## v14.5.17 ([2021-01-05](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.17))
- 🐞 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、通常矢印の判定が優先されてしまう事象を修正 ( PR [#929](https://github.com/cwtickle/danoniplus/pull/929), [#930](https://github.com/cwtickle/danoniplus/pull/930), [#932](https://github.com/cwtickle/danoniplus/pull/932) ) <- :boom: **initial**

## v14.5.16 ([2020-12-25](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.16))
- 🐞 カスタムjs, スキンjsを二重読込している問題を修正 ( PR [#917](https://github.com/cwtickle/danoniplus/pull/917) ) <- :boom: [**v7.7.0**](Changelog-v7.html#v770-2019-08-25)
- 🐞 楽曲・画像読込チェックの待ち時間誤りを修正 ( PR [#915](https://github.com/cwtickle/danoniplus/pull/915) ) <- :boom: [**v10.1.1**](Changelog-v10.html#v1011-2019-11-11)

## v14.5.15 ([2020-12-21](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.15))
- 🐞 曲終了直後にリトライキーを押すとALL0のリザルトが表示される問題を修正 ( PR [#908](https://github.com/cwtickle/danoniplus/pull/908) ) <- :boom: [**v0.67.x**](Changelog-v0.html#v067x-2018-11-17) 

## v14.5.14 ([2020-11-23](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.14))
- 🐞 Display:Colorのボタンが無効化されていた場合にColorTypeの挙動により、Display:Colorの切り替えができてしまう問題を修正 ( PR [#892](https://github.com/cwtickle/danoniplus/pull/892) ) <- :boom: [**v14.0.2**](Changelog-v14.html#v1402-2020-04-29) 

## v14.5.13 ([2020-11-02](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.13))
- 🐞 速度データ(speed_change)が空の場合、データがあると判断されてしまいspeed_changeが優先されてしまう問題を修正 ( PR [#884](https://github.com/cwtickle/danoniplus/pull/884) ) <- :boom: [**v8.0.0**](Changelog-v8.html#v800-2019-09-08) 

## v14.5.12 ([2020-10-16](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.12))
- 🐞 矢印塗りつぶし有、ステップゾーンをOFFにした場合に矢印塗りつぶし部分が残る問題を修正 ( PR [#866](https://github.com/cwtickle/danoniplus/pull/866) ) <- :boom: [**v5.12.0**](Changelog-v5.html#v5120-2019-06-14)

## v14.5.11 ([2020-10-09](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.11))
- 🛠️ danoni_main.jsに対してstrictモードを解除
- 🐞 tuningのみ指定があった場合に制作者リンクが出ない問題を修正 ( PR [#850](https://github.com/cwtickle/danoniplus/pull/850) ) <- :boom: [**v3.0.0**](Changelog-v3.html#v300-2019-02-25)
- 🐞 ツール値出力時、時間表示がおかしくなることがある問題を修正 ( PR [#858](https://github.com/cwtickle/danoniplus/pull/858) ) <- :boom: [**v12.0.0**](Changelog-v12.html#v1200-2020-02-09) <- [**v2.0.0**](Changelog-v2.html#v200-2019-01-18)

## v14.5.9 ([2020-08-24](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.9))
- 🐞 リトライ時に稀に早回しになる不具合を修正、キーリピートを無効化 ( PR [#810](https://github.com/cwtickle/danoniplus/pull/810) ) <- :boom: [**v4.0.0**](Changelog-v4.html#v400-2019-04-25)
- 🐞 キー変換処理が抜けていた部分を修正 ( PR [#811](https://github.com/cwtickle/danoniplus/pull/811) ) <- :boom: [**v11.2.0**](Changelog-v11.html#v1120-2020-01-04)

## v14.5.8 ([2020-08-22](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.8))
- 🛠️ Applicationキーがキーコンフィグ画面、メイン画面で反応しないよう変更 ( PR [#806](https://github.com/cwtickle/danoniplus/pull/806) )

## v14.5.7 ([2020-07-02](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.7))
- 🛠️ バージョン比較用のリンクをSecurity Policyに変更 ( Issue [#759](https://github.com/cwtickle/danoniplus/pull/759), PR [#760](https://github.com/cwtickle/danoniplus/pull/760) )

## v14.5.6 ([2020-06-27](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.6))
- 🐞 カスタムゲージ使用時にクリア失敗時のリザルトモーションが使用できない問題を修正 ( Issue [#749](https://github.com/cwtickle/danoniplus/pull/749), PR [#751](https://github.com/cwtickle/danoniplus/pull/751) ) <- :boom: [**v9.4.0**](Changelog-v9.html#v940-2019-10-20)

## v14.5.5 ([2020-06-21](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.5))
- 🛠️ プレイ中に他のキーイベントが呼ばれないようにするよう変更 ( PR [#741](https://github.com/cwtickle/danoniplus/pull/741) )

## v14.5.4 ([2020-06-18](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.4))
- 🐞 通常キーであらかじめデフォルトセットされているキーコンフィグパターンと異なるキーを割り当てた際、初回保存時のみそのキーがリセットされる問題を修正 ( PR [#738](https://github.com/cwtickle/danoniplus/pull/738) ) <- :boom: [**v6.6.0**](Changelog-v6.html#v660-2019-07-08)

## v14.5.3 ([2020-05-24](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.3))
- 🐞 特殊キーの後に通常キーの譜面があると譜面選択できない問題を修正 ( PR [#729](https://github.com/cwtickle/danoniplus/pull/729) ) <- :boom: [**v4.6.2**](Changelog-v4.html#v462-2019-05-04)

----

## v14.5.2 ([2020-05-13](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.2))
- 🛠️ バージョン比較用リンクを作成 ( PR [#711](https://github.com/cwtickle/danoniplus/pull/711) )

## v14.5.1 ([2020-05-09](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.1))
- 🛠️ 譜面データ用の特殊文字対象にバッククォート、シングルクォートを追加 ( PR [#706](https://github.com/cwtickle/danoniplus/pull/706) )
- 🐞 歌詞表示の一部で置き換え文字の処理が利いていない問題を修正 ( PR [#706](https://github.com/cwtickle/danoniplus/pull/706) ) <- :boom: [**v14.4.0**](Changelog-v14.html#v1440-2020-05-05)

## v14.5.0 ([2020-05-07](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.0))
- ⭐ 譜面数が5を超える場合、自動で譜面セレクターを使用するよう変更 ( PR [#703](https://github.com/cwtickle/danoniplus/pull/703) )
- 🛠️ グラフON/OFFボタン、Data Saveボタン等の説明文を追加 ( PR [#701](https://github.com/cwtickle/danoniplus/pull/701) )
- 🛠️ Twitter投稿リザルトで曲名・制作者名の後に半角空白を追加 ( PR [#702](https://github.com/cwtickle/danoniplus/pull/702) )
- 🐞 danoni_setting.jsでDisplay設定を明示的に有効にした場合、ボタンの初期値がOFFになってしまう問題を修正 ( PR [#700](https://github.com/cwtickle/danoniplus/pull/700) ) <- :boom: [**v14.0.2**](Changelog-v14.html#v1402-2020-04-29)

## v14.4.0 ([2020-05-05](https://github.com/cwtickle/danoniplus/releases/tag/v14.4.0))
- ⭐ 譜面データでカンマ、ドル等の特殊文字を利用するための文字列を作成 ( Issue [#697](https://github.com/cwtickle/danoniplus/pull/697), PR [#696](https://github.com/cwtickle/danoniplus/pull/696) )
- 🐞 結果画面のTweetで<, >の文字が置換されて表示されてしまう問題を修正 ( PR [#696](https://github.com/cwtickle/danoniplus/pull/696) ) <- :boom:   **initial**

## v14.3.4 ([2020-05-04](https://github.com/cwtickle/danoniplus/releases/tag/v14.3.4))
- ⭐ ローカル時に限り、誤差1フレームでもFast/Slowを表示するように変更 ( PR [#685](https://github.com/cwtickle/danoniplus/pull/685) )
- ⭐ 結果画面にFast/Slowのカウント数を表示するよう変更 ( PR [#685](https://github.com/cwtickle/danoniplus/pull/685), [#693](https://github.com/cwtickle/danoniplus/pull/693), [#695](https://github.com/cwtickle/danoniplus/pull/695) )
- ⭐ ±1フレーム以内で表示するJust表記を廃止 ( PR [#685](https://github.com/cwtickle/danoniplus/pull/685) )
- ⭐ Twitter投稿用リザルトのURL表示に譜面番号を付加するよう変更 ( PR [#686](https://github.com/cwtickle/danoniplus/pull/686) )
- ⭐ 譜面データでパイプ、アンパサンド等の特殊文字を利用するための文字列を作成 ( PR [#688](https://github.com/cwtickle/danoniplus/pull/688) )
- 🛠️ フリーズアローヒット時のコード整理 ( PR [#684](https://github.com/cwtickle/danoniplus/pull/684) )
- 🐞 フリーズ始点判定有効時、シャキン以下の判定関数に差分フレーム数としてマイナス値が渡せていない問題を修正 ( PR [#684](https://github.com/cwtickle/danoniplus/pull/684) ) <- :boom: [**v5.7.0**](Changelog-v5.html#v570-2019-06-01)

## v14.2.0 ([2020-05-03](https://github.com/cwtickle/danoniplus/releases/tag/v14.2.0))
- 🛠️ APMの計算式をレベル計算ツール++の形式に寄せるよう修正 ( PR [#682](https://github.com/cwtickle/danoniplus/pull/682) )
- 🛠️ Appearanceの「Slit」を削除 ( PR [#681](https://github.com/cwtickle/danoniplus/pull/681) )
- 🐞 高速(5x以上)で矢印を見逃したとき、画面上に矢印が残ることがある事象を修正 ( PR [#681](https://github.com/cwtickle/danoniplus/pull/681) ) <- :boom: [**v14.1.0**](Changelog-v14.html#v1410-2020-05-01)

## v14.1.0 ([2020-05-01](https://github.com/cwtickle/danoniplus/releases/tag/v14.1.0))
- ⭐ 矢印描画について、ステップゾーン位置に応じて描画領域が変わるように変更  ( PR [#673](https://github.com/cwtickle/danoniplus/pull/673) )
- ⭐ Display: MusicInfo適用時、楽曲のクレジットを最初の数秒のみ表示する形式に変更 ( PR [#674](https://github.com/cwtickle/danoniplus/pull/674) )
- ⭐ グラデーション表記で色名 (blueやredなど) が使えるよう変更 ( PR [#675](https://github.com/cwtickle/danoniplus/pull/675) )
- 🛠️ 影矢印のデザインを見直し ( PR [#672](https://github.com/cwtickle/danoniplus/pull/672) )
- 🛠️ setShadowColor有効時、ステップゾーンとフリーズアローの塗りつぶし色の
適用スタイルをcssとして分けるように変更 ( PR [#672](https://github.com/cwtickle/danoniplus/pull/672) )
- 🛠️ ステップゾーン位置関連の変数をオブジェクトへ集約 ( PR [#673](https://github.com/cwtickle/danoniplus/pull/673) )
- 🛠️ 譜面ヘッダー：playbackRate, maxLifeValに対して入力チェックを強化 ( PR [#675](https://github.com/cwtickle/danoniplus/pull/675) )
- 🛠️ 結果画面で表示するHidden+, Sudden+について、パーセント表記を廃止 ( PR [#673](https://github.com/cwtickle/danoniplus/pull/673) )

## v14.0.2 ([2020-04-29](https://github.com/cwtickle/danoniplus/releases/tag/v14.0.2))
- ⭐ DisplayオプションのデフォルトOFF設定及び有効/無効化設定の実装 ( PR [#665](https://github.com/cwtickle/danoniplus/pull/665) )
- ⭐ DisplayオプションのボタンがONの状態のとき、
他のボタンを連動してOFFに自動変更する機能を実装 ( Issue [#664](https://github.com/cwtickle/danoniplus/pull/664), PR [#665](https://github.com/cwtickle/danoniplus/pull/665) )
- ⭐ オンマウスでオプション設定の説明文を表示するよう変更 ( PR [#663](https://github.com/cwtickle/danoniplus/pull/663) )
- 🛠️ 警告メッセージを常に再作成し手前に来るよう変更 ( PR [#665](https://github.com/cwtickle/danoniplus/pull/665) )
- 🛠️ 警告メッセージエリアの最大長を設定し、超過した場合はスクロールするよう変更 ( PR [#670](https://github.com/cwtickle/danoniplus/pull/670) )
- 🐞 キーコンフィグ画面で、割り当てキーがundefinedとなる場合がある問題を修正 ( PR [#668](https://github.com/cwtickle/danoniplus/pull/668) ) <- :boom: [**v13.3.1**](Changelog-v13.html#v1331-2020-04-12)

[**<- v15**](Changelog-v15.html) | **v14** | [**v13 ->**](Changelog-v13.html)
