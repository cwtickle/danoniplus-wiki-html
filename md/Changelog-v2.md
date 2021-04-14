⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

[**<- v3**](Changelog-v3.html) | **v2** | [**v1 ->**](Changelog-v1.html)

## [Warning] 更新終了後の不具合情報
- [更新を終了したバージョンの不具合情報#v2](DeprecatedVersionBugs.html#v2) を参照

## v2.9.11 ([2019-05-31](https://github.com/cwtickle/danoniplus/releases/tag/v2.9.11))
- 🐞 判定基準位置が1フレーム手前になっている問題を修正 ( PR [#318](https://github.com/cwtickle/danoniplus/pull/318), [#323](https://github.com/cwtickle/danoniplus/pull/323) ) <- :boom: **initial**

## v2.9.7 ([2019-05-21](https://github.com/cwtickle/danoniplus/releases/tag/v2.9.7))
- 🐞 back_dataのフレーム数が小さすぎる場合に画面が止まる問題を修正 ( PR [#305](https://github.com/cwtickle/danoniplus/pull/305) ) <- :boom: [**v2.4.0**](Changelog-v2.html#v240-2019-02-08) 

## v2.9.6 ([2019-05-11](https://github.com/cwtickle/danoniplus/releases/tag/v2.9.6))
- 🐞 ライフ回復・ダメージ量計算でフリーズアローのカウントが間違っていたのを修正 ( PR [#284](https://github.com/cwtickle/danoniplus/pull/284) ) <- :boom: [**v0.72.x**](Changelog-v0.html#v072x-2018-11-20)

## v2.9.5 ([2019-04-27](https://github.com/cwtickle/danoniplus/releases/tag/v2.9.5))
- 🛠️ back_dataでX/Y座標の整数値制限を緩和（小数が使えるように）( PR [#254](https://github.com/cwtickle/danoniplus/pull/254) ) 
- 🐞 back_dataでOpacityが機能していない問題を修正 ( PR [#254](https://github.com/cwtickle/danoniplus/pull/254) ) <- :boom: [**v0.65.x**](Changelog-v0.html#v065x-2018-11-16)

## v2.9.4 ([2019-04-21](https://github.com/cwtickle/danoniplus/releases/tag/v2.9.4))
- 🐞 ローディング100%で数秒止まる問題の修正 ( PR [#217](https://github.com/cwtickle/danoniplus/pull/217) ) <- :boom: [**v2.9.2**](Changelog-v2.html#v292-2019-02-25)
- 🐞 画像ファイル読込(preloadImages)時にjsエラーになる問題を修正 ( PR [#244](https://github.com/cwtickle/danoniplus/pull/244) ) <- :boom: [**v0.67.x**](Changelog-v0.html#v067x-2018-11-17)

----

## v2.9.3 ([2019-02-25](https://github.com/cwtickle/danoniplus/releases/tag/v2.9.3))
- 🛠️ 共通系関数のIE特殊対応を削除 ( PR [#213](https://github.com/cwtickle/danoniplus/pull/213) )

## v2.9.2 ([2019-02-25](https://github.com/cwtickle/danoniplus/releases/tag/v2.9.2))
- 🐞 Web上で、曲時間がNaNになることがある不具合を修正 ( PR [#208](https://github.com/cwtickle/danoniplus/pull/208) ) <- :boom: [**v2.6.0**](Changelog-v2.html#v260-2019-02-10)

## v2.9.1 ([2019-02-21](https://github.com/cwtickle/danoniplus/releases/tag/v2.9.1))
- 🐞 back_data利用時、フレーム計算が失敗しエラーとなる問題を修正 ( PR [#207](https://github.com/cwtickle/danoniplus/pull/207) ) <- :boom: [**v2.8.0**](Changelog-v2.html#v280-2019-02-17)

## v2.9.0 ([2019-02-17](https://github.com/cwtickle/danoniplus/releases/tag/v2.9.0))
- ⭐️ ロード画面をカスタムできるように変更 ( PR [#203](https://github.com/cwtickle/danoniplus/pull/203) )

## v2.8.1 ([2019-02-17](https://github.com/cwtickle/danoniplus/releases/tag/v2.8.1))
- 🐞 再生速度変更時のフェードアウト動作の修正 ( PR [#201](https://github.com/cwtickle/danoniplus/pull/201) ) <- :boom: [**v2.8.0**](Changelog-v2.html#v280-2019-02-17)

## v2.8.0 ([2019-02-17](https://github.com/cwtickle/danoniplus/releases/tag/v2.8.0))
- ⭐️ 譜面ヘッダーで曲の再生速度を指定できるように変更 ( PR [#199](https://github.com/cwtickle/danoniplus/pull/199) ) 
- ⭐️ ソース更新年を表記するように変更

## v2.7.1 ([2019-02-16](https://github.com/cwtickle/danoniplus/releases/tag/v2.7.1))
- 🛠️ Firefoxかつローカル環境のとき、非推奨として表示するように変更 ( PR [#198](https://github.com/cwtickle/danoniplus/pull/198) )
- 🐞 楽曲再生前に処理落ち（ブラウザを非アクティブにした場合を含む）すると譜面がずれる問題の修正 ( PR [#197](https://github.com/cwtickle/danoniplus/pull/197) ) <- :boom: [**v0.73.x**](Changelog-v0.html#v073x-2018-11-20)

## v2.7.0 ([2019-02-15](https://github.com/cwtickle/danoniplus/releases/tag/v2.7.0))
- 🛠️ 可能な場合にWebAudioAPIで楽曲を再生するように変更 ( PR [#195](https://github.com/cwtickle/danoniplus/pull/195) )

## v2.6.1 ([2019-02-12](https://github.com/cwtickle/danoniplus/releases/tag/v2.6.1))
- 🐞 フェードイン時間がblankFrameより小さい時にタイミングがずれる問題を修正 ( PR [#192](https://github.com/cwtickle/danoniplus/pull/192) ) <- :boom: [**v0.63.x**](Changelog-v0.html#v063x-2018-11-13)

## v2.6.0 ([2019-02-10](https://github.com/cwtickle/danoniplus/releases/tag/v2.6.0))
- ⭐️ ロード画面の実装 ( PR [#190](https://github.com/cwtickle/danoniplus/pull/190) )

## v2.5.3 ([2019-02-09](https://github.com/cwtickle/danoniplus/releases/tag/v2.5.3))
- 🛠️ フェードインのスライダー処理の記述方法変更 ( PR [#189](https://github.com/cwtickle/danoniplus/pull/189) )

## v2.5.2 ([2019-02-09](https://github.com/cwtickle/danoniplus/releases/tag/v2.5.2))
- 🐞 ランクがPF/F/X以外のとき、リザルト画面に遷移できない不具合を修正 ( PR [#187](https://github.com/cwtickle/danoniplus/pull/187) ) <- :boom: [**v2.4.0**](Changelog-v2.html#v240-2019-02-08)

## v2.5.1 ([2019-02-09](https://github.com/cwtickle/danoniplus/releases/tag/v2.5.1))
- 🐞 フェードインのスライダー処理の不具合を修正 <- :boom: [**v2.4.0**](Changelog-v2.html#v240-2019-02-08)

## v2.5.0 ([2019-02-08](https://github.com/cwtickle/danoniplus/releases/tag/v2.5.0))
- ⭐️ 譜面データ（外部ファイル）の文字コードを指定できるように変更 ( PR [#180](https://github.com/cwtickle/danoniplus/pull/180) )

## v2.4.0 ([2019-02-08](https://github.com/cwtickle/danoniplus/releases/tag/v2.4.0))
- 🛠️ コード記述の見直し（IE11依存の記述見直し）( PR [#178](https://github.com/cwtickle/danoniplus/pull/178) )

## v2.3.0 ([2019-02-06](https://github.com/cwtickle/danoniplus/releases/tag/v2.3.0))
- ⭐️ 譜面データの外部ファイル化に対応 ( PR [#174](https://github.com/cwtickle/danoniplus/pull/174), Issue [#145](https://github.com/cwtickle/danoniplus/pull/145) )

## v2.2.0 ([2019-02-05](https://github.com/cwtickle/danoniplus/releases/tag/v2.2.0))
- ⭐️ 譜面ヘッダーにて、譜面別に（製作者側が）タイミング調整できるように変更 ( PR [#173](https://github.com/cwtickle/danoniplus/pull/173) )

## v2.1.2 ([2019-01-24](https://github.com/cwtickle/danoniplus/releases/tag/v2.1.2))
- 🐞 メインのReady?表示が表示されない不具合を修正 ( PR [#171](https://github.com/cwtickle/danoniplus/pull/171) ) <- :boom: [**v2.1.0**](Changelog-v2.html#v210-2019-01-24)

## v2.1.1 ([2019-01-24](https://github.com/cwtickle/danoniplus/releases/tag/v2.1.1))
- 🐞 デフォルト背景が前に見えてしまう不具合を修正 ( PR [#170](https://github.com/cwtickle/danoniplus/pull/170) ) <- :boom: [**v2.1.0**](Changelog-v2.html#v210-2019-01-24)

## v2.1.0 ([2019-01-24](https://github.com/cwtickle/danoniplus/releases/tag/v2.1.0))
- ⭐️ （デフォルト）タイトル文字・矢印及び背景をmain側に移植 ( PR [#169](https://github.com/cwtickle/danoniplus/pull/169) )
- ⭐️ タイトル文字のフォント設定に対応 ( PR [#169](https://github.com/cwtickle/danoniplus/pull/169) )

## v2.0.2 ([2019-01-24](https://github.com/cwtickle/danoniplus/releases/tag/v2.0.2))
- 🐞 フェードアウト中にリザルト画面へ移行させた場合の音量不具合を修正 ( PR [#167](https://github.com/cwtickle/danoniplus/pull/167) ) <- :boom: **initial**
- 🐞 初期ライフ量が常に整数値になるように修正 ( PR [#167](https://github.com/cwtickle/danoniplus/pull/167) ) <- :boom: **initial**

## v2.0.1 ([2019-01-19](https://github.com/cwtickle/danoniplus/releases/tag/v2.0.1))
- 🛠️ IE11の非対応化に伴うコード修正 ( PR [#166](https://github.com/cwtickle/danoniplus/pull/166) )

## v2.0.0 ([2019-01-18](https://github.com/cwtickle/danoniplus/releases/tag/v2.0.0))
- 🛠️ テンプレート文字列を使用するように変更 ( PR [#162](https://github.com/cwtickle/danoniplus/pull/162), [#163](https://github.com/cwtickle/danoniplus/pull/163) )

[**<- v3**](Changelog-v3.html) | **v2** | [**v1 ->**](Changelog-v1.html)
