⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

[**<- v2**](Changelog-v2.html) | **v1** | [**v0 ->**](Changelog-v0.html)

## [Warning] 更新終了後の不具合情報
- [更新を終了したバージョンの不具合情報#v1](DeprecatedVersionBugs.html#v1) を参照

## v1.15.17 ([2019-10-08](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.17))
- 🐞 速度変化が同一フレームにあると正常に動作しなくなる不具合を修正 ( PR [#477](https://github.com/cwtickle/danoniplus/pull/477) ) <- :boom: **initial**

## v1.15.16 ([2019-10-06](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.16))
- 🐞 エスケープ文字の適用順序誤りを修正 ( PR [#472](https://github.com/cwtickle/danoniplus/pull/472), [#473](https://github.com/cwtickle/danoniplus/pull/473) ) <- :boom: [**v0.66.x**](Changelog-v0.html#v066x-2018-11-16)

## v1.15.15 ([2019-09-23](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.15))
- 🐞 ロード画面でEnterを押すと複数回ロードが発生する問題を修正 ( PR [#432](https://github.com/cwtickle/danoniplus/pull/432) ) <- :boom: **initial**
- 🐞 メイン画面で曲中リトライキーを連打した場合に譜面がずれることがある問題を修正 ( PR [#433](https://github.com/cwtickle/danoniplus/pull/433) ) <- :boom: **initial**

## v1.15.14 ([2019-09-16](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.14))
- 🐞 ゲームオーバー時の200ミリ秒遅延により、ハイスコア表示がおかしくなることがある問題を修正 ( PR [#428](https://github.com/cwtickle/danoniplus/pull/428) ) <- :boom: **initial**

## v1.15.13 ([2019-09-15](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.13))
- 🐞 速度変化が補正込みで負のフレームにあるときの不具合を修正 ( PR [#426](https://github.com/cwtickle/danoniplus/pull/426) ) <- :boom: **initial**

## v1.15.12 ([2019-08-03](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.12))
- 🐞 back_dataで0フレームが指定された場合に動作しないことがある問題を修正 ( PR [#388](https://github.com/cwtickle/danoniplus/pull/388) ) <- :boom: [**v0.65.x**](Changelog-v0.html#v065x-2018-11-16)

## v1.15.11 ([2019-07-21](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.11))
- 🐞 リザルト画面で、フェードアウト中にTitleBack/Retryするとフェードアウト状態が引き継がれてしまう問題を修正 ( PR [#384](https://github.com/cwtickle/danoniplus/pull/384) ) <- :boom: [**v0.68.x**](Changelog-v0.html#v068x-2018-11-17)

## v1.15.10 ([2019-07-06](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.10))
- 🐞 フェードイン時に個別加速が掛からない問題を修正 ( PR [#363](https://github.com/cwtickle/danoniplus/pull/363) ) <- :boom: **initial**

## v1.15.9 ([2019-06-18](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.9))
- 🛠️ フリーズアローの枠外判定の修正・見直し（条件により止まってしまう問題の修正）( PR [#341](https://github.com/cwtickle/danoniplus/pull/341) )
- 🐞 フリーズアローのみの譜面が再生できない問題を修正 ( PR [#343](https://github.com/cwtickle/danoniplus/pull/343) ) <- :boom: **initial**

## v1.15.8 ([2019-05-31](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.8))
- 🐞 判定基準位置が1フレーム手前になっている問題を修正 ( PR [#318](https://github.com/cwtickle/danoniplus/pull/318), [#323](https://github.com/cwtickle/danoniplus/pull/323) ) <- :boom: **initial**

## v1.15.4 ([2019-05-11](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.4))
- 🐞 ライフ回復・ダメージ量計算でフリーズアローのカウントが間違っていたのを修正 ( PR [#284](https://github.com/cwtickle/danoniplus/pull/284) ) <- :boom: [**v0.72.x**](Changelog-v0.html#v072x-2018-11-20)

## v1.15.3 ([2019-04-27](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.3))
- 🛠️ back_dataでX/Y座標の整数値制限を緩和（小数が使えるように）( PR [#254](https://github.com/cwtickle/danoniplus/pull/254) ) 
- 🐞 back_dataでOpacityが機能していない問題を修正 ( PR [#254](https://github.com/cwtickle/danoniplus/pull/254) ) <- :boom: [**v0.65.x**](Changelog-v0.html#v065x-2018-11-16)

## v1.15.2 ([2019-02-12](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.2))
- 🐞 フェードイン時間がblankFrameより小さい時にタイミングがずれる問題を修正 ( PR [#192](https://github.com/cwtickle/danoniplus/pull/192) ) <- :boom: [**v0.63.x**](Changelog-v0.html#v063x-2018-11-13)

## v1.15.1 ([2019-01-24](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.1))
- 🐞 フェードアウト中にリザルト画面へ移行させた場合の音量不具合を修正 ( PR [#167](https://github.com/cwtickle/danoniplus/pull/167) ) <- :boom: **initial**
- 🐞 初期ライフ量が常に整数値になるように修正 ( PR [#167](https://github.com/cwtickle/danoniplus/pull/167) ) <- :boom: **initial**

----

## v1.15.0 ([2019-01-14](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.0))
- ⭐️ フルコンボ演出の表示切替を譜面側から行えるように変更 (finishView=none) ( PR [#161](https://github.com/cwtickle/danoniplus/pull/161) )

## v1.14.0 ([2019-01-12](https://github.com/cwtickle/danoniplus/releases/tag/v1.14.0))
- ⭐️ ステップゾーン間隔を譜面側から設定できるように変更 (blankX) ( PR [#160](https://github.com/cwtickle/danoniplus/pull/160) )
- ⭐️ 5key, 9A/9Bkeyのステップゾーン間隔のデフォルトを変更（5keyは広く、9A/9Bkeyは狭く） ( PR [#160](https://github.com/cwtickle/danoniplus/pull/160) ) 
- ⭐️ 既存キーに対して各種キー設定の上書きを可能に変更 ( PR [#160](https://github.com/cwtickle/danoniplus/pull/160) ) 

## v1.13.0 ([2019-01-06](https://github.com/cwtickle/danoniplus/releases/tag/v1.13.0))
- ⭐️ 判定名をカスタムできるように変更 ( PR [#158](https://github.com/cwtickle/danoniplus/pull/158) ) 
- ⭐️ リザルト画面の右上のクリアマークについて、パーフェクト・フルコンボの表記ができるよう変更 ( PR [#158](https://github.com/cwtickle/danoniplus/pull/158) )

## v1.12.1 ([2019-01-05](https://github.com/cwtickle/danoniplus/releases/tag/v1.12.1))
- 🛠️ 外部jsファイルの乱数制御方法変更（乱数→時刻制御）( PR [#157](https://github.com/cwtickle/danoniplus/pull/157) ) 
- 🛠️ Tweetスコアの表示変数変更（ローカル変数→グローバル変数）( PR [#157](https://github.com/cwtickle/danoniplus/pull/157) )

## v1.12.0 ([2019-01-04](https://github.com/cwtickle/danoniplus/releases/tag/v1.12.0))
- ⭐️ タイトル文字以外のフォントを設定できるように変更 ( PR [#156](https://github.com/cwtickle/danoniplus/pull/156), Issue [#124](https://github.com/cwtickle/danoniplus/pull/124) ) 
  - 譜面データ内：customFont にて設定（既定：Meiryo UI）
- ⭐️ 外部jsファイルのキャッシュを利用しないように変更 ( PR [#156](https://github.com/cwtickle/danoniplus/pull/156) )

## v1.11.1 ([2019-01-03](https://github.com/cwtickle/danoniplus/releases/tag/v1.11.1))
- 🐞 Adjustmentがマイナス値のとき、曲終了時間が短くなる問題を修正 ( PR [#155](https://github.com/cwtickle/danoniplus/pull/155) ) <- :boom: **initial**

## v1.11.0 ([2019-01-02](https://github.com/cwtickle/danoniplus/releases/tag/v1.11.0))
- ⭐️ 判定処理のカスタム処理を分離 ( PR [#154](https://github.com/cwtickle/danoniplus/pull/154), Issue [#151](https://github.com/cwtickle/danoniplus/pull/151) ) 
- ⭐️ ライフ表示について、小数点切り捨てで表示するように変更 ( PR [#154](https://github.com/cwtickle/danoniplus/pull/154), Issue [#150](https://github.com/cwtickle/danoniplus/pull/150) - 2 ) 
- ⭐️ ライフのボーダーラインに使用するフォントサイズをjs側で指定 ( PR [#154](https://github.com/cwtickle/danoniplus/pull/154), Issue [#150](https://github.com/cwtickle/danoniplus/pull/150) - 3 )

## v1.10.1 ([2019-01-01](https://github.com/cwtickle/danoniplus/releases/tag/v1.10.1))
- 🐞 歌詞表示(追加分)についてフェードイン・アウトが利いていない問題を修正 ( PR [#153](https://github.com/cwtickle/danoniplus/pull/153) ) <- :boom: **initial**

## v1.10.0 ([2018-12-30](https://github.com/cwtickle/danoniplus/releases/tag/v1.10.0))
- ⭐️ 曲終了フレーム(endFrame)について、譜面別に指定できるように変更 ( PR [#149](https://github.com/cwtickle/danoniplus/pull/149) )

## v1.9.0 ([2018-12-30](https://github.com/cwtickle/danoniplus/releases/tag/v1.9.0))
- ⭐️ 歌詞表示で、左揃え/中央揃え/右揃えの設定を可能に変更 ( PR [#148](https://github.com/cwtickle/danoniplus/pull/148) ) 
  - word_dataのキーワード指定でそれぞれ、[left][center][right]とすると変更が可能
- ⭐️ 歌詞表示種類を2から4に拡大 
- ⭐️ 歌詞表示位置を中央にするために、歌詞表示サイズを変更 (横幅 - 200px)

## v1.8.0 ([2018-12-25](https://github.com/cwtickle/danoniplus/releases/tag/v1.8.0))
- ⭐️ Tweet内容にPlaystyle (Speed, Motion, Reverse, Gaugeの変更状況)を表示するように変更 ( PR [#144](https://github.com/cwtickle/danoniplus/pull/144) )

## v1.7.1 ([2018-12-24](https://github.com/cwtickle/danoniplus/releases/tag/v1.7.1))
- 🛠️ 音楽ファイルとして、base64変換したmp3データ(jsファイル, txtファイル)を指定できるように変更 ( PR [#143](https://github.com/cwtickle/danoniplus/pull/143) )

## v1.7.0 ([2018-12-24](https://github.com/cwtickle/danoniplus/releases/tag/v1.7.0))
- ⭐️ 音楽ファイルとして、base64変換したmp3データ(jsファイル)を指定できるように変更 ( PR [#140](https://github.com/cwtickle/danoniplus/pull/140) )

## v1.6.0 ([2018-12-23](https://github.com/cwtickle/danoniplus/releases/tag/v1.6.0))
- ⭐️ ゲージ設定の名称変更（Borderless→Original）( PR [#138](https://github.com/cwtickle/danoniplus/pull/138) )  
- ⭐️ ゲージ設定「Light」の既定を見直し（ダメージ半減 → 回復量2倍）( PR [#138](https://github.com/cwtickle/danoniplus/pull/138) )

## v1.5.1 ([2018-12-23](https://github.com/cwtickle/danoniplus/releases/tag/v1.5.1))
- 🐞 SuddenDeathで1ミスFailedにならない場合がある問題を修正 ( PR [#132](https://github.com/cwtickle/danoniplus/pull/132) ) <- :boom: [**v1.5.0**](Changelog-v1.html#v150-2018-12-23)

## v1.5.0 ([2018-12-23](https://github.com/cwtickle/danoniplus/releases/tag/v1.5.0))
- ⭐️ 設定のGaugeに「Easy」「Hard」（ノルマ制の場合）、「Light」（ライフ制の場合）を追加 ( PR [#130](https://github.com/cwtickle/danoniplus/pull/130) ) 
- ⭐️ ノルマ制オプション（Normal, Easy, Hard）に対して、個別にノルマ・回復・ダメージ・初期ライフを設定可能な変数を追加 
- ⭐️ Gaugeオプションにおいて、初期ライフ(Init)の表記を追加 
- ⭐️ Gaugeオプションにおいて、ノルマ(Border)の表記をパーセントから実ライフ値に変更 
- ⭐️ ノルマ(Border)を0にした場合、ライフが空のときに途中終了する仕様に変更 (Hardゲージ実装に合わせ)

## v1.4.0 ([2018-12-13](https://github.com/cwtickle/danoniplus/releases/tag/v1.4.0))
- 🛠️ コード記述の見直し (機能変更なし) 
  - 厳密等価演算子 === と !== を使うように変更 ( PR [#126](https://github.com/cwtickle/danoniplus/pull/126) )
  - 真偽値の比較に等価演算子を使わないように変更 ( PR [#126](https://github.com/cwtickle/danoniplus/pull/126) )
  - 設定画面のSpeed, Adjustmentの上限・下限値の直接指定を見直し ( PR [#127](https://github.com/cwtickle/danoniplus/pull/127) )

## v1.3.0 ([2018-12-11](https://github.com/cwtickle/danoniplus/releases/tag/v1.3.0))
- ⭐️ フリーズアローのヒット時のデフォルト色を変更 ( PR [#125](https://github.com/cwtickle/danoniplus/pull/125) )
- ⭐️ ゲージ設定に「Practice」を追加 (ライフ制選択時)  ( PR [#125](https://github.com/cwtickle/danoniplus/pull/125) ) 
- 🛠️ キーコンフィグのカーソル移動をアニメーション化 ( PR [#125](https://github.com/cwtickle/danoniplus/pull/125) )
- 🛠️ 譜面名の文字サイズ調整 (譜面名が長い場合に自動で文字を縮小) ( PR [#125](https://github.com/cwtickle/danoniplus/pull/125) )

## v1.2.0 ([2018-12-04](https://github.com/cwtickle/danoniplus/releases/tag/v1.2.0))
- ⭐️ タイトルにリロードボタンを追加 (左上の「R」ボタン) ( PR [#120](https://github.com/cwtickle/danoniplus/pull/120) )
- ⭐️ danoni_custom.js にローカルバージョンを指定することでタイトル右下のバージョンに補記できるように変更 ( PR [#120](https://github.com/cwtickle/danoniplus/pull/120) )
- 🛠️ 一部オブジェクトで、zIndex指定されていた個所を削除 ( PR [#120](https://github.com/cwtickle/danoniplus/pull/120) )

## v1.1.4 ([2018-12-03](https://github.com/cwtickle/danoniplus/releases/tag/v1.1.4))
- 🛠️ 曲時間表示の位置を修正 (10分以上の表示に対応) ( PR [#118](https://github.com/cwtickle/danoniplus/pull/118) )
- 🐞 独自キーの変数posXが数値ではなく文字列として取り込まれていた不具合を修正 ( PR [#119](https://github.com/cwtickle/danoniplus/pull/119) ) <- :boom: **initial**

## v1.1.3 ([2018-12-02](https://github.com/cwtickle/danoniplus/releases/tag/v1.1.3))
- 🛠️ Firefoxアクセス時の非推奨マークを削除 ( PR [#117](https://github.com/cwtickle/danoniplus/pull/117) )
- 🐞 Firefoxで楽曲が遅れて再生されることがある問題を修正 ( PR [#117](https://github.com/cwtickle/danoniplus/pull/117) ) <- :boom: **initial**

## v1.1.2 ([2018-12-02](https://github.com/cwtickle/danoniplus/releases/tag/v1.1.2))
- 🐞 個別加速(boost_data)のみ、譜面やSpeed:OFFしてもデータリセットされない問題を修正 ( PR [#116](https://github.com/cwtickle/danoniplus/pull/116) ) <- :boom: **initial**

## v1.1.1 ([2018-12-02](https://github.com/cwtickle/danoniplus/releases/tag/v1.1.1))
- 🐞 フリーズアローヒット時に後続矢印位置が補正されない問題を修正 ( PR [#115](https://github.com/cwtickle/danoniplus/pull/115) ) <- :boom: [**v1.0.2**](Changelog-v1.html#v102-2018-11-27)

## v1.1.0 ([2018-12-01](https://github.com/cwtickle/danoniplus/releases/tag/v1.1.0))
- ⭐️ Edge V18以降で初期矢印色及び色変化に対応 ( PR [#114](https://github.com/cwtickle/danoniplus/pull/114) )
- 🐞 曲時間直指定時、終了時間指定がおかしくなることがある不具合を修正 ( PR [#114](https://github.com/cwtickle/danoniplus/pull/114) ) <- :boom: **initial**

## v1.0.2 ([2018-11-27](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.2))
- 🛠️ フリーズアローのヒット開始位置をステップゾーン上になるように位置調整 ( PR [#112](https://github.com/cwtickle/danoniplus/pull/112) )
- 🛠️ ゲージ設定で、ノルマ必須の場合のBorder表記を%表記に変更 ( PR [#112](https://github.com/cwtickle/danoniplus/pull/112) )
- 🐞 譜面変更ボタンを変更した場合に、ゲージ設定がリセットされないことがある問題を修正 ( PR [#112](https://github.com/cwtickle/danoniplus/pull/112) ) <- :boom: **initial**

## v1.0.1 ([2018-11-25](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1))
- 🛠️ ローカル時のみフレーム数を表示する仕様に変更 ( PR [#111](https://github.com/cwtickle/danoniplus/pull/111) )
- 🐞 デフォルトのゲージ設定がBorderlessになっていない問題を修正 ( PR [#111](https://github.com/cwtickle/danoniplus/pull/111) ) <- :boom: **initial**

## v1.0.0 ([2018-11-25](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1))
- ⭐️ Clear, Failed条件及び結果画面のモーションを追加 ( PR [#109](https://github.com/cwtickle/danoniplus/pull/109) )
- ⭐️ Gaugeオプションの実装 ( PR [#109](https://github.com/cwtickle/danoniplus/pull/109) )
- 🐞 IE11でゲーム開始直後に止まる問題を修正 ( PR [#108](https://github.com/cwtickle/danoniplus/pull/108) ) <- :boom: **initial**

[**<- v2**](Changelog-v2.html) | **v1** | [**v0 ->**](Changelog-v0.html)
