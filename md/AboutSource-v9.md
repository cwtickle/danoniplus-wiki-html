# ソースの構成 (v1～v9)
Dancing☆Onigiri(CW Edition)ソースの各ファイルの詳細説明です。  
中身の説明は別ページにて。  

|第1階層|第2階層|必須|内容|
|----|----|----|----|
|css|danoni_main.css|*|矢印の色変化、Resultモーションなどで使用。<br>バージョンアップのタイミングでの変更が時々あるので、ページ個別のcssとは分けることを推奨。|
|danoni|---||Dan☆Oniの動作サンプルページ。|
|img|---|*|画像ファイル。矢印やAAキャラクタなどのセット。|
|img|cursor.png|*|キーコンフィグのカーソル|
|img|frzbar.png|*|フリーズアローバー、ライフゲージ本体|
|img|borderline.png|*|ノルマ制ゲージのとき、ボーダー位置を表示する画像。|
|img|arrow_500.png|*|矢印本体|
|img|arrowShadow_500.png|*|矢印の裏側描画用。フリーズアローで使う。|
|img|c_600.png|*|AA(しぃ)|
|img|giko_600.png|*|AA(ギコ)|
|img|iyo_600.png|*|AA(ぃょぅ)|
|img|monar_600.png|*|AA(モナー)|
|img|morara_600.png|*|AA(モララー)|
|img|onigiri_600.png|*|AA(おにぎり)|
|img|aaShadow_500.png|*|AAキャラクタの裏側描画用。フリーズアローで使う。|
|js|---|*|Dancing☆Onigiri(CW Edition)のソースの多くはここで記載されている。<br>danoni_main.jsは必須。他のcustomファイルは作品別に設定を分けたり、名前を変えたりできる。[譜面ヘッダー#customjs](dos-h0019-customjs.html)にて設定が可能。|
|js|danoni_main.js|*|メインソース。danoni_main.cssとセットで使用。<br>ライブラリのような位置づけで、通常このファイルがバージョンアップのたびに差し替えられる。<br>改造したいときは、下記customファイルの利用を推奨。|
|js|danoni_setting.js|*|ユーザ共通設定。<br>ver3.0.0より追加。作品共通で設定する項目に使用する。|
|js|danoni_custom.js|*|ユーザカスタム用ソースその１（共通カスタム）。<br>danoni_main.jsから呼び出して使う。<br>名前変更も可能だが、その場合は[譜面ヘッダー#customjs](dos-h0019-customjs.html)にて設定が必須。|
|js|danoni_custom2.js||ユーザカスタム用ソースその２（作品別カスタム）。<br>danoni_main.jsから呼び出して使う。利用は任意。<br>使用の際は、[譜面ヘッダー#customjs](dos-h0019-customjs.html)にて設定しないと使用できない。|
|music|---|*|音楽ファイルの格納場所。[譜面ヘッダー#musicFolder](dos-h0013-musicFolder.html)にて作品別に変えることができる。|
|music|nosound.mp3|*|最初から入っている無音ファイル。|