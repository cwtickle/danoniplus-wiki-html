# 譜面ヘッダー仕様 (初期設定)
ParaFla版をベースとしているため、ほとんどの項目はそのまま使えます。  
また区切り文字として"|"を使用していますが、"&"も一応使えます。  
注意点は[ParaFlaユーザ向け使い方](forParaFlaUser)もご覧ください。  

(*)必須項目 / (★)ParaFlaソースとの共用項目 / (◇)譜面別設定可 / (◆)譜面別分割書式可  
また使用頻度が高かったり、要所で使う可能性のあるものは太字にしています。  

## 🎶 楽曲・譜面情報
- [**musicTitle**](dos-h0001-musicTitle.html) (*, ★)  楽曲／楽曲クレジット
- [**difData**](dos-h0002-difData.html) (★, ◇)  譜面情報 
- [**musicUrl**](dos-h0011-musicUrl.html) (*)  楽曲ファイル名
- [musicNo](dos-h0012-musicNo.html) (◇)  楽曲ファイルと譜面の対応付け
- [musicFolder](dos-h0013-musicFolder.html)  楽曲ファイルの格納先
- [dummyId](dos-h0042-dummyId.html) (◇)  ダミー譜面の指定

## ⏳ プレイ時間制御・譜面位置調整
- [startFrame](dos-h0005-startFrame.html) (★, ◇)  プレイ開始フレーム数
- [blankFrame](dos-h0006-blankFrame.html)  曲開始までの空白フレーム数
- [**endFrame**](dos-h0007-endFrame.html) (◇)  プレイ終了フレーム数
- [**fadeFrame**](dos-h0008-fadeFrame.html) (◇)  フェードアウト開始フレーム数
- [**adjustment**](dos-h0009-adjustment.html) (◇)  譜面位置の初期調整
- [**playbackRate**](dos-h0010-playbackRate.html)  楽曲再生速度（主にテストプレイ用）

## 🛠 設定時の初期設定
- [minSpeed](dos-h0015-minSpeed.html)  設定できる最低速度
- [maxSpeed](dos-h0016-maxSpeed.html)  設定できる最高速度
- [difSelectorUse](dos-h0051-difSelectorUse.html)  譜面選択セレクターの利用有無
- [scoreDetailUse](dos-h0060-scoreDetailUse.html)  譜面明細表示の利用有無
- [**settingUse**](dos-h0035-settingUse.html)  設定項目の利用有無
   - motionUse, scrollUse, shuffleUse, ... etc
- [displayUse](dos-h0057-displayUse.html)  Display項目の利用有無, 初期値設定
   - stepZoneUse, judgmentUse, fastSlowUse, ... etc
- [displayChainOFF](dos-h0064-displayChainOFF.html)  Display項目の連動OFF設定
   - backgroundChainOFF, arrowEffectChainOFF, specialChainOFF, ... etc
- [transKeyUse](dos-h0024-transKeyUse.html) (◇)  別キーモードの利用有無
- [**customFont**](dos-h0020-customFont.html)  画面全般のフォント
- [**customGauge**](dos-h0053-customGauge.html) (◆)  カスタムゲージ設定
- [**gaugeX**](dos-h0022-gaugeX.html) (◇, ◆)  ゲージ設定の詳細
   - gaugeEasy, gaugeHard, gaugeLight, ... etc
- [colorDataType](dos-h0046-colorDataType.html)  色変化の過去互換設定
- [colorCdPaddingUse](dos-h0047-colorCdPaddingUse.html)  初期矢印色/フリーズアロー色のゼロパディング有無設定

## ⏯ プレイ時の初期設定
### 矢印・フリーズアロー色の設定
- [**setColor**](dos-h0003-setColor.html) (★, ◆)  矢印色
- [**frzColor**](dos-h0004-frzColor.html) (★, ◆)  フリーズアロー色
- [setShadowColor](dos-h0041-setShadowColor.html) (◆)  矢印の内側を塗りつぶす設定および色の設定
- [frzShadowColor](dos-h0062-frzShadowColor.html) (◆)  フリーズアローの矢印内側を塗りつぶす設定および色の設定
- [**defaultColorgrd**](dos-h0061-defaultColorgrd.html)  自動グラデーション設定
- [defaultFrzColorUse](dos-h0063-defaultFrzColorUse.html)  フリーズアロー初期色(frzColor)が未指定時の適用方法

### プレイ画面位置の設定
- [playingX](dos-h0070-playingX.html)  ゲーム表示エリアのX座標
- [playingWidth](dos-h0071-playingWidth.html)  ゲーム表示エリアの横幅
- [stepY](dos-h0014-stepY.html)  ステップゾーンのY座標位置
- [stepYR](dos-h0049-stepYR.html)  ステップゾーン(下)のY座標現位置からの差分
- [arrowJdgY / frzJdgY](dos-h0058-jdgY.html)  判定キャラクタのY座標位置
- [jdgPosReset](dos-h0065-jdgPosReset.html)  判定キャラクタ位置のリセット設定(Background:OFF時)
- [bottomWordSet](dos-h0059-bottomWordSet.html)  下側の歌詞表示位置をステップゾーン位置に連動させる設定
- [wordAutoReverse](dos-h0069-wordAutoReverse.html)  Reverse時に歌詞表示を条件付きで反転させる設定

### ライフゲージ・判定関連の設定
- [maxLifeVal](dos-h0045-maxLifeVal.html)  ライフの上限値
- [frzStartjdgUse](dos-h0037-frzStartjdgUse.html)  フリーズアロー開始判定の設定有無
- [frzAttempt](dos-h0038-frzAttempt.html)  フリーズアローヒット時の許容フレーム数

### 画面表示・キーコントロール
- [readyDelayFrame](dos-h0052-readyDelayFrame.html)  Ready?が表示されるまでの遅延フレーム数
- [readyAnimationFrame](dos-h0073-readyAnimationFrame.html)  Ready?のアニメーションフレーム数
- [readyAnimationName](dos-h0074-readyAnimationName.html)  Ready?のアニメーション名
- [readyColor](dos-h0075-readyColor.html)  Ready?の先頭色設定
- [readyHtml](dos-h0080-readyHtml.html)  Ready?の文字設定
- [finishView](dos-h0023-finishView.html)  フルコンボ演出の有無
- [keyRetry](dos-h0039-keyRetry.html)  リトライを行うショートカットキーのキーコード
- [keyTitleBack](dos-h0040-keyTitleBack.html)  タイトルバックを行うショートカットキーのキーコード

## ⚓️ タイトル・結果画面の初期設定
- [**commentVal**](dos-h0066-commentVal.html)  コメント表示
- [commentAutoBr](dos-h0067-commentAutoBr.html)  コメント表示時に改行タグを自動挿入する設定
- [commentExternal](dos-h0068-commentExternal.html)  コメントを本体の外部に置く設定
- [masktitleButton](dos-h0043-masktitleButton.html)  タイトル画面上のボタン群の有効/無効設定
- [resultDelayFrame](dos-h0076-resultDelayFrame.html)  CLEARED/FAILEDが表示されるまでの遅延フレーム数
- [maskresultButton](dos-h0044-maskresultButton.html)  リザルト画面上のボタン群の有効/無効設定
- [resultMotionSet](dos-h0048-resultMotionSet.html)  リザルトモーションのON/OFF設定
- [**resultFormat**](dos-h0072-resultFormat.html)  リザルトデータのフォーマット設定

## 🏙 カスタムデータの取込
- [**customjs**](dos-h0019-customjs.html)  カスタムjsファイルの指定
- [**preloadImages**](dos-h0021-preloadImages.html)  画像ファイルの事前読み込み設定
- [**autoPreload**](dos-h0055-autoPreload.html)  画像ファイルの自動読み込み設定
- [**skinType**](dos-h0054-skinType.html)  スキン設定
- [settingType](dos-h0056-settingType.html)  共通設定名
- [backBright](dos-h0081-backBright.html)  背景の明暗状態

## 🍂 デフォルトデザインの利用有無
- [**customTitleUse**](dos-h0025-customTitleUse.html)  タイトルの曲名文字
- [customTitleArrowUse](dos-h0026-customTitleArrowUse.html)  タイトルの背景矢印
- [customTitleAnimationUse](dos-h0078-customTitleAnimationUse.html)  タイトルのアニメーション設定
- [customBackUse](dos-h0027-customBackUse.html)  背景(プレイ画面以外)
- [customBackMainUse](dos-h0028-customBackMainUse.html)  背景(プレイ画面)
- [customReadyUse](dos-h0029-customReadyUse.html)  プレイ開始時演出

## 🌟 タイトル曲名文字(デフォルトデザイン)のエフェクト
- [**titlesize**](dos-h0030-titlesize.html)  文字サイズ
- [**titlefont**](dos-h0031-titlefont.html)  フォント
- [titlegrd / titlearrowgrd](dos-h0032-titlegrd.html)  グラデーション
- [titlepos](dos-h0033-titlepos.html)  X, Y座標位置
- [**titlelineheight**](dos-h0034-titlelineheight.html)  複数行の際の行間
- [**titleanimation**](dos-h0077-titleanimation.html)  アニメーション設定
- [titleanimationclass](dos-h0079-titleanimationclass.html)  アニメーションクラス設定

## 📋 クレジット関連
- [**tuning**](dos-h0017-tuning.html) (★)  製作者クレジット
- [**makerView**](dos-h0050-makerView.html)  譜面別の制作者名表示設定 
- [**hashTag**](dos-h0018-hashTag.html)  ハッシュタグ
- [releaseDate](dos-h0036-releaseDate.html)  作品公開日
