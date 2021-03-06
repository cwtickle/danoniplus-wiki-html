# バージョン管理ポリシー / Versioning Policy
- Dancing☆Onigiri (CW Edition)におけるバージョン管理ポリシーについて記述します。

## Version Numbering
- バージョンの付与方法は原則、[Semantic Versioning 2.0.0](https://semver.org/)に準じ、  
`x.y.z`(例：`18.9.3`)の形式で付与します。  
- サポートバージョンについては [Security Policy](../security/policy) をご覧ください。

## Major Version (x)
- 後方互換性が無い変更、大幅なコード改変を行った場合に番号`x`を上げます。
- また、前回メジャーバージョンを上げたときから100 Commit以上開きがあり、  
ソースの乖離が大きいと判断した場合、互換性の状況に関係なく番号`x`を上げることがあります。  
※ただし、機能追加や変更がある場合に限ります。
- ソースをカスタムしている場合は、[アップグレードガイド](MigrationGuide.html)を参照して  
バージョンアップするかを検討してください。

## Minor Version (y)
- 小規模な機能追加や変更が発生した場合に、**最新メジャーバージョンに限り**番号`y`を上げます。  
- 過去バージョンについてはこの数字が最も大きいものが修正対象です  
（サポート終了しているバージョンを除く）。  
※過去バージョンは機能追加や変更は原則行わず、バグフィックスなど必要最小限の変更のみ行います。
- 後方互換性は極力保っていますが、カスタムしている場合はその限りでない場合があります。  
主な変更点は[更新情報概要](UpdateInfo.html)や[Release](https://github.com/cwtickle/danoniplus/releases)に記載していますので、そちらをご覧ください。

## Revision / Patch Version (z)
- `x`や`y`で行われた機能追加・変更に対する（後方互換性のある）  
バグフィックスが行われた場合、番号`z`を上げます。  
- そのバグフィックスをサポートバージョンにも適用する場合は、  
サポートバージョンの番号`z`についても番号を上げます。
- 機能追加では無いもののソース管理上必要な機能やコード修正の場合、  
`y`ではなく`z`が上がることがあります。

## Alpha / Beta Version
- 実装機能が大きい場合に、バージョン名の後ろに`-M1`や`-RC`をつける場合があります。  
これらのバージョンは正規リリース前のもので、後方互換性は考慮されていません。
- `-M1`, `-M2`, ... が開発中のバージョン、`-RC`がリリース候補版であることを表します。  
リリース候補であっても、その後に互換性のない修正が入ることがありますのでご注意ください。

## バージョン番号付与後にリリースを取り消した場合
- リリース前に不具合が発覚し、それがバージョン番号付与後である場合は、  
リリースを取り下げて修正を実施した後、バージョン番号`z`を上げて対応します。 
  - 例) `14.3.0`を取り下げた場合、次回更新時は`14.3.1`としてリリースする。 
- リリースを取り下げた後に更新する内容が、小規模な機能追加や変更を伴う場合は  
バージョン番号`y`を上げて対応します。 
