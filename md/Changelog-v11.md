⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

[**<- v12**](Changelog-v12.html) | **v11** | [**v10 ->**](Changelog-v10.html)

## [Warning] 更新終了後の不具合情報
- [更新を終了したバージョンの不具合情報#v11](DeprecatedVersionBugs.html#v11) を参照

## v11.4.5 ([2020-04-16](https://github.com/cwtickle/danoniplus/releases/tag/v11.4.5))
- 🛠️ 厳密等価演算子が使用されていない箇所を修正 ( PR [#654](https://github.com/cwtickle/danoniplus/pull/654) )

## v11.4.4 ([2020-04-12](https://github.com/cwtickle/danoniplus/releases/tag/v11.4.4))
- 🐞 キーコンフィグ画面で代替キーの無効化ができない問題を修正 ( PR [#647](https://github.com/cwtickle/danoniplus/pull/647) ) <- :boom: [**v10.3.0**](Changelog-v10.html#v1030-2019-12-01)

## v11.4.3 ([2020-04-11](https://github.com/cwtickle/danoniplus/releases/tag/v11.4.3))
- 🛠️ ローカルで直接htmlファイルを開いても画像が表示されるように変更 ( PR [#627](https://github.com/cwtickle/danoniplus/pull/627), [#628](https://github.com/cwtickle/danoniplus/pull/628) )
- 🐞 設定画面（フェードイン表示）、キーコンフィグ画面（カラータイプ）のid重複を修正 ( PR [#642](https://github.com/cwtickle/danoniplus/pull/642) ) <- :boom: [**v3.12.0**](Changelog-v3.html#v3120-2019-04-21), [**v0.76.x**](Changelog-v0.html#v076x-2018-11-24)

## v11.4.2 ([2020-03-08](https://github.com/cwtickle/danoniplus/releases/tag/v11.4.2))
- 🐞 ダミー矢印のヒット位置が前の通常矢印のヒット結果に引きずられる問題を修正 ( PR [#623](https://github.com/cwtickle/danoniplus/pull/623) ) <- :boom: [**v10.4.0**](Changelog-v10.html#v1040-2019-12-07)

## v11.4.1 ([2020-02-25](https://github.com/cwtickle/danoniplus/releases/tag/v11.4.1))
- 🐞 スコア上書き時ハイスコア差分が計算されない問題を修正 ( PR [#616](https://github.com/cwtickle/danoniplus/pull/616) ) <- :boom: [**v10.5.0**](Changelog-v10.html#v1050-2019-12-13)

----

## v11.4.0 ([2020-02-05](https://github.com/cwtickle/danoniplus/releases/tag/v11.4.0))
- ⭐️ 譜面明細画面に速度変化数・プレイ時間などの補足情報を追加 ( Issue [#417](https://github.com/cwtickle/danoniplus/pull/417), PR [#598](https://github.com/cwtickle/danoniplus/pull/598) )

## v11.3.1 ([2020-01-30](https://github.com/cwtickle/danoniplus/releases/tag/v11.3.1))
- 🛠️ startFrameの値に応じて速度変化・譜面密度グラフの位置が変わるように修正 ( PR [#595](https://github.com/cwtickle/danoniplus/pull/595) )
- 🐞 譜面密度グラフにおいて、最大密度部分に色が付かない問題を修正 ( PR [#595](https://github.com/cwtickle/danoniplus/pull/595) ) <- :boom: [**v11.3.0**](Changelog-v11.html#v1130-2020-01-29)

## v11.3.0 ([2020-01-29](https://github.com/cwtickle/danoniplus/releases/tag/v11.3.0))
- ⭐️ 速度変化の遷移グラフを表示する機能の実装 ( Issue [#417](https://github.com/cwtickle/danoniplus/pull/417), PR [#589](https://github.com/cwtickle/danoniplus/pull/589), [#590](https://github.com/cwtickle/danoniplus/pull/590), [#591](https://github.com/cwtickle/danoniplus/pull/591) )
- ⭐️ 譜面密度グラフの実装 ( Issue [#417](https://github.com/cwtickle/danoniplus/pull/417), PR [#592](https://github.com/cwtickle/danoniplus/pull/592) )
- 🛠️ リザルト画面部分のコード整理 ( PR [#588](https://github.com/cwtickle/danoniplus/pull/588) )
- 🛠️ 譜面ロード部分のコード整理 ( PR [#590](https://github.com/cwtickle/danoniplus/pull/590), [#594](https://github.com/cwtickle/danoniplus/pull/594) )

## v11.2.1 ([2020-01-12](https://github.com/cwtickle/danoniplus/releases/tag/v11.2.1))
- 🛠️ メイン画面初期化部分のコード見直し ( PR [#586](https://github.com/cwtickle/danoniplus/pull/586) )
- 🐞 Display: Judgement をOFFにしたときに、判定キャラクタが消えない問題を修正 ( PR [#586](https://github.com/cwtickle/danoniplus/pull/586) ) <- :boom: [**v11.0.0**](Changelog-v11.html#v1100-2019-12-14)

## v11.2.0 ([2020-01-04](https://github.com/cwtickle/danoniplus/releases/tag/v11.2.0))
- 🛠️ キーを押す操作の処理の見直し ( PR [#582](https://github.com/cwtickle/danoniplus/pull/582) )
- 🐞 ロード画面でブロックすべきキーコントロールがブロックされない問題を修正 ( PR [#581](https://github.com/cwtickle/danoniplus/pull/581) ) <- :boom: [**v8.0.4**](Changelog-v8.html#v804-2019-09-23)
- 🐞 譜面名未指定のときにリザルトコピー時のクレジットがundefinedになる問題を修正 ( PR [#583](https://github.com/cwtickle/danoniplus/pull/583) ) <- :boom: [**v8.2.0**](Changelog-v8.html#v820-2019-09-24)

## v11.1.2 ([2019-12-28](https://github.com/cwtickle/danoniplus/releases/tag/v11.1.2))
- ⭐️ 下側の歌詞表示位置をステップゾーン位置に追随させる設定を追加 ( PR [#574](https://github.com/cwtickle/danoniplus/pull/574) )
- ⭐️ 判定キャラクタ、ReadyのY座標を下側のステップゾーン位置(stepYR)に合わせて
自動調整するように変更 ( PR [#574](https://github.com/cwtickle/danoniplus/pull/574) )
- 🐞 ライフが0のとき、ライフ値が反映されない問題を修正 ( PR [#573](https://github.com/cwtickle/danoniplus/pull/573), [#576](https://github.com/cwtickle/danoniplus/pull/576) ) <- :boom: [**v10.5.0**](Changelog-v10.html#v1050-2019-12-13)

## v11.0.2 ([2019-12-22](https://github.com/cwtickle/danoniplus/releases/tag/v11.0.2))
- 🐞 キーコンフィグがundefinedになる場合がある問題を修正 ( PR [#569](https://github.com/cwtickle/danoniplus/pull/569) ) <- :boom: **initial**
- 🐞 実装途中の未定義関数により、低速時エラーで止まる問題を修正 ( PR [#570](https://github.com/cwtickle/danoniplus/pull/570) ) <- :boom: [**v10.3.0**](Changelog-v10.html#v1030-2019-12-01)

## v11.0.1 ([2019-12-16](https://github.com/cwtickle/danoniplus/releases/tag/v11.0.1))
- 🐞 Fast表示の誤字を修正 ( PR [#566](https://github.com/cwtickle/danoniplus/pull/566) ) <- :boom: [**v11.0.0**](Changelog-v11.html#v1100-2019-12-14)
- 🐞 結果画面（曲名）のid重複を修正 ( PR [#567](https://github.com/cwtickle/danoniplus/pull/567) ) <- :boom: [**v3.5.0**](Changelog-v3.html#v350-2019-03-23)

## v11.0.0 ([2019-12-14](https://github.com/cwtickle/danoniplus/releases/tag/v11.0.0))
- ⭐️ Displayオプションのデフォルト設定を追加 ( Issue [#415](https://github.com/cwtickle/danoniplus/pull/415), PR [#556](https://github.com/cwtickle/danoniplus/pull/556) )
- ⭐️ カスタム用のDisplayオプション「Special」を追加 ( PR [#556](https://github.com/cwtickle/danoniplus/pull/556) )
- ⭐️ 判定キャラクタの下にFast/Slow/Just表記を追加 ( PR [#556](https://github.com/cwtickle/danoniplus/pull/556) )
- ⭐️ 判定キャラクタの位置調整機能を追加 ( Issue [#415](https://github.com/cwtickle/danoniplus/pull/415), PR [#556](https://github.com/cwtickle/danoniplus/pull/556) )
- ⭐️ 5keyのKeyPattern: 3(おにぎり中央)の既定のキーコンフィグを変更 ( PR [#555](https://github.com/cwtickle/danoniplus/pull/555) )
- ⭐️ 7keyの既定のキーコンフィグを追加 ( PR [#555](https://github.com/cwtickle/danoniplus/pull/555) )
- 🛠️ 別キーモードで、指定の必要が無い項目を削除 ( PR [#555](https://github.com/cwtickle/danoniplus/pull/555) )
- 🛠️ fileでも起動可能なようにcrossorigin属性の付加条件を変更 ( PR [#564](https://github.com/cwtickle/danoniplus/pull/564) )

[**<- v12**](Changelog-v12.html) | **v11** | [**v10 ->**](Changelog-v10.html)
