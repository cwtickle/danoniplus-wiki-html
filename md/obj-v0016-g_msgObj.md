[← オブジェクトリファレンスに戻る](ObjectReferenceIndex.html)  

## g_msgObj / g_lbl_msgObj

### 概要
- オンマウステキスト、確認メッセージを管理するオブジェクト。
- `g_local_msgObj`は`g_msgObj`のローカル版で、  
`g_local_msgObj`側のプロパティが優先される設定になっている。

### 生成タイミング
- 初回起動時

### プロパティ
```javascript
const g_msgObj = {

    reload: `ページを再読込します。`,
    howto: `ゲーム画面の見方や設定の詳細についてのページへ移動します（GitHub Wiki）。`,
    dataReset: `この作品で保存されているハイスコアや\nAdjustment情報等をリセットします。`,
    github: `Dancing☆Onigiri (CW Edition)のGitHubページへ移動します。`,
    security: `Dancing☆Onigiri (CW Edition)のサポート情報ページへ移動します。`,

    dataResetConfirm: `この作品のローカル設定をクリアします。よろしいですか？\n(ハイスコアやAdjustment等のデータがクリアされます)`,
    keyResetConfirm: `キーを初期配置に戻します。よろしいですか？`,

    difficulty: `譜面を選択します。`,
    speed: `矢印の流れる速度を設定します。`,
    motion: `矢印の速度を一定ではなく、\n変動させるモーションをつけるか設定します。`,
    reverse: `矢印の流れる向きを設定します。`,
    scroll: `各レーンのスクロール方向をパターンに沿って設定します。`,
    shuffle: `譜面を左右反転したり、ランダムにします。\nランダムにした場合は別譜面扱いとなり、ハイスコアは保存されません。`,
    autoPlay: `オートプレイや一部キーを自動で打たせる設定を行います。\nオートプレイ時はハイスコアを保存しません。`,
    gauge: `クリア条件を設定します。`,
    adjustment: `タイミングにズレを感じる場合、\n数値を変えることでズレを直すことができます。`,
    fadein: `譜面を途中から再生します。\n途中から開始した場合はハイスコアを保存しません。`,
    volume: `ゲーム内の音量を設定します。`,

    graph: `速度変化や譜面密度状況、\n譜面の難易度など譜面の詳細情報を表示します。`,
    dataSave: `ハイスコア、リバース設定、\nキーコンフィグの保存の有無を設定します。`,
    toDisplay: `プレイ画面上のオブジェクトの\n表示・非表示（一部透明度）を設定します。`,
    toSettings: `SETTINGS画面へ戻ります。`,

    d_stepzone: `ステップゾーンの表示`,
    d_judgment: `判定キャラクタ・コンボの表示`,
    d_fastslow: `Fast/Slow表示`,
    d_lifegauge: `ライフゲージの表示`,
    d_score: `現時点の判定数を表示`,
    d_musicinfo: `音楽情報（時間表示含む）`,
    d_filterline: `Hidden+, Sudden+使用時のフィルターの境界線表示`,
    d_speed: `途中変速、個別加速の有効化設定`,
    d_color: `色変化の有効化設定`,
    d_lyrics: `歌詞表示の有効化設定`,
    d_background: `背景・マスクモーションの有効化設定`,
    d_arroweffect: `矢印・フリーズアローモーションの有効化設定`,
    d_special: `作品固有の特殊演出の有効化設定`,

    appearance: `流れる矢印の見え方を制御します。`,
    opacity: `判定キャラクタ、コンボ数、Fast/Slow、Hidden+/Sudden+の\n境界線表示の透明度を設定します。`,

};
```