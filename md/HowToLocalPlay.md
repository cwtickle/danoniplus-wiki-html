# ローカルでのプレイ方法
- Chrome 79より、ローカル上での画像読込に制限が入り、  
既定の状態(htmlファイルをダブルクリックで起動)ではプレイできなくなりました。  
（ライフゲージ、矢印・フリーズアローが見えない状況になっている状態を指します。）

### 補足情報
- **ver12.3.0以降** (ver11はver11.4.3以降, ver9はver9.4.23以降)より、htmlファイルをそのまま開く場合は  
ソース直書きのバイナリ変換データを参照するようにしたため、  
**画像が表示されない問題は無くなりました。**  
- ローカルサーバーを立てる場合では**遅延の少ない Web Audio API が常時使用できる  
といった利点**もあるため、ページ自体は残しておきます。  
- 環境の違いによるオーディオ再生方法の違いについては[オーディオ仕様](Audio.html)をご覧ください。

## 対応方法
![81-0local](./wiki/81-0local.png) 

最初に以下A, Bどちらかの設定が必要です。  
将来性を考慮し、Aの方法で作ることを推奨します。  
※ver12.3.0の変更により、Bの方法は対策としてほぼ意味がなくなりました。  
　（そのままhtmlファイルを開いてプレイが可能なため）

## A. ローカルサーバーを立てる
- 1～3は初回のみです。次回以降は[4から](#4-apache%E3%81%AE%E8%B5%B7%E5%8B%95)行えばOKです。  
うまく行かない場合は[こちら](HowToLocalPlay-Appendix.html)もご覧ください。

### 1. Xampp をダウンロード
https://www.apachefriends.org/jp/index.html

### 2. Xampp をインストール
- 基本的に「Next」を押すだけでインストール可能です。
<details>
<summary>詳細は[ここをクリック]してください。</summary>

![81-0xampp](./wiki/81-0xampp.png)  
![81-1xampp](./wiki/81-1xampp.png)  
![81-2xampp](./wiki/81-2xampp.png)  
![81-3xampp](./wiki/81-3xampp.png)  
![81-4xampp](./wiki/81-4xampp.png)  
![81-5xampp](./wiki/81-5xampp.png)  
![81-6xampp](./wiki/81-6xampp.png)  
![81-7xampp](./wiki/81-7xampp.png)  
![81-8xampp](./wiki/81-8xampp.png)  
![81-9xampp](./wiki/81-9xampp.png)  
</details>

### 3. Xampp（Apache）の設定
- Config -> httpd.conf をクリックします。
![81-10xampp](./wiki/81-10xampp.png)  

- Windowsの場合、次回以降すぐに起動できるよう、「ピン留め」しておくと便利です。
![81-11xampp](./wiki/81-11xampp.png)

- DocumentRoot 及び Directoryの値を、ダンおにを作成しているフォルダーに設定します。  
※すでにXamppが導入済みで、Directoryを変えたくない場合は[こちら](HowToLocalPlay-Appendix.html)をご覧ください。

- 例) C:/danoniplus　※"￥"は"/"に変更してください。  
![81-12xampp](./wiki/81-12xampp.png)  

### 4. Apacheの起動
- Apacheの「Start」ボタンを押してApacheを起動します。
![81-13xampp](./wiki/81-13xampp.png)

### 5. ブラウザを起動して、ダンおにが起動することを確認します。
例えば、`C:\danoniplus\danoni\danoni1.html`にあるファイルを確認するときは  
`http://localhost/danoni/danoni1.html`へアクセスすればOKです。  
![81-14xampp](./wiki/81-14xampp.png)

- danoni_main.jsを入れ替えるときはキャッシュが残っていることがあります。  
スーパーリロード（Ctrl + F5キー）を行うか、  
.htaccessというファイルを DocumentRoot に指定したフォルダに置いてください。  
中身は下記のように記載します。
```
FileEtag None
RequestHeader unset If-Modified-Since
Header set Cache-Control no-store
```
- 終了するときは、Apacheの「Stop」ボタンを押して終了してください。
![81-13xampp](./wiki/81-13xampp.png)

参考
https://qiita.com/massie_g/items/2913066e596dae197539

## B. Chromeの設定変更により回避する
### 1. Chrome の設定変更

Chromeの「設定」を開きます。  
詳細設定 > システム より、「Google Chrome を閉じた際にバックグラウンド アプリの処理を続行する
」の**チェックを外します。**  
※下記は Chrome 79の場合であり、後継バージョンの場合は表示が異なる場合があります。

![92local](./wiki/92local.png)

### 2. Chromeの終了

Chromeの画面を全て閉じます。

### 3. Chromeに起動オプションをつけたショートカットを作成

既存のChromeのショートカットをコピーします。  
![93local](./wiki/93local.png)

コピーしたショートカットを右クリック -> プロパティ を選びます。  
「リンク先」の最後に、「 --allow-file-access-from-files」を追加します。  
![94local](./wiki/94local.png)

「詳細設定」ボタンを押し、「管理者として実行」にチェックを入れて「OK」を押します。
![95local](./wiki/95local.png)

作成したショートカットよりChromeを起動して、その中でダンおに用のHTMLファイルを開けば、  
ローカルでもプレイが可能になります。  
※この状態の場合、ドラッグ＆ドロップが利かないため、  
　面倒かもしれませんがフォルダーをコピーしてURLエリアへ貼り付けてください。

例）C:/danoni/sample/danoni1.html
