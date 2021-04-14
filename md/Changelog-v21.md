⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

 | **v21** | [**v20 ->**](Changelog-v20.html)

## v21.4.2 ([2021-04-07](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.2))
- ⭐ キーコンフィグの対応キー箇所をボタンに変更 ( PR [#1040](https://github.com/cwtickle/danoniplus/pull/1040), [#1048](https://github.com/cwtickle/danoniplus/pull/1048) )
- 🛠️ キー数、共通処理系のコード整理 ( PR [#1041](https://github.com/cwtickle/danoniplus/pull/1041), [#1042](https://github.com/cwtickle/danoniplus/pull/1042), [#1043](https://github.com/cwtickle/danoniplus/pull/1043), [#1045](https://github.com/cwtickle/danoniplus/pull/1045), [#1046](https://github.com/cwtickle/danoniplus/pull/1046), [#1050](https://github.com/cwtickle/danoniplus/pull/1050) )
- 🛠️ 警告ウィンドウ内の上下レイアウト崩れを改善 ( Issue [#823](https://github.com/cwtickle/danoniplus/pull/823), PR [#1046](https://github.com/cwtickle/danoniplus/pull/1046) )
- 🐞 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まる問題を修正
 ( PR [#1044](https://github.com/cwtickle/danoniplus/pull/1044), Gitter [2021-04-06](https://gitter.im/danonicw/community?at=606c808592a3431fd67b1640) ) <- :boom: [**v3.1.0**](Changelog-v3.html#v310-2019-02-26)

## v21.3.0 ([2021-04-03](https://github.com/cwtickle/danoniplus/releases/tag/v21.3.0))
- 🛠️ 同じ警告メッセージが二重に表示される可能性がある問題を改善 ( PR [#1037](https://github.com/cwtickle/danoniplus/pull/1037)  )
- 🛠️ g_loadObjのプロパティ値について、読込完了時に `true` に変えるよう統一 ( PR [#1036](https://github.com/cwtickle/danoniplus/pull/1036) )
- 🛠️ 空スプライト作成処理を`createEmptySprite`関数へ移行 ( PR [#1038](https://github.com/cwtickle/danoniplus/pull/1038) )

## v21.2.0 ([2021-03-28](https://github.com/cwtickle/danoniplus/releases/tag/v21.2.0))
- ⭐ 背景状況により明暗用のカラーセットを使用するよう変更 ( PR [#1033](https://github.com/cwtickle/danoniplus/pull/1033) )
- ⭐ ColorType：Type0について、未指定かつ明背景の場合、自動で中間色を黒にするよう変更 ( PR [#1033](https://github.com/cwtickle/danoniplus/pull/1033) )
- 🛠️ データセーブフラグ切替ボタンをDisplay画面にも表示 ( PR [#1032](https://github.com/cwtickle/danoniplus/pull/1032) )
- 🛠️ danoni3.html のカスタムjsサンプルを更新 ( PR [#1034](https://github.com/cwtickle/danoniplus/pull/1034) )
- 🛠️ メッセージ表示周りのコード整理 ( PR [#1033](https://github.com/cwtickle/danoniplus/pull/1033) )
- 🛠️ CSSファイルの動的読み込みについて読込完了待ちをするよう変更 ( PR [#1033](https://github.com/cwtickle/danoniplus/pull/1033) )

## v21.1.0 ([2021-03-19](https://github.com/cwtickle/danoniplus/releases/tag/v21.1.0))
- ⭐ 譜面毎にカスタムゲージリストが作成できるように変更 ( PR [#1024](https://github.com/cwtickle/danoniplus/pull/1024) )
- ⭐ ゲージ個別設定（譜面ヘッダー）について、譜面毎の分割記法に対応 ( PR [#1024](https://github.com/cwtickle/danoniplus/pull/1024) )
- ⭐ 譜面分割＆譜面番号可変時、初期矢印・フリーズアロー色（setColor2, frzColor2, ...）を譜面番号固定時と同様、個別の譜面ファイルへ記載できるように変更 ( PR [#1024](https://github.com/cwtickle/danoniplus/pull/1024) )
- ⭐ カスタムゲージリストについて、ライフ制ゲージ/ノルマ制ゲージ/共通設定ファイルで指定のリストを設定できるよう変更 ( Issue [#1026](https://github.com/cwtickle/danoniplus/pull/1026), PR [#1027](https://github.com/cwtickle/danoniplus/pull/1027) )
- 🛠️ 文字列関連のコード整理 ( PR [#1024](https://github.com/cwtickle/danoniplus/pull/1024), [#1025](https://github.com/cwtickle/danoniplus/pull/1025) )

## v21.0.0 ([2021-03-12](https://github.com/cwtickle/danoniplus/releases/tag/v21.0.0))
- ⭐ 初期矢印・フリーズアロー色(setColor/frzColor)の譜面別設定実装 ( Issue [#390](https://github.com/cwtickle/danoniplus/pull/390), PR [#1019](https://github.com/cwtickle/danoniplus/pull/1019) )
- ⭐ 譜面分割＆譜面番号固定時、個別の譜面ファイル内に
setColor/frzColor/setShadowColor/frzShadowColorの記述があれば、その値を採用するよう変更 ( PR [#1019](https://github.com/cwtickle/danoniplus/pull/1019) )
- ⭐ 譜面セレクター表示時のショートカットキー実装 ( PR [#1013](https://github.com/cwtickle/danoniplus/pull/1013) )
- ⭐ 矢印・フリーズアローモーションの20以上のキー対応 ( PR [#1020](https://github.com/cwtickle/danoniplus/pull/1020) )
- 🛠️ 非推奨関数を danoni_legacy_function.js へ移動 ( PR [#1017](https://github.com/cwtickle/danoniplus/pull/1017) )
- 🛠️ 譜面セレクター表示時、Difficulty設定、各画面移動以外の隠れているボタンに対する
ショートカットキーを無効化 ( PR [#1013](https://github.com/cwtickle/danoniplus/pull/1013) )
- 🛠️ キーコンフィグ画面の影矢印部分がColorTypeの変化に対応するよう変更 ( PR [#1013](https://github.com/cwtickle/danoniplus/pull/1013) )
- 🛠️ キーコンフィグ画面、レベル計算ツール周りのコード整理 ( PR [#1016](https://github.com/cwtickle/danoniplus/pull/1016), [#1018](https://github.com/cwtickle/danoniplus/pull/1018), [#1021](https://github.com/cwtickle/danoniplus/pull/1021) )

 | **v21** | [**v20 ->**](Changelog-v20.html)
