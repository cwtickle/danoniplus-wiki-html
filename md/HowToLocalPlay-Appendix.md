# ローカルでのプレイ方法(補足)
## 1. Xampp(Apache)のDocumentRootを変えずに設定する方法 (Windows)
- シンボリックリンクを使用します。  
ダンおにフォルダーが`C:\danoniplus`の場合、コマンドプロンプト もしくは PowerShell(管理者)にて下記のように指定します。
```Batchfile
mklink /D C:\danoniplus C:\xampp\apache\htdocs\danoniplus
```
※ C:\xampp\apache\htdocs にドキュメントルートがあることが前提です。(Xamppの既定値)

これにより、httpd.confを変更しなくても `http://localhost/danoniplus/`にアクセスすればダンおに用フォルダーへアクセスできます。

参考：
https://dev.classmethod.jp/etc/make_windows_symbolic_link/

## 2. フォルダーに全角（漢字・カタカナ・ひらがな等）が含まれている場合
- 直接フォルダー名を手打ちするとアクセスに失敗する可能性があります。
いずれかを試してみてください。

1. フォルダー名、ファイル名を全て半角英数字（ハイフン、アンダースコアは可）に置き換える（推奨）。
    - 実際にサーバーにアップロードするときは半角英数字にすることが多いため、名称を揃えることができるメリットがあります。
2. フォルダー名やファイル名を手打ちせず、Apacheを起動した状態で一旦`http://localhost`へアクセスする。
    - この場合、ダンおにフォルダーの一覧が下記のように表示されます。  
フォルダーから対象のファイルへたどって、プレイできることを確認してください。

![82-1xampp](./wiki/82-1xampp.png)  

## 3. Xampp(Apache)が起動できない場合
- Apacheではポート80番を利用していますが、他のアプリケーション（Skypeなど）で
すでにポート80番を使用している場合があります。

- 下記のリンクのように、Skype側のポートを変更することで解消できます。  
https://web-generalist.com/skype-port-off/

- 何らかの理由で、他のアプリケーションのポートが変更できない場合は、  
Xampp(Apache)側のポートを変更します。  
Xamppを開き、Config -> httpd.conf をクリックします。

![81-10xampp](./wiki/81-10xampp.png) 

- 下記のように「Listen 80」と書いてあるところを探し、  
「80」の部分を別の数字（例えば、10000）に直して保存します。

![82-2xampp](./wiki/82-2xampp.png) 

- Xamppに戻り、Apacheを開始してください。  
なおListenの数字を10000に変えた場合、アクセス先は`http://localhost:10000/`となります。  
(Listenの数字を変わると、この10000の部分を変える必要があります)