# 本体のバージョンアップ方法 (従来)
- Dancing☆Onigiri (CW Edition)では、  
基本的に更新ファイルを入れ替えることでバージョンアップができます。
- ただし、[カスタムjsを使ったスクリプト追加・変更](AboutCustomJs.html)（≠譜面データ）をしている場合、  
単純に入れ替えただけでは動作しない場合があります。  
[更新情報概要](UpdateInfo.html)や[アップグレードガイド](MigrationGuide.html)も必要に応じて確認してください。

## 事前に確認するもの
1. 最初に、本体のバージョンを確認します。  
バージョンは、Dan★Oniを起動したタイトル画面で確認できます。  
（この場合はVer3.9.0 (GitHub上はv3.9.0と表記) となります）
<img src="./wiki/danoniVersion.png" width="400">

## バージョンアップ方法（Gitを利用しない場合）
※メジャーバージョンアップを伴う場合、  
下記の「メジャーバージョンアップを含む更新を行う場合」もご覧ください。

2. [Releases](https://github.com/cwtickle/danoniplus/releases)へアクセスします。   
「**Files changed**」項目に、今回更新すべきファイルの一覧が載っています。  
「格納先のフォルダ」「対象のファイル名」「そのファイルの最終更新バージョン」を確認します。  
現在のバージョンより、**「最終更新」のバージョンが大きいファイル全て**が更新対象です。

<img src="./wiki/danoniReleaseC.png" width="100%">

通常は「danoni_main.js」のみをダウンロードすれば問題ありません。  
上記のように、他のファイルも対象になっている場合は合わせてダウンロードします。  

3. [danoniplus]フォルダの直下（ダウンロード直下のフォルダ）にある  
[css][js]フォルダの中身を一旦デスクトップ等へ退避（コピー）します。

4. 2.でダウンロードしたファイルを[css][js]フォルダへ上書きコピーします。  
※拡張子が.cssの場合は[css]フォルダへ、.jsの場合は[js]フォルダへ入れてください。  

5. Dan★Oniを起動し、バージョン番号が新しいものになっていればバージョンアップ完了です。  
一通りプレイして、問題がなければそのまま使用してください。  

## 注意点
「danoni_custom.js」「danoni_custom2.js」「danoni_setting.js」は  
利用者がカスタム可能なフォーマットファイルです。  
通常特別な記載がない限り、入れ替えの必要はありません。  
カスタムしている場合、個別に設定しているソースが上書きされてしまうため注意が必要です。 

最近はこのファイルを更新した場合、Release上は名前を「danoni_custom-template.js」としてアップしています。  

## 現バージョンと最新バージョンとの差分を確認する方法
- GitHub上のReleaseより確認可能です。  
ソース差分を確認する方向けで、通常意識する必要はありません。  
自身の現バージョンを確認し、それに対応するReleaseを見ると「XX Commits」というリンクがあります。  
これをクリックすると、最新バージョンとの差分が確認できます。  

- また、変更内容からリンクされている部分には、Pull RequestやIssueへのリンクがあり、
変更理由や背景を記録しています。  
<img src="./wiki/danoniReleaseB.png" width="600">

### Release上に表記される記号について
- Dancing☆Onigiri (CW Edition)では、以下のように区分することで  
変更内容がわかるように記述しています。  
- 変更点については、関連するPull Request/Issueの番号をリンクしています。  

|-|名称|概要|
|----|----|---|
|:star:|**New Features**|新機能について記述しています。|
|:hammer_and_wrench:|**Improvements**|新機能ではないが、コードの構成を見直した場合に記述します。|
|:beetle:|**Bug Fixes**|前バージョンの不具合を修正した場合に記述します。|
|:arrows_clockwise:|**Files changed**|直近に変更のあったファイルの一覧を記述します。|
|:notebook_with_decorative_cover:|**Documentation**|今回の機能変更に関連するWikiなどのリンク先を記述します。|
|:heart:|**Contributors**|新機能の起案、不具合情報の提供、Pull Requestを行ったなど<br>今回のリリースにご協力いただいた方を掲載します。|
|:four_leaf_clover:|**Remarks**|今回の変更に関する詳細や注意点があれば、記述します。|
|:fishing_pole_and_fish:|**Related Releases**|今回の変更の起因となったバージョン及び、同様の変更を行った過去バージョン・リンクを記述します。|
|:bulb:|**Recent Changes**|直近で更新されたバージョン・リンクを記述します。|

### メジャーバージョンアップを含む更新を行う場合
- v11からv12など、しばらく更新しなかった場合には`danoni_main.js`の他に  
変更が必要なファイルがある場合があります。  
事前に、ダンおにのフォルダ一式を別の場所にコピーしておくと良いです。

- Release画面より、「compare」ボタンを押して  
現在適用中のバージョンをクリックしてください。  
<img src="./wiki/danoniRelease6.png" width="600">

- 適用中のバージョンと最新を比較した画面が表示されます。  
「files changed XX」と書かれた場所をクリックするとファイルの変更状況が見えるので、  
さらに「XX changed files」のリンクをクリックしてください。  
変更が必要なファイルの一覧が表示されます。
<img src="./wiki/danoniRelease7.png" width="600">

- この一覧より、拡張子が「.js」「.css」に変更があったファイルで、  
ダウンロードしていないものがあれば最新の「Release」より、  
「Source code(zip)」一式をダウンロードして表示されたファイルを上書きしてください。  
(ただし、「danoni_custom.js」「danoni_custom2.js」「danoni_setting.js」は  
中身を確認したうえで上書きが必要か確認してください。通常は上書き不要です。)
<img src="./wiki/danoniRelease8.png" width="600">

- メジャーバージョンアップの場合、直近のRelease状況（Recent Changes）や  
[アップグレードガイド](MigrationGuide.html)を参照して、他に変更が必要な箇所が無いか確認してから  
更新を行ってください。