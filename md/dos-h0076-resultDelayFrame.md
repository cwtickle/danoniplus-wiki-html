[← 譜面ヘッダー仕様に戻る](dos_header.html)
## resultDelayFrame
### 使い方
```
|resultDelayFrame=1000|
```
### 説明
結果表示の「CLEARED」「FAILED」の表示を遅延させるフレーム数を指定します。  
デフォルトは0フレームです。  
readyDelayFrameと同様、CSSの`animationDelay`属性を使用していますが、  
こちらは指定が無い場合、属性の付与を行いません。  
また、途中終了した場合もこの設定の有無によらず、同様に0フレーム扱いとして処理します。

### 関連項目
- [readyDelayFrame](dos-h0052-readyDelayFrame.html)  Ready?が表示されるまでの遅延フレーム数
- [**customjs**](dos-h0019-customjs.html)  カスタムjsファイルの指定

### 更新履歴

|Version|変更内容|
|----|----|
|[v16.4.0](https://github.com/cwtickle/danoniplus/releases/tag/v16.4.0)|初回実装|