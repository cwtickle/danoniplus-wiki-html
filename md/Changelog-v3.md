⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

[**<- v4**](Changelog-v4.html) | **v3** | [**v2 ->**](Changelog-v2.html)

## [Warning] 更新終了後の不具合情報
- [更新を終了したバージョンの不具合情報#v3](DeprecatedVersionBugs.html#v3) を参照

## v3.13.9 ([2019-05-31](https://github.com/cwtickle/danoniplus/releases/tag/v3.13.9))
- 🐞 判定基準位置が1フレーム手前になっている問題を修正 ( PR [#318](https://github.com/cwtickle/danoniplus/pull/318), [#323](https://github.com/cwtickle/danoniplus/pull/323) ) <- :boom: **initial**

## v3.13.5 ([2019-05-26](https://github.com/cwtickle/danoniplus/releases/tag/v3.13.5))
- 🐞 譜面ヘッダー：titlesizeを64以上に指定すると文字欠けが起こる問題を修正 ( PR [#308](https://github.com/cwtickle/danoniplus/pull/308) ) <- :boom: [**v3.5.0**](Changelog-v3.html#v350-2019-03-23)

## v3.13.4 ([2019-05-21](https://github.com/cwtickle/danoniplus/releases/tag/v3.13.4))
- 🐞 back_dataのフレーム数が小さすぎる場合に画面が止まる問題を修正 ( PR [#305](https://github.com/cwtickle/danoniplus/pull/305) ) <- :boom: [**v2.4.0**](Changelog-v2.html#v240-2019-02-08) 

## v3.13.3 ([2019-05-11](https://github.com/cwtickle/danoniplus/releases/tag/v3.13.3))
- 🐞 ライフ回復・ダメージ量計算でフリーズアローのカウントが間違っていたのを修正 ( PR [#284](https://github.com/cwtickle/danoniplus/pull/284) ) <- :boom: [**v0.72.x**](Changelog-v0.html#v072x-2018-11-20)

## v3.13.2 ([2019-04-27](https://github.com/cwtickle/danoniplus/releases/tag/v3.13.2))
- 🛠️ back_dataでX/Y座標の整数値制限を緩和（小数が使えるように）( PR [#254](https://github.com/cwtickle/danoniplus/pull/254) ) 
- 🐞 back_dataでOpacityが機能していない問題を修正 ( PR [#254](https://github.com/cwtickle/danoniplus/pull/254) ) <- :boom: [**v0.65.x**](Changelog-v0.html#v065x-2018-11-16)

----

## v3.13.1 ([2019-04-21](https://github.com/cwtickle/danoniplus/releases/tag/v3.13.1))
- 🐞 startFrameが指定されないときにプレイ画面で止まる問題を修正 ( PR [#250](https://github.com/cwtickle/danoniplus/pull/250) ) <- :boom: [**v3.11.0**](Changelog-v3.html#v3110-2019-04-17)

## v3.13.0 ([2019-04-21](https://github.com/cwtickle/danoniplus/releases/tag/v3.13.0))
- 🛠️ ColorTypeがDefault以外の場合、Display:ColorをOFFにするよう修正 ( PR [#247](https://github.com/cwtickle/danoniplus/pull/247) )

## v3.12.0 ([2019-04-21](https://github.com/cwtickle/danoniplus/releases/tag/v3.12.0))
- ⭐️ キーコンフィグ画面で作品毎の矢印色ではない、
共通デフォルト色を指定できるように変更 (ColorTypeの追加) ( PR [#245](https://github.com/cwtickle/danoniplus/pull/245) )

## v3.11.1 ([2019-04-17](https://github.com/cwtickle/danoniplus/releases/tag/v3.11.1))
- 🐞 画像ファイル読込(preloadImages)時にjsエラーになる問題を修正 ( PR [#244](https://github.com/cwtickle/danoniplus/pull/244) ) <- :boom: [**v0.67.x**](Changelog-v0.html#v067x-2018-11-17)

## v3.11.0 ([2019-04-17](https://github.com/cwtickle/danoniplus/releases/tag/v3.11.0))
- ⭐️ 全ての矢印を判定させていれば、フェードイン位置によらずクリアと見做すように変更 ( PR [#242](https://github.com/cwtickle/danoniplus/pull/242) ) 
- ⭐️ 譜面ヘッダー「startFrame」について、譜面毎に設定できるように変更 ( PR [#242](https://github.com/cwtickle/danoniplus/pull/242) )

## v3.10.0 ([2019-04-17](https://github.com/cwtickle/danoniplus/releases/tag/v3.10.0))
- ⭐️ 複数譜面で歌詞表示（wordX_data）が無い場合、自動的に1譜面目のword_dataも見るように変更 ( PR [#240](https://github.com/cwtickle/danoniplus/pull/240) ) 
- ⭐️ 速度変化、色変化、歌詞表示のセット毎改行区切りに対応 ( PR [#240](https://github.com/cwtickle/danoniplus/pull/240) )

## v3.9.0 ([2019-04-14](https://github.com/cwtickle/danoniplus/releases/tag/v3.9.0))
- ⭐️ パターン付きのキー指定（DP, 9A-2など）を自動修正するように変更 ( PR [#238](https://github.com/cwtickle/danoniplus/pull/238) ) 
- ⭐️ CSSモーションパターンを追加し、デフォルトの曲名表示に対してモーションを指定 ( PR [#239](https://github.com/cwtickle/danoniplus/pull/239) )

## v3.8.0 ([2019-04-13](https://github.com/cwtickle/danoniplus/releases/tag/v3.8.0))
- 🛠️ タイトル画面のカスタム部分の表示深度が手前になるように変更 ( PR [#237](https://github.com/cwtickle/danoniplus/pull/237) )

## v3.7.0 ([2019-04-06](https://github.com/cwtickle/danoniplus/releases/tag/v3.7.0))
- 🛠️ カスタムデザイン（背景）の使用について、メインとそれ以外で設定を分離 ( PR [#234](https://github.com/cwtickle/danoniplus/pull/234) )

## v3.6.0 ([2019-04-03](https://github.com/cwtickle/danoniplus/releases/tag/v3.6.0))
- ⭐️ 設定ファイル ( danoni_setting.js )のデフォルト値を指定 ( PR [#232](https://github.com/cwtickle/danoniplus/pull/232) ) 
- ⭐️ カスタムデザインの有無を設定ファイルで一律指定できるように変更 ( PR [#232](https://github.com/cwtickle/danoniplus/pull/232) )
- 🐞 総ノート数が0のときスコアがNaNになる不具合の修正 <- :boom: **initial**

## v3.5.0 ([2019-03-23](https://github.com/cwtickle/danoniplus/releases/tag/v3.5.0))
- ⭐️ 曲名タイトル（デフォルト）の複数行対応 ( PR [#229](https://github.com/cwtickle/danoniplus/pull/229) )

## v3.4.0 ([2019-03-22](https://github.com/cwtickle/danoniplus/releases/tag/v3.4.0))
- 🛠️ 矢印毎にスクロール情報を保持するように変更 ( PR [#228](https://github.com/cwtickle/danoniplus/pull/228) )

## v3.3.1 ([2019-03-16](https://github.com/cwtickle/danoniplus/releases/tag/v3.3.1))
- 🐞 12, 14key(Type1)のキーコンフィグ間違いを修正 ( PR [#227](https://github.com/cwtickle/danoniplus/pull/227) ) <- :boom: **initial**

## v3.3.0 ([2019-03-15](https://github.com/cwtickle/danoniplus/releases/tag/v3.3.0))
- 🛠️ 17keyのデフォルト配置を横一列に変更 ( PR [#226](https://github.com/cwtickle/danoniplus/pull/226) )  
- 🛠️ Displayオプションのデザイン変更 ( PR [#225](https://github.com/cwtickle/danoniplus/pull/225) )

## v3.2.0 ([2019-03-12](https://github.com/cwtickle/danoniplus/releases/tag/v3.2.0))
- ⭐️ タイトル画面の曲名にWebフォントが使用できるように変更 ( PR [#223](https://github.com/cwtickle/danoniplus/pull/223) ) 
- ⭐️ 曲名のグラデーション対応 ( PR [#223](https://github.com/cwtickle/danoniplus/pull/223) )

## v3.1.4 ([2019-03-01](https://github.com/cwtickle/danoniplus/releases/tag/v3.1.4))
- 🐞 追加キー定義でシャッフルグループが正しく読み込めない問題の修正 ( PR [#222](https://github.com/cwtickle/danoniplus/pull/222) ) <- :boom: [**v3.1.0**](Changelog-v3.html#v310-2019-02-26)

## v3.1.3 ([2019-02-27](https://github.com/cwtickle/danoniplus/releases/tag/v3.1.3))
- 🐞 不正な歌詞データで画面が止まる不具合を修正 ( PR [#219](https://github.com/cwtickle/danoniplus/pull/219) ) <- :boom: [**v0.65.x**](Changelog-v0.html#v065x-2018-11-16)

## v3.1.2 ([2019-02-26](https://github.com/cwtickle/danoniplus/releases/tag/v3.1.2))
- 🐞 ローディング100%で数秒止まる問題の修正 ( PR [#217](https://github.com/cwtickle/danoniplus/pull/217) ) <- :boom: [**v2.9.2**](Changelog-v2.html#v292-2019-02-25)

## v3.1.1 ([2019-02-26](https://github.com/cwtickle/danoniplus/releases/tag/v3.1.1))
- 🛠️ Gaugeに対して製作者側で設定可否を指定できるように変更 ( PR [#212](https://github.com/cwtickle/danoniplus/pull/212) , [#216](https://github.com/cwtickle/danoniplus/pull/216) )

## v3.1.0 ([2019-02-26](https://github.com/cwtickle/danoniplus/releases/tag/v3.1.0))
- ⭐️ Shuffle機能（Mirror, Randomなど）を追加 ( PR [#209](https://github.com/cwtickle/danoniplus/pull/209) ) 
- ⭐️ Motion/Shuffle/AutoPlayに対して製作者側で設定可否を指定できるように変更 ( PR [#212](https://github.com/cwtickle/danoniplus/pull/212) )

## v3.0.0 ([2019-02-25](https://github.com/cwtickle/danoniplus/releases/tag/v3.0.0))
- 🛠️ 製作者別設定ファイルを追加 ( PR [#210](https://github.com/cwtickle/danoniplus/pull/210) )

[**<- v4**](Changelog-v4.html) | **v3** | [**v2 ->**](Changelog-v2.html)
