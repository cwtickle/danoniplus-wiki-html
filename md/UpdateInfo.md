# 更新情報 / UpdateInfo
- 新機能を中心にまとめています。
- 最新の情報は[Release](https://github.com/cwtickle/danoniplus/releases) もしくは Changelog(下記バージョン別リンク) をご利用ください。
- アップグレードについては[アップグレードガイド(Migration Guide)](MigrationGuide.html)もご覧ください。

## ⭐ v21 ([Changelog](Changelog-v21).html)
- 初期矢印・フリーズアロー色(setColor/frzColor)の**譜面別設定**実装
- 譜面分割＆譜面番号固定時、個別の譜面ファイル内に  
setColor/frzColor/setShadowColor/frzShadowColorの記述があれば、その値を採用するよう変更
- **譜面セレクター表示時**のショートカットキー実装
- 矢印・フリーズアローモーションの20以上のキー対応
- キーコンフィグ画面の影矢印部分がColorTypeの変化に対応するよう変更
- **譜面毎にカスタムゲージリスト**が作成できるように変更
- ゲージ個別設定（譜面ヘッダー）について、**譜面毎の分割記法**に対応
- カスタムゲージリストについて、ライフ制ゲージ/ノルマ制ゲージ/共通設定ファイルで  
指定のリストを設定できるよう変更
- 背景状況により**明暗用のカラーセットを使用**するよう変更
- 警告メッセージ群の管理方法を見直し
- 空スプライト作成処理を`createEmptySprite`関数へ移行
- キーコンフィグの対応キー箇所を**ボタンに変更**

### 💡 Feature Updates
- [**v21.4.2**](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.2) / [v21.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.3.0) / [**v21.2.0**](https://github.com/cwtickle/danoniplus/releases/tag/v21.2.0) / [**v21.1.0**](https://github.com/cwtickle/danoniplus/releases/tag/v21.1.0) / [**v21.0.0**](https://github.com/cwtickle/danoniplus/releases/tag/v21.0.0)

### 📔 Documentation
- [ゲーム内で使用できるショートカット](Shortcut.html)
- [オブジェクト一覧](ObjectReferenceIndex.html) ( [g_shortcutObj](obj-v0017-g_shortcutObj.html) / [g_gaugeOptionObj](obj-v0007-g_gaugeOptionObj.html) / [fuzzyListMatching](fnc-c0039-fuzzyListMatching.html) / [makeWarningWindow](fnc-c0013-makeWarningWindow.html) / [importCssFile](fnc-c0020-importCssFile.html) / [createEmptySprite](fnc-c0043-createEmptySprite.html) / [g_errMsgObj](obj-v0026-g_errMsgObj.html) )
- 譜面ヘッダー仕様 ( [customGauge](dos-h0053-customGauge.html) / [gaugeX](dos-h0022-gaugeX.html) / [setColor](dos-h0003-setColor.html) / [frzColor](dos-h0004-frzColor.html) / [setShadowColor](dos-h0041-setShadowColor.html) / [frzShadowColor](dos-h0062-frzShadowColor.html) / [backBright](dos-h0081-backBright.html) / [defaultColorgrd](dos-h0061-defaultColorgrd.html) )
- 譜面エフェクト仕様 ( [矢印・フリーズアローモーション](dos-e0005-motionData.html) )

## ⭐ v20 ([Changelog](Changelog-v20).html)
- ボタン処理を**画面移動系とそれ以外**に分離
- ボタンの割り込み処理を本体処理より前に挿入できるよう変更
- 右クリック操作の無いボタンに対して処理を追加できるように変更
- タイトル文字、譜面名の**フォントサイズ**の自動設定方法を改善
- ボタン・ショートカットキー有効化までのフレーム数設定を実装
- 11ikeyに方向表示が異なるキーパターンを追加
- 設定名、結果画面用の省略名を置き換える機能を実装
- タイトル画面、ロード画面(iOSのみ)のショートカットキーを追加

### 💡 Feature Updates
- [v20.5.1](https://github.com/cwtickle/danoniplus/releases/tag/v20.5.1) / [v20.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v20.4.0) / [**v20.3.1**](https://github.com/cwtickle/danoniplus/releases/tag/v20.3.1) / [**v20.2.0**](https://github.com/cwtickle/danoniplus/releases/tag/v20.2.0) / [v20.1.2](https://github.com/cwtickle/danoniplus/releases/tag/v20.1.2) / [**v20.0.0**](https://github.com/cwtickle/danoniplus/releases/tag/v20.0.0)

### 📔 Documentation
- [ゲーム内で使用できるショートカット](Shortcut.html)
- [共通設定ファイル仕様](dos_setting.html) - 設定名の上書き可否設定 (g_lblRenames)
- [オブジェクト一覧](ObjectReferenceIndex.html) ( [createCss2Button](fnc-c0004-createCss2Button.html) / [g_btnAddFunc / g_cxtAddFunc](obj-v0018-g_btnAddFunc.html) / [g_btnDeleteFlg / g_cxtDeleteFlg](obj-v0019-g_btnDeleteFlg.html) / [g_shortcutObj](obj-v0017-g_shortcutObj.html) / [g_btnWaitFrame](obj-v0020-g_btnWaitFrame.html) / [g_btnPatterns](obj-v0021-g_btnPatterns.html) / [g_lblNameObj / g_local_lblNameObj](obj-v0015-g_lblNameObj.html) / [getBasicFont](fnc-c0029-getBasicFont.html) / [setShortcutEvent](fnc-c0035-setShortcutEvent.html) /  [clearWindow](fnc-c0021-clearWindow.html) )

## ⭐ v19 ([Changelog](Changelog-v19).html)
- ゲージ設定(Gauge)の**ゲージ種・譜面別の入力補完**に対応
- danoni_setting.jsに**カスタムゲージリスト、デフォルトスキン、デフォルトカスタムJs指定**を追加
- タイトルの背景矢印の透明度を指定できるように変更
- グラデーションで色名を指定する場合に、透明度を合わせて指定できるよう変更
- ラベルテキスト及び説明文を danoni_constants.js へ移動・集約
- musicFolderのカレントディレクトリ指定に対応
- settingType, skinType, customjsについて**カレント＋サブディレクトリ指定**に対応
- Ready? 文字を直接書き換える設定を追加
- 作品htmlの**配置場所の変更**に対応
- 8keyにおいてEnterおにぎりを左側にするモードと12keyモードを実装
- **画面別ショートカットキー**を実装
- Ready? の文字幅を画面幅に合わせるよう変更

### 💡 Feature Updates
- [**v19.5.0**](https://github.com/cwtickle/danoniplus/releases/tag/v19.5.0) / [**v19.4.1**](https://github.com/cwtickle/danoniplus/releases/tag/v19.4.1) / [**v19.3.0**](https://github.com/cwtickle/danoniplus/releases/tag/v19.3.0) / [**v19.2.0**](https://github.com/cwtickle/danoniplus/releases/tag/v19.2.0) / [v19.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.1.0) / [v19.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v19.0.0)

### 📔 Documentation
- [ID一覧](idReferenceIndex.html)
- [ゲーム内ショートカット](Shortcut.html)
- 譜面ヘッダー仕様 ( [gaugeX](dos-h0022-gaugeX.html) / [titlegrd / titlearrowgrd](dos-h0032-titlegrd.html) / [musicFolder](dos-h0013-musicFolder.html) / [settingType](dos-h0056-settingType.html) / [skinType](dos-h0054-skinType.html) / [customjs](dos-h0019-customjs.html) / [readyHtml](dos-h0080-readyHtml.html) )
- [共通設定ファイル仕様](dos_setting.html)
- [グラデーション仕様](dos-c0001-gradation.html)
- [オブジェクト一覧](ObjectReferenceIndex.html) ( [g_lblNameObj](obj-v0015-g_lblNameObj.html) / [g_msgObj](obj-v0016-g_msgObj.html) / [g_shortcutObj](obj-v0017-g_shortcutObj.html) / [commonKeyDown](fnc-c0007-commonKeyDown.html) )

## ⭐ v18 ([Changelog](Changelog-v18).html)
- 矢印・フリーズアローの個別属性設定を見直し
- Display設定, Appearance, Opacity, ColorTypeのローカルストレージ保存に対応
- Adjustment, Volume, Appearance, Opacity, ColorTypeに限り、  
ローカル保存している設定を選択時にアスタリスクを付けるように変更
- **23key**を既定キーとして実装
- 矢印・フリーズアロー色の**強制グラデーション指定/解除**設定を実装
- 背景・マスクモーションで使用可能な画像ファイル拡張子に**svg形式**を追加
- 背景・マスクモーションのテキスト部分において**HTMLタグを許容**するよう変更
- **タイトル文字のアニメーション**を1・2行目で個別に設定できるよう変更
- 9A/9Bkeyの別キーモード時の配色を一部変更
- Firefoxで画像のプリロードを有効にするよう変更
- ライフ制ゲージ設定に「Heavy」を追加
- ColorType: 2のおにぎりの初期色を白から薄青に変更
- Gitter(得点報告用), ゲーム画面説明へのリンクを追加

### 💡 Feature Updates
- [**v18.9.0**](https://github.com/cwtickle/danoniplus/releases/tag/v18.9.0) / [v18.8.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.8.0) / [v18.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.0) / [v18.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.6.0) / [**v18.5.0**](https://github.com/cwtickle/danoniplus/releases/tag/v18.5.0) / [**v18.4.0**](https://github.com/cwtickle/danoniplus/releases/tag/v18.4.0) / [**v18.3.0**](https://github.com/cwtickle/danoniplus/releases/tag/v18.3.0) / [**v18.2.0**](https://github.com/cwtickle/danoniplus/releases/tag/v18.2.0) / [**v18.1.0**](https://github.com/cwtickle/danoniplus/releases/tag/v18.1.0) / [v18.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.0.0)

### 📔 Documentation
- [ゲーム画面の説明](AboutGameSystem.html)
- [ID一覧](IdReferenceIndex.html)
- 譜面ヘッダー仕様 ( [gaugeX](dos-h0022-gaugeX.html) / [defaultColorgrd](dos-h0061-defaultColorgrd.html) / [titleanimation](dos-h0077-titleanimation.html) / [customTitleAnimationUse](dos-h0078-customTitleAnimationUse.html) / [titleanimationclass](dos-h0079-titleanimationclass.html) )
- [譜面本体仕様](dos_score.html)
- 譜面エフェクト仕様 ( [back/mask_data](dos-e0004-animationData.html) )
- [共通設定ファイル仕様](dos_setting.html)
- [主要オブジェクトのプロパティ](objectMainRef.html)
- [ローカルストレージ仕様](LocalStorage.html)
- [譜面データにおける特殊文字の取り扱い](SpecialCharacters.html)

## ⭐ v17 ([Changelog](Changelog-v17).html)
- ラベル・ボタン・色付きオブジェクト作成用関数を作り直し
- ボタンクリック、右クリック後の処理に対して処理を追加できる機能を実装
- ボタン及びラベルのスタイル一括変更関数を実装
- タイトル文字のフォントと位置について2行目指定ができるように変更
- strictモードを再有効化

### 💡 Feature Updates
- [v17.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.5.0) / [**v17.4.0**](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.0) / [v17.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.3.0) / [v17.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.2.0) / [v17.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.1.0) / [v17.0.1](https://github.com/cwtickle/danoniplus/releases/tag/v17.0.1)

### 📔 Documentation
- 譜面ヘッダー仕様 ( [titlesize](dos-h0030-titlesize.html) / [titlefont](dos-h0031-titlefont.html)  / [titlepos](dos-h0033-titlepos.html) )
- [オブジェクト一覧](objectReferenceIndex.html) ( [createDivCss2Label](fnc-c0002-createDivCss2Label.html) / [createColorObject2](fnc-c0003-createColorObject2.html) / [createCss2Button](fnc-c0004-createCss2Button.html) / [changeStyle](fnc-c0005-changeStyle.html) )

## ⭐ v16 ([Changelog](Changelog-v16).html)
- プレイ画面範囲の横幅・位置調整機能を追加
- `KeyboardEvent.keyCode`を`KeyboardEvent.code`へ置き換え
- リザルトデータの**クリップボードコピー機能**を実装 
- CapsLockキーの無効化設定及び無効キーのメッセージを追加
- **20個以上のキー**に対する色変化（単発矢印・個別）に対応
- リザルトデータの**フォーマット機能**を実装
- Ready表示の**アニメーション変更、先頭色変更**に対応
- Ready表示の遅延フレーム設定について、プレイ中のフェードイン有効時は無効にするよう変更
- 結果画面のCLEARED / FAILED表示に対する遅延フレーム設定を実装

### 💡 Feature Updates
- [v16.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v16.4.0) / [**v16.3.0**](https://github.com/cwtickle/danoniplus/releases/tag/v16.3.0) / [**v16.2.1**](https://github.com/cwtickle/danoniplus/releases/tag/v16.2.1) / [**v16.1.0**](https://github.com/cwtickle/danoniplus/releases/tag/v16.1.0) / [v16.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v16.0.0)

### 📔 Documentation
- [ID一覧](IdReferenceIndex.html)
- 譜面ヘッダー仕様 ( [playingX](dos-h0070-playingX.html) / [playingWidth](dos-h0071-playingWidth.html) / [resultFormat](dos-h0072-resultFormat.html) / [readyAnimationFrame](dos-h0073-readyAnimationFrame.html) / [readyAnimationName](dos-h0074-readyAnimationName.html) / [readyColor](dos-h0075-readyColor.html) )
- [共通設定ファイル仕様](dos_setting.html)
- 譜面エフェクト仕様 ( [acolor/color_data](dos-e0002-colorData.html) )

## ⭐ v15 ([Changelog](Changelog-v15).html)
- AutoPlay設定に対して一部キーを**アシスト**する設定を追加
- 外部リンクに対してオンマウスでURLを表示
- 譜面効果データでフレーム・深度等に**数式**が使えるよう変更
- 主要画像をpng形式から**svg形式**へ変更
- 作品コメント文をタイトル画面に表示する機能を実装
- 作品を**動的に切り替え**られる機能及び関連機能を実装
- Background:OFF時に判定表示位置(jdgY)を初期化する設定を追加
- Reverse時に条件付きで**歌詞を上下逆**の位置に表示するよう変更
- 歌詞表示で**フォントサイズが変更**できる構文を追加
- 7, 11, 11L, 11Wkeyにおいて12keyモードを実装 
- Winキー+Shiftキーでキーコンが反応しないように処理を見直し

### 💡 Feature Updates
- [v15.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.7.0) / [v15.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.6.0) / [v15.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.5.0) / [v15.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.4.0) / [v15.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.3.0) / [**v15.2.0**](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.0) / [**v15.1.0**](https://github.com/cwtickle/danoniplus/releases/tag/v15.1.0) / [**v15.0.0**](https://github.com/cwtickle/danoniplus/releases/tag/v15.0.0)

### 📔 Documentation
- [キーの仕様について](keys.html)
- [ソースの構成](AboutSource.html)
- [ID一覧](idReferenceIndex.html)
- [共通設定ファイル仕様](dos_setting.html)
- 譜面ヘッダー仕様 ( [jdgPosReset](dos-h0065-jdgPosReset.html) / [commentVal](dos-h0066-commentVal.html) / [commentAutoBr](dos-h0067-commentAutoBr.html) / [commentExternal](dos-h0068-commentExternal.html) / [wordAutoReverse](dos-h0069-wordAutoReverse.html) )
- 譜面エフェクト仕様 ( [speed/boost_data](dos-e0001-speedData.html) / [acolor/color_data](dos-e0002-colorData.html) / [word_data](dos-e0003-wordData.html) / [back/mask_data](dos-e0004-animationData.html) )
- [譜面データにおける特殊文字の取り扱い](SpecialCharacters.html)

## ⭐ v14 ([Changelog](Changelog-v14).html)
- Displayオプションの**デフォルトON/OFF**設定及び**有効/無効化**設定の実装
- DisplayオプションのボタンがONの状態のとき、  
他のボタンを**連動してOFF**に自動変更する機能を実装
- オンマウスでオプション設定の説明文を表示するよう変更 
- 矢印描画について、ステップゾーン位置に応じて描画領域が変わるように変更
- Display: MusicInfo適用時、楽曲のクレジットを最初の数秒のみ表示する形式に変更
- グラデーション表記で**色名** (blueやredなど) が使えるよう変更
- 影矢印のデザインを見直し
- APMの計算式をレベル計算ツール++の形式に寄せるよう修正
- ローカル時に限り、誤差1フレームでもFast/Slowを表示するように変更  
(合わせて、±1フレーム以内で表示するJust表記を廃止)
- 結果画面に**Fast/Slowのカウント数を表示**するよう変更
- Twitter投稿用リザルトの**URL表示に譜面番号を付加**するよう変更
- 譜面データで**パイプ、アンパサンド等の特殊文字**を利用するための文字列を作成
- 譜面数が5を超える場合、自動で譜面セレクターを使用するよう変更
- バージョン比較用リンクを作成

### 💡 Feature Updates
- [v14.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v14.5.0) / [v14.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v14.4.0) / [**v14.3.4**](https://github.com/cwtickle/danoniplus/releases/tag/v14.3.4) / [v14.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v14.2.0) / [v14.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v14.1.0) / [**v14.0.2**](https://github.com/cwtickle/danoniplus/releases/tag/v14.0.2)

### 📔 Documentation
- [共通設定ファイル仕様](dos_setting.html)
- [グラデーション仕様](dos-c0001-gradation.html)
- 譜面ヘッダー仕様 ( [displayUse](dos-h0057-displayUse.html) / [displayChainOFF](dos-h0064-displayChainOFF.html) / [difSelectorUse](dos-h0051-difSelectorUse.html) )
- [譜面データにおける特殊文字の取り扱い](SpecialCharacters.html)

## ⭐ v13 ([Changelog](Changelog-v13).html)
- **矢印塗りつぶし部分の初期色**に対してグラデーション他に対応
- フリーズアロー初期色 (frzColor)が未定義の場合、  
矢印初期色 (setColor) の値から適用する形式に変更
- フリーズアローの塗りつぶし部分に対する設定を追加
- 従来のfrzColor補完ができる設定を追加
- Appearance設定に「**Hidden+**」「**Sudden+**」「**Hid&Sud+**」を追加
- 既定のキーに対して最低1つの代替キーを設定するよう変更
- Display:JudgmentをJudgment(判定キャラクタ)、FastSlow、Score(判定数)に分離
- Displayオプションのデフォルト無効化設定を追加
- 判定表示、Hidden+/Sudden+の境界線表示の透明度を調整する「Opacity」を実装
- 開始/終了フレームなどを指定するstartFrame, fadeFrame, endFrameについて  
疑似タイマー表記に対応

### 💡 Feature Updates
- [v13.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v13.6.0) / [v13.5.1](https://github.com/cwtickle/danoniplus/releases/tag/v13.5.1) / [**v13.4.0**](https://github.com/cwtickle/danoniplus/releases/tag/v13.4.0) / [v13.3.1](https://github.com/cwtickle/danoniplus/releases/tag/v13.3.1) / [**v13.2.0**](https://github.com/cwtickle/danoniplus/releases/tag/v13.2.0) / [v13.1.1](https://github.com/cwtickle/danoniplus/releases/tag/v13.1.1) / [**v13.0.0**](https://github.com/cwtickle/danoniplus/releases/tag/v13.0.0)

### 📔 Documentation
- [ゲーム画面の説明](AboutGameSystem.html)
- [共通設定ファイル仕様](dos_setting.html)
- 譜面ヘッダー仕様 ( [setColor](dos-h0003-setColor.html) / [frzColor](dos-h0004-frzColor.html) / [setShadowColor](dos-h0041-setShadowColor.html) / [frzShadowColor](dos-h0062-frzShadowColor.html) / [defaultFrzColorUse](dos-h0063-defaultFrzColorUse.html) / [displayUse](dos-h0057-displayUse.html) / [startFrame](dos-h0005-startFrame.html) / [fadeFrame](dos-h0008-fadeFrame.html) / [endFrame](dos-h0007-endFrame.html) )


## ⭐ v12 ([Changelog](Changelog-v12).html)
- 矢印色、フリーズアロー色の**グラデーション**を実装
- 常時グラデーション設定の追加
- タイトル曲名、背景矢印のグラデーション拡張を実装
- **レベル計算**ツール++の移植
- 矢印描画エリアを縮小する設定を追加
- 7ikeyのScroll: Asymmetryについて、左矢印のスクロールを反転する仕様に変更
- ローカルで直接htmlファイルを開いても画像が表示されるように変更

### 💡 Feature Updates
- [**v12.3.0**](https://github.com/cwtickle/danoniplus/releases/tag/v12.3.0) / [v12.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.2.0) / [v12.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.1.0) / [**v12.0.0**](https://github.com/cwtickle/danoniplus/releases/tag/v12.0.0)

### 📔 Documentation
- [キーの仕様について](keys.html)
- [グラデーション仕様](dos-c0001-gradation.html)
- 譜面ヘッダー仕様 ( [setColor](dos-h0003-setColor.html) / [frzColor](dos-h0004-frzColor.html) / [titlegrd / titlearrowgrd](dos-h0032-titlegrd.html) / [defaultColorgrd](dos-h0061-defaultColorgrd.html) )
- 譜面エフェクト仕様 ( [acolor/color_data](dos-e0002-colorData.html) )
- [ローカルでのプレイ方法](HowToLocalPlay.html)

## ⭐ v11 ([Changelog](Changelog-v11).html)
- Displayオプションのデフォルト設定を追加
- カスタム用のDisplayオプション「Special」を追加
- 判定キャラクタの下に**Fast/Slow/Just**表記を追加
- 判定キャラクタの位置調整機能を追加
- 5keyのKeyPattern: 3(おにぎり中央)の既定のキーコンフィグを変更
- 7keyの既定のキーコンフィグを追加
- 下側の歌詞表示位置をステップゾーン位置に追随させる設定を追加
- 判定キャラクタ、ReadyのY座標を下側のステップゾーン位置(stepYR)に合わせて  
自動調整するように変更
- **速度変化の遷移グラフ、譜面密度分布グラフ**の実装

### 💡 Feature Updates
- [v11.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v11.4.0) / [**v11.3.0**](https://github.com/cwtickle/danoniplus/releases/tag/v11.3.0) / [v11.1.2](https://github.com/cwtickle/danoniplus/releases/tag/v11.1.2) / [**v11.0.0**](https://github.com/cwtickle/danoniplus/releases/tag/v11.0.0)

### 📔 Documentation
- 譜面ヘッダー仕様 ( [displayUse](dos-h0057-displayUse.html) / [arrowJdgY / frzJdgY](dos-h0058-jdgY.html) / [bottomWordSet](dos-h0059-bottomWordSet.html) / [scoreDetailUse](dos-h0060-scoreDetailUse.html) )
- [画面の位置調整方法](tips-0003-position-adjustment.html)

## ⭐ v10 ([Changelog](Changelog-v10).html)
- **スキン**機能の実装
- 背景・マスクに対象拡張子のデータがあれば、**自動でpreload**する機能を実装
- danoni_setting.js を**グループごとに分けられる**ように変更
- js, css, skinフォルダ配下のファイル指定に対して**カレントディレクトリ指定**に対応  
(skinType, settingType, musicUrl, customjs でファイルの先頭に(..) を付加することで可能)
- danoni_custom.js や danoni_setting.js が無くても動作するように変更
- Canvasタグを使用しなくても動作するように変更
- **MacOS, iOS** (Safari)において動作しない問題を修正 (v5, v8, v9にも適用済)
- **スクロール拡張**（Cross / Split / Flat 他）に対応
- 矢印のヒット部分を**押したタイミングに応じて変える**ように変更
- 譜面データで使用する矢印名で命名できる種類を拡張  
（ある程度任意の名前を指定しても、フリーズアローが自動で対応するように変更）

### 💡 Feature Updates
- [v10.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v10.4.0)  / [**v10.2.1**](https://github.com/cwtickle/danoniplus/releases/tag/v10.2.1) / [v10.1.1](https://github.com/cwtickle/danoniplus/releases/tag/v10.1.1) / [**v10.0.0**](https://github.com/cwtickle/danoniplus/releases/tag/v10.0.0)

### 📔 Documentation
- [更新情報 (UpdateInfo-v10)](UpdateInfo-v10.html)
- [アップグレードガイド](MigrationGuide.html)
- [ソースの構成](AboutSource.html)
- [共通設定ファイル仕様](dos_setting.html)
- 譜面ヘッダー仕様 ( [musicUrl](dos-h0011-musicUrl.html) / [customjs](dos-h0019-customjs.html) / [skinType](dos-h0054-skinType.html) / [settingType](dos-h0056-settingType.html) / [autoPreload](dos-h0055-autoPreload.html) / [scrollUse](dos-h0035-settingUse.html) )
- 譜面エフェクト仕様 ( [word_data](dos-e0003-wordData.html) / [back_data / mask_data](dos-e0004-animationData.html) )

## ⭐ v9 ([Changelog](Changelog-v9).html)
- **Appearance**オプションの実装
- Ready表示の**遅延フレーム設定**を追加
- リバース用の歌詞表示（wordRev_data）を実装 
- **カスタムゲージ設定**の実装

### 💡 Feature Updates
- [v9.4.2](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.2) / [**v9.4.0**](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.0) / [v9.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v9.3.0) / [v9.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v9.2.0) / [v9.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v9.1.0) / [**v9.0.0**](https://github.com/cwtickle/danoniplus/releases/tag/v9.0.0)

### 📔 Documentation
- [共通設定ファイル仕様](dos_setting.html)
- 譜面ヘッダー仕様 ( [appearanceUse](dos-h0035-settingUse.html) / [readyDelayFrame](dos-h0052-readyDelayFrame.html) / [customGauge](dos-h0053-customGauge.html) / [gaugeX](dos-h0022-gaugeX.html) )
- 譜面エフェクト仕様 ( [back_data / mask_data](dos-e0004-animationData.html) / [word_data](dos-e0003-wordData.html) )

## ⭐ v8 ([Changelog](Changelog-v8).html)
- タイトル/リザルトモーションの**音楽同期**に対応
- リザルトモーションを譜面別に作成できるように変更
- **楽曲のフェードアウト長**を指定できるように変更
- 速度変化表記 (speed_data/change) の統一
- ステップゾーン(下)位置を変更できる設定を追加
- **制作者表示の複数化**に対応（設定画面・結果画面・リザルトコピー）
- 曲名（複数行）を1行で表示する場合に間を空白で埋めない（全角で埋める）設定を追加
- 譜面変更用の**セレクター**を実装
- **譜面毎のファイル分割**に対応
- 譜面をファイル分割した場合に、譜面番号を常時固定するかどうかの設定を追加

### 💡 Feature Updates
- [v8.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v8.7.0) / [**v8.5.0**](https://github.com/cwtickle/danoniplus/releases/tag/v8.5.0) / [v8.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v8.4.0) / [**v8.3.0**](https://github.com/cwtickle/danoniplus/releases/tag/v8.3.0) / [v8.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v8.2.0) / [v8.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v8.1.0) / [v8.0.4](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.4) / [**v8.0.0**](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.0)

### 📔 Documentation
- [譜面の作成概要](HowToMake.html)
- 譜面ヘッダー仕様 ( [musicTitle](dos-h0001-musicTitle.html) / [difData](dos-h0002-difData.html) / [fadeFrame](dos-h0008-fadeFrame.html) / [stepYR](dos-h0049-stepYR.html) / [makerView](dos-h0050-makerView.html) / [difSelectorUse](dos-h0051-difSelectorUse.html) )
- 譜面エフェクト仕様 ( [back_data / mask_data](dos-e0004-animationData.html) / [speed_data/change / boost_data](dos-e0001-speedData.html) )
- [ローカルストレージ仕様](LocalStorage.html)

## ⭐ v7 ([Changelog](Changelog-v7).html)
- 矢印・フリーズアローに**CSSモーション**機能を実装
- フリーズアローヒット時の個別色変化のタイミングを変更
- デフォルトで選択状態にする譜面をURLで指定できる機能を実装
- 譜面読込画面に入ったときに譜面データ・リザルトモーションを再読込できるように変更
- タイトル/リザルトモーションのジャンプ(loop/jump)で  
**確率でジャンプ先を変えられる**ように変更
- 歌詞表示・背景/マスクモーションにおいて**同一フレームの複数同時描画**に対応
- 背景/マスクモーションにおいて、深度に「ALL」を指定することで、  
全てのオブジェクトを**一斉クリア**できるように対応
- 楽曲の終了判定タイミングを秒単位から**フレーム単位**に変更
- クリア失敗時のリザルトモーションを実装
- 背景・マスクモーション、速度変化、色変化、歌詞表示で**コメント文**を実装

### 💡 Feature Updates
- [**v7.9.0**](https://github.com/cwtickle/danoniplus/releases/tag/v7.9.0) / [v7.8.1](https://github.com/cwtickle/danoniplus/releases/tag/v7.8.1) / [**v7.8.0**](https://github.com/cwtickle/danoniplus/releases/tag/v7.8.0) / [**v7.7.0**](https://github.com/cwtickle/danoniplus/releases/tag/v7.7.0) /  [v7.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v7.6.0) / [**v7.5.0**](https://github.com/cwtickle/danoniplus/releases/tag/v7.5.0) / [v7.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v7.4.0) / [**v7.3.0**](https://github.com/cwtickle/danoniplus/releases/tag/v7.3.0) / [v7.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v7.1.0) / [**v7.0.0**](https://github.com/cwtickle/danoniplus/releases/tag/v7.0.0)

### 📔 Documentation
- 譜面ヘッダー仕様 ( [colorDataType](dos-h0046-colorDataType.html) / [colorCdPaddingUse](dos-h0047-colorCdPaddingUse.html) / [resultMotionSet](dos-h0048-resultMotionSet.html) )
- 譜面エフェクト仕様 ( [矢印・フリーズアローモーション](dos-e0005-motionData.html) / [back_data / mask_data](dos-e0004-animationData.html) )

## ⭐ v6 ([Changelog](Changelog-v6).html)
- **ダミー**矢印・フリーズアロー機能の実装
- 配点と最大スコアを変数化し、danoni_custom/setting.jsから変更できるように対応
- リバース用背景・マスクモーション(backRev_data, maskRev_data)の実装
- **リザルトモーション**(backresult_data, maskresult_data)の実装
- タイトルに対してマスクモーション(masktitle_data)を実装
- ライフ上限値の設定を追加
- **ライフ制ゲージ** (Original, Light, NoRecovery)の設定を譜面ヘッダーから設定できるように変更
- 特殊キー(keyExtraList指定キー)に対してリバース、キーコンフィグ保存に対応

### 💡 Feature Updates
- [v6.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v6.6.0) / [**v6.5.0**](https://github.com/cwtickle/danoniplus/releases/tag/v6.5.0) / [v6.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v6.4.0) / [**v6.3.0**](https://github.com/cwtickle/danoniplus/releases/tag/v6.3.0) /  [v6.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v6.2.0) / [v6.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v6.1.0) / [**v6.0.0**](https://github.com/cwtickle/danoniplus/releases/tag/v6.0.0)

### 📔 Documentation
- 譜面ヘッダー仕様 ( [dummyId](dos-h0042-dummyId.html) / [maxLifeVal](dos-h0045-maxLifeVal.html) / [gaugeOriginal / gaugeLight / gaugeNoRecovery](dos-h0022-gaugeX.html) )
- 譜面エフェクト仕様 ( [back_data / mask_data](dos-e0004-animationData.html) )
- [ローカルストレージ仕様](LocalStorage.html)

## ⭐ v5 ([Changelog](Changelog-v5).html)
- タイトル（デフォルト）の**行別グラデーション**に対応
- 縦方向のスケーリングに対応
- 最低・最高速度、譜面変更ボタン(setDifficulty)に対してカスタム関数を追加
- 歌詞表示(word_data)の**複数階層化**に対応
- 歌詞フェードイン・アウトの時間の可変対応
- フリーズアロー**開始判定**の実装
- 譜面データのURIデコードに対応
- 譜面データの&区切り可否の切替機能を追加
- フリーズアローの許容フレームを譜面ヘッダーから指定できるように変更
- キー毎にタイトルバック、リトライ用ショートカットキーの指定を行えるように変更
- 通常矢印の**内側を塗りつぶす**機能を追加

### 💡 Feature Updates
- [**v5.12.0**](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.0) / [v5.11.0](https://github.com/cwtickle/danoniplus/releases/tag/v5.11.0) / [**v5.10.0**](https://github.com/cwtickle/danoniplus/releases/tag/v5.10.0) / [v5.9.0](https://github.com/cwtickle/danoniplus/releases/tag/v5.9.0) /  [**v5.8.0**](https://github.com/cwtickle/danoniplus/releases/tag/v5.8.0) / [v5.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v5.7.0) / [**v5.6.6**](https://github.com/cwtickle/danoniplus/releases/tag/v5.6.6) / [v5.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v5.6.0) / [**v5.4.0**](https://github.com/cwtickle/danoniplus/releases/tag/v5.4.0) / [v5.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v5.2.0) / [**v5.1.0**](https://github.com/cwtickle/danoniplus/releases/tag/v5.1.0) / [v5.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v5.0.0)

### 📔 Documentation
- [キーの仕様について](keys.html)
- [共通設定ファイル仕様](dos_setting.html)
- 譜面ヘッダー仕様 ( [titlegrd](dos-h0032-titlegrd.html) / [minSpeed](dos-h0015-minSpeed.html) / [maxSpeed](dos-h0016-maxSpeed.html) / [frzStartjdgUse](dos-h0037-frzStartjdgUse.html) / [frzAttempt](dos-h0038-frzAttempt.html) / [keyRetry](dos-h0039-keyRetry.html) / [keyTitleBack](dos-h0040-keyTitleBack.html) )
- 譜面エフェクト仕様 ( [word_data](dos-e0003-wordData.html) )

## ⭐ v4 ([Changelog](Changelog-v4).html)
- 譜面別の**複数曲読込**に対応 ![v4.0.0](https://img.shields.io/badge/-v4.0.0-blue)
- **ローカルストレージ**(作品別、キー別)を実装 ![v4.6.0](https://img.shields.io/badge/-v4.6.0-blue)
- 画面全体に**マスク**を設定するためのデータ(mask_data)を実装 ![v4.2.0](https://img.shields.io/badge/-v4.2.0-blue)
- タイトル画面に対して背景表示をつける機能 (backtitle_data) を追加 ![v4.7.0](https://img.shields.io/badge/-v4.7.0-blue)
- 11key譜面を**11Lkeyとして**プレイできるモードを追加 ![v4.8.0](https://img.shields.io/badge/-v4.8.0-blue)
- 曲中リトライ以外のタイミングで曲の再読み込みを行う仕様に変更 ![v4.10.0](https://img.shields.io/badge/-v4.10.0-blue)

### 💡 Feature Updates
- [**v4.10.0**](https://github.com/cwtickle/danoniplus/releases/tag/v4.10.0) / [**v4.8.0**](https://github.com/cwtickle/danoniplus/releases/tag/v4.8.0) / [v4.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v4.7.0) / [**v4.6.0**](https://github.com/cwtickle/danoniplus/releases/tag/v4.6.0) /  [**v4.4.0**](https://github.com/cwtickle/danoniplus/releases/tag/v4.4.0) / [v4.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v4.3.0) / [**v4.2.0**](https://github.com/cwtickle/danoniplus/releases/tag/v4.2.0) / [v4.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v4.1.0) / [**v4.0.0**](https://github.com/cwtickle/danoniplus/releases/tag/v4.0.0)

### 📔 Documentation
- 譜面ヘッダー仕様 ( [musicUrl](dos-h0011-musicUrl.html) / [musicNo](dos-h0012-musicNo.html) / [transKeyUse](dos-h0024-transKeyUse.html) )
- 譜面エフェクト仕様 ( [mask_data / backtitle_data](dos-e0004-animationData.html) )
- [ローカルストレージ仕様](LocalStorage.html)

## ⭐ v3 ([Changelog](Changelog-v3).html)
- 製作者別設定ファイルを追加 ![v3.0.0](https://img.shields.io/badge/-v3.0.0-blue)
- **Shuffle**機能（Mirror, Randomなど）を追加 ![v3.1.0](https://img.shields.io/badge/-v3.1.0-blue)
- 曲名タイトル（デフォルト）の複数行、モーション、グラデーション対応 ![v3.5.0](https://img.shields.io/badge/-v3.5.0-blue)
- 速度変化、色変化、歌詞表示の**セット毎改行区切り**に対応 ![v3.10.0](https://img.shields.io/badge/-v3.10.0-blue)
- 譜面ヘッダー「startFrame」について、譜面毎に設定できるように変更 ![v3.11.0](https://img.shields.io/badge/-v3.11.0-blue)
- キーコンフィグ画面で作品毎の矢印色ではない、  
共通デフォルト色を指定できるように変更 (ColorTypeの追加) ![v3.12.0](https://img.shields.io/badge/-v3.12.0-blue)

### 💡 Feature Updates
- [v3.12.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.12.0) / [v3.11.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.11.0) / [**v3.10.0**](https://github.com/cwtickle/danoniplus/releases/tag/v3.10.0) / [v3.9.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.9.0) /  [v3.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.7.0) / [v3.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v3.6.0) / [**v3.5.0**](https://github.com/cwtickle/danoniplus/releases/tag/v3.5.0) / [**v3.2.0**](https://github.com/cwtickle/danoniplus/releases/tag/v3.2.0) / [**v3.1.0**](https://github.com/cwtickle/danoniplus/releases/tag/v3.1.0) / [**v3.0.0**](https://github.com/cwtickle/danoniplus/releases/tag/v3.0.0)

### 📔 Documentation
- [ソースの構成](AboutSource.html)
- [共通設定ファイル仕様](dos_setting.html)
- 譜面ヘッダー仕様 ( [motionUse / shuffleUse / autoPlayUse / gaugeUse](dos-h0035-settingUse.html) /   
[musicTitle](dos-h0001-musicTitle.html) / [titlesize](dos-h0030-titlesize.html) /  [titlelineheight](dos-h0034-titlelineheight.html) / 
[startFrame](dos-h0005-startFrame.html) )
- 譜面エフェクト仕様 ( [acolor/color_data](dos-e0002-colorData.html) / [word_data](dos-e0003-wordData.html) )

## ⭐ v2 ([Changelog](Changelog-v2).html)
- 譜面データの**外部ファイル化**に対応 ![v2.3.0](https://img.shields.io/badge/-v2.3.0-blue)
- ロード画面の実装 ![v2.6.0](https://img.shields.io/badge/-v2.6.0-blue)
- オンライン時にWebAudioAPIで楽曲を再生するように変更 ![v2.7.0](https://img.shields.io/badge/-v2.7.0-blue) 
- 譜面ヘッダーで**曲の再生速度を指定**できる機能を追加 ![v2.8.0](https://img.shields.io/badge/-v2.8.0-blue)
- 譜面ヘッダーにて、譜面別に（製作者側が）**タイミング調整**できるように変更 ![v2.2.0](https://img.shields.io/badge/-v2.2.0-blue)
- タイトル文字のフォント設定に対応 ![v2.1.0](https://img.shields.io/badge/-v2.1.0-blue)

### 💡 Feature Updates
- [v2.9.0](https://github.com/cwtickle/danoniplus/releases/tag/v2.9.0) / [**v2.8.0**](https://github.com/cwtickle/danoniplus/releases/tag/v2.8.0) / [v2.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v2.7.0) / [v2.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v2.6.0) /  [v2.5.0](https://github.com/cwtickle/danoniplus/releases/tag/v2.5.0) / [**v2.3.0**](https://github.com/cwtickle/danoniplus/releases/tag/v2.3.0) / [**v2.2.0**](https://github.com/cwtickle/danoniplus/releases/tag/v2.2.0) / [**v2.1.0**](https://github.com/cwtickle/danoniplus/releases/tag/v2.1.0) / [v2.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v2.0.0)

### 📔 Documentation
- [譜面の作成概要](HowToMake.html)
- 譜面ヘッダー仕様 ( [adjustment](dos-h0009-adjustment.html) / [playbackRate](dos-h0010-playbackRate.html) )

## ⭐ v1 ([Changelog](Changelog-v1).html)
- **Gauge**オプションの実装 ![v1.0.0](https://img.shields.io/badge/-v1.0.0-blue)
- **ノルマ制ゲージ** (Normal, Easy, Hard)の設定を譜面ヘッダーから設定できるように変更 ![v1.5.0](https://img.shields.io/badge/-v1.5.0-blue)
- 音楽ファイルについて**base64エンコード**に対応 ![v1.7.0](https://img.shields.io/badge/-v1.7.0-blue)
- 歌詞表示で、左揃え/中央揃え/右揃えの設定を追加 ![v1.9.0](https://img.shields.io/badge/-v1.9.0-blue)
- 歌詞表示の二重階層化に対応 ![v1.9.0](https://img.shields.io/badge/-v1.9.0-blue)
- 曲終了フレーム(endFrame)の譜面別指定に対応 ![v1.10.0](https://img.shields.io/badge/-v1.10.0-blue)
- 判定処理のカスタム処理を分離 ![v1.11.0](https://img.shields.io/badge/-v1.11.0-blue)
- 外部jsファイルのキャッシュを利用しないように変更 ![v1.12.0](https://img.shields.io/badge/-v1.12.0-blue)
- タイトル文字以外のフォントを設定できるように変更 ![v1.12.0](https://img.shields.io/badge/-v1.12.0-blue)
- ステップゾーン間隔を譜面側から設定できるように変更 (blankX) ![v1.14.0](https://img.shields.io/badge/-v1.14.0-blue)

### 💡 Feature Updates
- [v1.15.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.15.0) / [v1.14.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.14.0) / [v1.13.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.13.0) / [v1.12.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.12.0) /  [**v1.11.0**](https://github.com/cwtickle/danoniplus/releases/tag/v1.11.0) / [v1.10.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.10.0) / [**v1.9.0**](https://github.com/cwtickle/danoniplus/releases/tag/v1.9.0) / [**v1.7.0**](https://github.com/cwtickle/danoniplus/releases/tag/v1.7.0) / [**v1.5.0**](https://github.com/cwtickle/danoniplus/releases/tag/v1.5.0) / [v1.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.3.0) / [v1.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.2.0) / [v1.0.0](https://github.com/cwtickle/danoniplus/releases/tag/v1.0.1)

### 📔 Documentation
- [ゲーム画面の説明](AboutGameSystem.html)
- [譜面の作成概要](HowToMake.html)
- [キーの仕様について](keys.html)
- 譜面ヘッダー仕様 ( [endFrame](dos-h0007-endFrame.html) / [musicUrl](dos-h0011-musicUrl.html) / [customFont](dos-h0020-customFont.html) / [gaugeX](dos-h0022-gaugeX.html) / [finishView](dos-h0023-finishView.html) )
- 譜面エフェクト仕様 ( [word_data](dos-e0003-wordData.html) )
