# カスタムjs(スキンjs)による処理割込み
Dancing☆Onigiri(CW Edition)ソースでは、  
カスタムjsファイルやスキンjsファイルによる処理割込みを行うことで  
danoni_main.js を直接変更することなく、画面内のオブジェクトの情報を変更することができます。    
アクセスできるオブジェクトについては[DOM](DOM.html)、[ID一覧](idReferenceIndex.html)、[オブジェクト一覧](objectReferenceIndex.html)のページもご覧ください。  

なお、スキン用関数についてはフォントサイズや色変更などが  
CSSで制御できない場合に使用することを想定していますが、  
カスタムjsと同じような使い方をすることも可能です。

## タイトル画面 (titleInit)
![interrupt1](./wiki/interrupt1.png)

## 設定画面 (optionInit)
![interrupt2](./wiki/interrupt2.png)

## 設定(Display)画面 (settingsDisplayInit)
![interrupt3](./wiki/interrupt3.png)

## キーコンフィグ画面 (keyConfigInit)
![interrupt4](./wiki/interrupt4.png)

## 読込画面 (loadingScoreInit)
![interrupt5](./wiki/interrupt5.png)

## メイン画面 (mainInit)
![interrupt6](./wiki/interrupt6.png)

## 結果画面 (resultInit)
![interrupt7](./wiki/interrupt7.png)

