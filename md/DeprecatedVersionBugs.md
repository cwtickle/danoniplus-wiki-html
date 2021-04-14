# 更新を終了したバージョンの不具合情報
- 可能であれば、[アップグレードガイド](MigrationGuide.html)を参考にサポートバージョンへの更新を推奨しますが、  
作品の変更状況によっては、それができない場合があります。  
その場合でも対処ができるように、情報を記載しておきます。
- 更新終了時の最終バージョンでの不具合情報です。  
それ以前のバージョンでは、別の不具合が残っている可能性があります。  

## v18
- 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まって表示される ⇒ ( [v21.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/1044) )

## v17
- 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まって表示される ⇒ ( [v21.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/1044) )

## v16
- 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まって表示される ⇒ ( [v21.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/1044) )

## v15
- 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まって表示される ⇒ ( [v21.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/1044) )
- 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、  
通常矢印の判定が優先されてしまう ⇒ ( [v18.7.1](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.1), [v18.7.2](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.2) / [Fix](https://github.com/cwtickle/danoniplus/compare/v17.5.7...v17.5.8) )
- カスタムjs, スキンjsが多重読込され変数エラーが発生する可能性がある ⇒ ( [v18.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/917) )
- 曲終了直後にリトライキーを押すとALL0のリザルトが表示される ⇒ ( [v18.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.6.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/908) )
- Display:Colorのボタンが無効化されていた場合に  
ColorTypeの挙動により、Display:Colorの切り替えができてしまう ⇒ ( [v18.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.3.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/892) )
- 速度データ(speed_change)が空の場合、データがあると判断されてしまい  
speed_changeが優先されてしまう ⇒ ( [v18.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.1.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/884) )

## v13
- 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まって表示される ⇒ ( [v21.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/1044) )
- 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、  
通常矢印の判定が優先されてしまう ⇒ ( [v18.7.1](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.1), [v18.7.2](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.2) / [Fix](https://github.com/cwtickle/danoniplus/compare/v17.5.7...v17.5.8) )
- カスタムjs, スキンjsが多重読込され変数エラーが発生する可能性がある ⇒ ( [v18.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/917) )
- 曲終了直後にリトライキーを押すとALL0のリザルトが表示される ⇒ ( [v18.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.6.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/908) )
- 速度データ(speed_change)が空の場合、データがあると判断されてしまい  
speed_changeが優先されてしまう ⇒ ( [v18.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.1.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/884) )
- 矢印塗りつぶし有、ステップゾーンをOFFにした場合に矢印塗りつぶし部分が残る ⇒ ( [v17.4.3](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.3) / [Fix](https://github.com/cwtickle/danoniplus/compare/v16.4.3...v16.4.4) )
- 一部変数が初期化されていないため、strictモードが有効化できない ⇒ ( [v17.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/855) )
- ツール値出力時、譜面未定義の時間表示がおかしくなる ⇒ ( [v17.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/858) )
- tuningのみ指定があった場合に制作者リンクが出ない ⇒ ( [v17.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.3.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/850) )
- リトライ時に稀に早回しになる ⇒ ( [v16.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v16.2.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/810) )

## v12
- 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まって表示される ⇒ ( [v21.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/1044) )
- 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、  
通常矢印の判定が優先されてしまう ⇒ ( [v18.7.1](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.1), [v18.7.2](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.2) / [Fix](https://github.com/cwtickle/danoniplus/compare/v17.5.7...v17.5.8) )
- カスタムjs, スキンjsが多重読込され変数エラーが発生する可能性がある ⇒ ( [v18.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/917) )
- 曲終了直後にリトライキーを押すとALL0のリザルトが表示される ⇒ ( [v18.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.6.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/908) )
- 速度データ(speed_change)が空の場合、データがあると判断されてしまい  
speed_changeが優先されてしまう ⇒ ( [v18.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.1.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/884) )
- 矢印塗りつぶし有、ステップゾーンをOFFにした場合に矢印塗りつぶし部分が残る ⇒ ( [v17.4.3](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.3) / [Fix](https://github.com/cwtickle/danoniplus/compare/v16.4.3...v16.4.4) )
- 一部変数が初期化されていないため、strictモードが有効化できない ⇒ ( [v17.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/855) )
- ツール値出力時、譜面未定義の時間表示がおかしくなる ⇒ ( [v17.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/858) )
- tuningのみ指定があった場合に制作者リンクが出ない ⇒ ( [v17.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.3.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/850) )
- リトライ時に稀に早回しになる ⇒ ( [v16.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v16.2.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/810) )
- CustomGauge使用時にクリア失敗時のリザルトモーションが使用できない ⇒ ( [v15.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.3.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/751) )
- プレイ中にブラウザのショートカットが動作してしまう ⇒ ( [v15.2.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/741) )
- 通常キーであらかじめデフォルトセットされているキーコンフィグパターンと  
異なるキーを割り当てた際、初回保存時のみそのキーがリセットされる ⇒ ( [v15.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/738) )
- 特殊キーの後に通常キーの譜面があると譜面選択ができなくなる ⇒ ( [v15.1.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.1.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/729) )

## v11
- 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まって表示される ⇒ ( [v21.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/1044) )
- 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、  
通常矢印の判定が優先されてしまう ⇒ ( [v18.7.1](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.1), [v18.7.2](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.2) / [Fix](https://github.com/cwtickle/danoniplus/compare/v17.5.7...v17.5.8) )
- カスタムjs, スキンjsが多重読込され変数エラーが発生する可能性がある ⇒ ( [v18.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/917) )
- 曲終了直後にリトライキーを押すとALL0のリザルトが表示される ⇒ ( [v18.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.6.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/908) )
- 速度データ(speed_change)が空の場合、データがあると判断されてしまい  
speed_changeが優先されてしまう ⇒ ( [v18.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.1.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/884) )
- 矢印塗りつぶし有、ステップゾーンをOFFにした場合に矢印塗りつぶし部分が残る ⇒ ( [v17.4.3](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.3) / [Fix](https://github.com/cwtickle/danoniplus/compare/v16.4.3...v16.4.4) )
- 一部変数が初期化されていないため、strictモードが有効化できない ⇒ ( [v17.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/855) )
- tuningのみ指定があった場合に制作者リンクが出ない ⇒ ( [v17.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.3.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/850) )
- リトライ時に稀に早回しになる ⇒ ( [v16.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v16.2.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/810) )
- CustomGauge使用時にクリア失敗時のリザルトモーションが使用できない ⇒ ( [v15.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.3.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/751) )
- プレイ中にブラウザのショートカットが動作してしまう ⇒ ( [v15.2.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/741) )
- 通常キーであらかじめデフォルトセットされているキーコンフィグパターンと  
異なるキーを割り当てた際、初回保存時のみそのキーがリセットされる ⇒ ( [v15.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/738) )
- 特殊キーの後に通常キーの譜面があると譜面選択ができなくなる ⇒ ( [v15.1.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.1.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/729) )
- フリーズ始点判定有効時、シャキン以下の判定関数に  
差分フレーム数としてマイナス値が渡せていない ⇒ ( [v14.3.4](https://github.com/cwtickle/danoniplus/releases/tag/v14.3.4) / [Fix](https://github.com/cwtickle/danoniplus/pull/684) )

## v10
- 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まって表示される ⇒ ( [v21.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/1044) )
- 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、  
通常矢印の判定が優先されてしまう ⇒ ( [v18.7.1](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.1), [v18.7.2](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.2) / [Fix](https://github.com/cwtickle/danoniplus/compare/v17.5.7...v17.5.8) )
- カスタムjs, スキンjsが多重読込され変数エラーが発生する可能性がある ⇒ ( [v18.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/917) )
- 曲終了直後にリトライキーを押すとALL0のリザルトが表示される ⇒ ( [v18.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.6.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/908) )
- 速度データ(speed_change)が空の場合、データがあると判断されてしまい  
speed_changeが優先されてしまう ⇒ ( [v18.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.1.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/884) )
- 矢印塗りつぶし有、ステップゾーンをOFFにした場合に矢印塗りつぶし部分が残る ⇒ ( [v17.4.3](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.3) / [Fix](https://github.com/cwtickle/danoniplus/compare/v16.4.3...v16.4.4) )
- 一部変数が初期化されていないため、strictモードが有効化できない ⇒ ( [v17.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/855) )
- tuningのみ指定があった場合に制作者リンクが出ない ⇒ ( [v17.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.3.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/850) )
- リトライ時に稀に早回しになる ⇒ ( [v16.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v16.2.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/810) )
- CustomGauge使用時にクリア失敗時のリザルトモーションが使用できない ⇒ ( [v15.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v15.3.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/751) )
- プレイ中にブラウザのショートカットが動作してしまう ⇒ ( [v15.2.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/741) )
- 通常キーであらかじめデフォルトセットされているキーコンフィグパターンと  
異なるキーを割り当てた際、初回保存時のみそのキーがリセットされる ⇒ ( [v15.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/738) )
- 特殊キーの後に通常キーの譜面があると譜面選択ができなくなる ⇒ ( [v15.1.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.1.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/729) )
- フリーズ始点判定有効時、シャキン以下の判定関数に  
差分フレーム数としてマイナス値が渡せていない ⇒ ( [v14.3.4](https://github.com/cwtickle/danoniplus/releases/tag/v14.3.4) / [Fix](https://github.com/cwtickle/danoniplus/pull/684) )
- キーコンフィグ画面で代替キーの無効化ができない ⇒ ( [v13.3.1](https://github.com/cwtickle/danoniplus/releases/tag/v13.3.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/647) )
- ローカルで直接htmlファイルを開いたときに矢印画像が表示されない ⇒ ( [v12.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.3.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/628) )
- ダミー矢印のヒット位置が前の通常矢印のヒット結果に引きずられる ⇒ ( [v12.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v12.2.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/623) )
- スコアを独自計算している場合、ハイスコア差分が計算されない ⇒ ( [v12.1.1](https://github.com/cwtickle/danoniplus/releases/tag/v12.1.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/616) )

## v9
- 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まって表示される ⇒ ( [v21.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/1044) )

## v8
- 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まって表示される ⇒ ( [v21.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/1044) )
- 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、  
通常矢印の判定が優先されてしまう ⇒ ( [v18.7.1](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.1), [v18.7.2](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.2) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.26...v9.4.27) )
- カスタムjsが多重読込され変数エラーが発生する可能性がある ⇒ ( [v18.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/917) )
- 曲終了直後にリトライキーを押すとALL0のリザルトが表示される ⇒ ( [v18.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.6.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/908) )
- 速度データ(speed_change)が空の場合、データがあると判断されてしまい  
speed_changeが優先されてしまう ⇒ ( [v18.1.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.1.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/884) )
- 矢印塗りつぶし有、ステップゾーンをOFFにした場合に矢印塗りつぶし部分が残る ⇒ ( [v17.4.3](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.3) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.21...v9.4.22) )
- tuningのみ指定があった場合に制作者リンクが出ない ⇒ ( [v17.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.3.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/850) )
- リトライ時に稀に早回しになる ⇒ ( [v16.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v16.2.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/810) )
- プレイ中にブラウザのショートカットが動作してしまう ⇒ ( [v15.2.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/741) )
- 通常キーであらかじめデフォルトセットされているキーコンフィグパターンと  
異なるキーを割り当てた際、初回保存時のみそのキーがリセットされる ⇒ ( [v15.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/738) )
- 特殊キーの後に通常キーの譜面があると譜面選択ができなくなる ⇒ ( [v15.1.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.1.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/729) )
- フリーズ始点判定有効時、判定関数に差分フレーム数として  
マイナス値が渡せていない ⇒ ( [v14.3.4](https://github.com/cwtickle/danoniplus/releases/tag/v14.3.4) / [Fix](https://github.com/cwtickle/danoniplus/pull/684) )
- ローカルで直接htmlファイルを開いたときに矢印画像が表示されない ⇒ ( [v12.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.3.0) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.22...v9.4.23) )
- ロード画面でブロックすべきキーコントロールがブロックされない ⇒ ( [v11.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v11.2.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/581) )
- 譜面名未指定のときにリザルトコピー時のクレジットがundefinedになる ⇒ ( [v11.2.0](https://github.com/cwtickle/danoniplus/releases/tag/v11.2.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/583) )
- MacOS, iOS (Safari)においてエンコードした音楽データが再生できない ⇒ ( [v9.4.15](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.15) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.14...v9.4.15) )

## v7
- 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まって表示される ⇒ ( [v21.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/1044) )
- 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、  
通常矢印の判定が優先されてしまう ⇒ ( [v18.7.1](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.1), [v18.7.2](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.2) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.26...v9.4.27) )
- カスタムjsが多重読込され変数エラーが発生する可能性がある ⇒ ( [v18.7.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/917) )
- 曲終了直後にリトライキーを押すとALL0のリザルトが表示される ⇒ ( [v18.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.6.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/908) )
- 矢印塗りつぶし有、ステップゾーンをOFFにした場合に矢印塗りつぶし部分が残る ⇒ ( [v17.4.3](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.3) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.21...v9.4.22) )
- tuningのみ指定があった場合に制作者リンクが出ない ⇒ ( [v17.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.3.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/850) )
- リトライ時に稀に早回しになる ⇒ ( [v16.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v16.2.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/810) )
- プレイ中にブラウザのショートカットが動作してしまう ⇒ ( [v15.2.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/741) )
- 通常キーであらかじめデフォルトセットされているキーコンフィグパターンと  
異なるキーを割り当てた際、初回保存時のみそのキーがリセットされる ⇒ ( [v15.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/738) )
- 特殊キーの後に通常キーの譜面があると譜面選択ができなくなる ⇒ ( [v15.1.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.1.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/729) )
- フリーズ始点判定有効時、判定関数に差分フレーム数として  
マイナス値が渡せていない ⇒ ( [v14.3.4](https://github.com/cwtickle/danoniplus/releases/tag/v14.3.4) / [Fix](https://github.com/cwtickle/danoniplus/pull/684) )
- ローカルで直接htmlファイルを開いたときに矢印画像が表示されない ⇒ ( [v12.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.3.0) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.22...v9.4.23) )
- MacOS, iOS (Safari)においてWeb Audio APIが動作しない ⇒ ( [v10.1.1](https://github.com/cwtickle/danoniplus/releases/tag/v10.1.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/527) )

## v6
- 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まって表示される ⇒ ( [v21.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/1044) )
- 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、  
通常矢印の判定が優先されてしまう ⇒ ( [v18.7.1](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.1), [v18.7.2](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.2) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.26...v9.4.27) )
- 曲終了直後にリトライキーを押すとALL0のリザルトが表示される ⇒ ( [v18.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.6.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/908) )
- 矢印塗りつぶし有、ステップゾーンをOFFにした場合に矢印塗りつぶし部分が残る ⇒ ( [v17.4.3](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.3) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.21...v9.4.22) )
- tuningのみ指定があった場合に制作者リンクが出ない ⇒ ( [v17.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.3.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/850) )
- リトライ時に稀に早回しになる ⇒ ( [v16.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v16.2.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/810) )
- プレイ中にブラウザのショートカットが動作してしまう ⇒ ( [v15.2.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/741) )
- 通常キーであらかじめデフォルトセットされているキーコンフィグパターンと  
異なるキーを割り当てた際、初回保存時のみそのキーがリセットされる ⇒ ( [v15.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/738) )
- 特殊キーの後に通常キーの譜面があると譜面選択ができなくなる ⇒ ( [v15.1.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.1.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/729) )
- フリーズ始点判定有効時、判定関数に差分フレーム数として  
マイナス値が渡せていない ⇒ ( [v14.3.4](https://github.com/cwtickle/danoniplus/releases/tag/v14.3.4) / [Fix](https://github.com/cwtickle/danoniplus/pull/684) )
- ローカルで直接htmlファイルを開いたときに矢印画像が表示されない ⇒ ( [v12.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.3.0) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.22...v9.4.23) )
- MacOS, iOS (Safari)においてWeb Audio APIが動作しない ⇒ ( [v10.1.1](https://github.com/cwtickle/danoniplus/releases/tag/v10.1.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/527) )

## v5
- 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まって表示される ⇒ ( [v21.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/1044) )
- 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、  
通常矢印の判定が優先されてしまう ⇒ ( [v18.7.1](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.1), [v18.7.2](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.2) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.26...v9.4.27) )
- 曲終了直後にリトライキーを押すとALL0のリザルトが表示される ⇒ ( [v18.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.6.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/908) )
- 矢印塗りつぶし有、ステップゾーンをOFFにした場合に矢印塗りつぶし部分が残る ⇒ ( [v17.4.3](https://github.com/cwtickle/danoniplus/releases/tag/v17.4.3) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.21...v9.4.22) )
- tuningのみ指定があった場合に制作者リンクが出ない ⇒ ( [v17.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.3.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/850) )
- リトライ時に稀に早回しになる ⇒ ( [v16.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v16.2.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/810) )
- プレイ中にブラウザのショートカットが動作してしまう ⇒ ( [v15.2.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/741) )
- 特殊キーの後に通常キーの譜面があると譜面選択ができなくなる ⇒ ( [v15.1.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.1.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/729) )
- フリーズ始点判定有効時、判定関数に差分フレーム数として  
マイナス値が渡せていない ⇒ ( [v14.3.4](https://github.com/cwtickle/danoniplus/releases/tag/v14.3.4) / [Fix](https://github.com/cwtickle/danoniplus/pull/684) )
- ローカルで直接htmlファイルを開いたときに矢印画像が表示されない ⇒ ( [v12.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.3.0) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.22...v9.4.23) )
- MacOS, iOS (Safari)においてエンコードした音楽データが再生できない ⇒ ( [v9.4.15](https://github.com/cwtickle/danoniplus/releases/tag/v9.4.15) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.14...v9.4.15) )

## v4
- 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まって表示される ⇒ ( [v21.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/1044) )
- 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、  
通常矢印の判定が優先されてしまう ⇒ ( [v18.7.1](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.1), [v18.7.2](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.2) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.26...v9.4.27) )
- 曲終了直後にリトライキーを押すとALL0のリザルトが表示される ⇒ ( [v18.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.6.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/908) )
- tuningのみ指定があった場合に制作者リンクが出ない ⇒ ( [v17.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.3.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/850) )
- リトライ時に稀に早回しになる ⇒ ( [v16.2.1](https://github.com/cwtickle/danoniplus/releases/tag/v16.2.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/810) )
- プレイ中にブラウザのショートカットが動作してしまう ⇒ ( [v15.2.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/741) )
- 特殊キーの後に通常キーの譜面があると譜面選択ができなくなる ⇒ ( [v15.1.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.1.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/729) )
- ローカルで直接htmlファイルを開いたときに矢印画像が表示されない ⇒ ( [v12.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.3.0) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.22...v9.4.23) )
- MacOS, iOS (Safari)においてWeb Audio APIが動作しない ⇒ ( [v10.1.1](https://github.com/cwtickle/danoniplus/releases/tag/v10.1.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/527) )

## v3
- 空の矢印データを含む譜面にS-Randomをかけるとフルコン演出が早まって表示される ⇒ ( [v21.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/1044) )
- 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、  
通常矢印の判定が優先されてしまう ⇒ ( [v18.7.1](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.1), [v18.7.2](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.2) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.26...v9.4.27) )
- 曲終了直後にリトライキーを押すとALL0のリザルトが表示される ⇒ ( [v18.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.6.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/908) )
- tuningのみ指定があった場合に制作者リンクが出ない ⇒ ( [v17.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v17.3.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/850) )
- プレイ中にブラウザのショートカットが動作してしまう ⇒ ( [v15.2.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/741) )
- ローカルで直接htmlファイルを開いたときに矢印画像が表示されない ⇒ ( [v12.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.3.0) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.22...v9.4.23) )
- MacOS, iOS (Safari)が非対応 ⇒ ( [v10.1.1](https://github.com/cwtickle/danoniplus/releases/tag/v10.1.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/527) )
- 速度変化が同一フレームにあると正常に動作しなくなる ⇒ ( [v8.7.3](https://github.com/cwtickle/danoniplus/releases/tag/v8.7.3) / [Fix](https://github.com/cwtickle/danoniplus/pull/477) )
- エスケープ文字の適用順序誤りにより、一部の文字が使用できない ⇒ ( [v8.7.2](https://github.com/cwtickle/danoniplus/releases/tag/v8.7.2) / [Fix](https://github.com/cwtickle/danoniplus/compare/v8.7.1...v8.7.2) )
- メイン画面で曲中リトライキーを連打した場合に譜面がずれることがある ⇒ ( [v8.0.4](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.4) / [Fix](https://github.com/cwtickle/danoniplus/pull/433) )
- ゲームオーバー時の200ミリ秒遅延により、  
ハイスコア表示がおかしくなることがある ⇒ ( [v8.0.2](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/428) )
- 速度変化が補正込みで負のフレームにあるときに動作しなくなる ⇒ ( [v8.0.1](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/426) )
- back_data, mask_dataで0フレームが指定された場合に動作しないことがある ⇒ ( [v7.5.1](https://github.com/cwtickle/danoniplus/releases/tag/v7.5.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/388) )
- リザルト画面で、フェードアウト中にTitleBack/Retryすると  
フェードアウト状態が引き継がれてしまう ⇒ ( [v7.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v7.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/384) )
- フェードイン時に個別加速が掛からない ⇒ ( [v6.5.1](https://github.com/cwtickle/danoniplus/releases/tag/v6.5.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/363) )
- フリーズアローのみの譜面が再生できない ⇒ ( [v5.12.2](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/343) )

## v2
- 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、  
通常矢印の判定が優先されてしまう ⇒ ( [v18.7.1](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.1), [v18.7.2](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.2) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.26...v9.4.27) )
- 曲終了直後にリトライキーを押すとALL0のリザルトが表示される ⇒ ( [v18.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.6.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/908) )
- プレイ中にブラウザのショートカットが動作してしまう ⇒ ( [v15.2.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/741) )
- ローカルで直接htmlファイルを開いたときに矢印画像が表示されない ⇒ ( [v12.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.3.0) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.22...v9.4.23) )
- MacOS, iOS (Safari)が非対応 ⇒ ( [v10.1.1](https://github.com/cwtickle/danoniplus/releases/tag/v10.1.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/527) )
- 速度変化が同一フレームにあると正常に動作しなくなる ⇒ ( [v8.7.3](https://github.com/cwtickle/danoniplus/releases/tag/v8.7.3) / [Fix](https://github.com/cwtickle/danoniplus/pull/477) )
- エスケープ文字の適用順序誤りにより、一部の文字が使用できない ⇒ ( [v8.7.2](https://github.com/cwtickle/danoniplus/releases/tag/v8.7.2) / [Fix](https://github.com/cwtickle/danoniplus/compare/v8.7.1...v8.7.2) )
- メイン画面で曲中リトライキーを連打した場合に譜面がずれることがある ⇒ ( [v8.0.4](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.4) / [Fix](https://github.com/cwtickle/danoniplus/pull/433) )
- ゲームオーバー時の200ミリ秒遅延により、  
ハイスコア表示がおかしくなることがある ⇒ ( [v8.0.2](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/428) )
- 速度変化が補正込みで負のフレームにあるときに動作しなくなる ⇒ ( [v8.0.1](https://github.com/cwtickle/danoniplus/releases/tag/v8.0.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/426) )
- back_data, mask_dataで0フレームが指定された場合に動作しないことがある ⇒ ( [v7.5.1](https://github.com/cwtickle/danoniplus/releases/tag/v7.5.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/388) )
- リザルト画面で、フェードアウト中にTitleBack/Retryすると  
フェードアウト状態が引き継がれてしまう ⇒ ( [v7.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v7.4.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/384) )
- フェードイン時に個別加速が掛からない ⇒ ( [v6.5.1](https://github.com/cwtickle/danoniplus/releases/tag/v6.5.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/363) )
- フリーズアローのみの譜面が再生できない ⇒ ( [v5.12.2](https://github.com/cwtickle/danoniplus/releases/tag/v5.12.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/343) )

## v1
- 同一レーン上に通常矢印とフリーズアローが短い間隔で存在するとき、  
通常矢印の判定が優先されてしまう ⇒ ( [v18.7.1](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.1), [v18.7.2](https://github.com/cwtickle/danoniplus/releases/tag/v18.7.2) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.26...v9.4.27) )
- 曲終了直後にリトライキーを押すとALL0のリザルトが表示される ⇒ ( [v18.6.0](https://github.com/cwtickle/danoniplus/releases/tag/v18.6.0) / [Fix](https://github.com/cwtickle/danoniplus/pull/908) )
- プレイ中にブラウザのショートカットが動作してしまう ⇒ ( [v15.2.2](https://github.com/cwtickle/danoniplus/releases/tag/v15.2.2) / [Fix](https://github.com/cwtickle/danoniplus/pull/741) )
- ローカルで直接htmlファイルを開いたときに矢印画像が表示されない ⇒ ( [v12.3.0](https://github.com/cwtickle/danoniplus/releases/tag/v12.3.0) / [Fix](https://github.com/cwtickle/danoniplus/compare/v9.4.22...v9.4.23) )
- MacOS, iOS (Safari)が非対応 ⇒ ( [v10.1.1](https://github.com/cwtickle/danoniplus/releases/tag/v10.1.1) / [Fix](https://github.com/cwtickle/danoniplus/pull/527) )  
※v1ではWeb Audio APIを使用していないため、  
　フェードイン時に譜面がずれることがあります。(Web Audio APIはv2以降の対応)