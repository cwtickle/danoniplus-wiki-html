# ソースの構成
Dancing☆Onigiri(CW Edition)ソースの各ファイルの詳細説明です。  
譜面設定については下記をご覧ください。
- [譜面本体仕様](dos_score.html) / [譜面ヘッダー仕様](dos_header.html) / [共通設定ファイル仕様](dos_setting.html) /   
[譜面エフェクト仕様](dos_effect.html) / [グラデーション仕様](dos-c0001-gradation.html)

|第1階層|第2階層|必須|内容|
|----|----|----|----|
|css|danoni_main.css|*|矢印の色変化、Resultモーションなどで使用。<br>バージョンアップのタイミングでの変更が時々あるので、ページ個別のcssとは分けることを推奨。|
|danoni|---||Dan☆Oniの動作サンプルページ。|
|img|---|*|画像ファイル。矢印やAAキャラクタなどのセット。|
|img|cursor.svg(png)|*|キーコンフィグのカーソル|
|img|frzbar.svg(png)|*|フリーズアローバー、ライフゲージ本体|
|img|borderline.svg(png)|*|ノルマ制ゲージのとき、ボーダー位置を表示する画像。|
|img|arrow.svg(png)|*|矢印本体|
|img|arrowShadow.svg(png)|*|矢印の裏側描画用。フリーズアローで使う。|
|img|c.svg(png)|*|AA(しぃ)|
|img|giko.svg(png)|*|AA(ギコ)|
|img|iyo.svg(png)|*|AA(ぃょぅ)|
|img|monar.svg(png)|*|AA(モナー)|
|img|morara.svg(png)|*|AA(モララー)|
|img|onigiri.svg(png)|*|AA(おにぎり)|
|img|aaShadow.svg(png)|*|AAキャラクタの裏側描画用。フリーズアローで使う。|
|js|---|*|Dancing☆Onigiri(CW Edition)のソースの多くはここで記載されている。<br>danoni_main.jsは必須。他のcustomファイルは作品別に設定を分けたり、名前を変えたりできる。[譜面ヘッダー#customjs](dos-h0019-customjs.html)にて設定が可能。|
|js|lib/danoni_constants.js|*|定数管理ファイル。danoni_main.jsとセットで更新される場合がある。|
|js|lib/danoni_legacy_function.js||過去互換関数。customで利用していない限りは不要。|
|js|lib/danoni_localbinary.js||ローカル起動用のデフォルト画像セット。<br>このファイルはサーバーにアップする必要はありません。|
|js|danoni_main.js|*|メインソース。danoni_main.cssとセットで使用。<br>ライブラリのような位置づけで、通常このファイルがバージョンアップのたびに差し替えられる。<br>改造したいときは、下記customファイルの利用を推奨。|
|js|danoni_setting.js||ユーザ共通設定。<br>ver3.0.0より追加。作品共通で設定する項目に使用する。|
|js|danoni_custom.js||ユーザカスタム用ソースその１（共通カスタム）。<br>danoni_main.jsから呼び出して使う。<br>名前変更も可能だが、その場合は[譜面ヘッダー#customjs](dos-h0019-customjs.html)にて設定が必須。|
|js|danoni_custom2.js||ユーザカスタム用ソースその２（作品別カスタム）。<br>danoni_main.jsから呼び出して使う。利用は任意。<br>使用の際は、[譜面ヘッダー#customjs](dos-h0019-customjs.html)にて設定しないと使用できない。|
|music|---|*|音楽ファイルの格納場所。[譜面ヘッダー#musicFolder](dos-h0013-musicFolder.html)にて作品別に変えることもできる他、v10からは`(..)`をファイル名の前に指定することでカレントディレクトリ指定も可能。|
|music|nosound.mp3|*|最初から入っている無音ファイル。|
|skin|---|*|スキン用のcss/jsファイルの格納場所。<br>danoni_skin_XXX.cssの形で指定。カレントディレクトリ指定も可能。|
|skin|danoni_skin_default.css|*|デフォルトスキン|
|skin|danoni_skin_default.js||デフォルトスキン拡張|
|skin|danoni_skin_light.css||白背景スキン|
|skin|danoni_skin_light.js||白背景スキン拡張|
|skin|danoni_skin_skyblue.css||スカイブルースキン|
|skin|danoni_skin_skyblue.js||スカイブルースキン拡張|
|skin|danoni_skin_background.css||背景用スキンテンプレート|
|skin|danoni_skin_background.js||背景用スキン拡張テンプレート|
|skin|danoni_skin_blank.css||スキン2つ目テンプレート|
|skin|danoni_skin_blank.js||スキン2つ目拡張テンプレート|