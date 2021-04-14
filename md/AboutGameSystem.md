# ゲーム画面の説明 (About Game System)
- [ゲーム内で使用できるショートカット](Shortcut.html)も合わせてご覧ください。

## GameTitle / ゲームタイトル
- Click Here!! を押してゲームをスタートします。  
※作品により、画面の見た目が異なる場合があります。  
(Press Click Here !! to start the game.)

![01game-title](./wiki/01game-title-1_v10.png)

## Settings / 設定画面
- 譜面(Difficulty)や矢印の流れる速度などを変更できます。  
(You can change the charts (Difficulty) and the speed of the sequences.
 In DanOni, we call the sequences "arrows".)  
- PLAYボタンを押すとゲームがスタートします。  
譜面のタイミングがずれるときは、Adjustmentの設定を上下させてみてください。

![11game-setting1](./wiki/11game-setting1-1_v10.png)

### Difficulty (譜面)
譜面が複数あれば、変更することができます。  
(Set the charts if the works have multiple charts.)

### Speed (速度)
1x から 10x の間で矢印の流れる速度を変更できます。  
※譜面により、これ以上(以下)の速度で矢印が流れてくる場合があります。  
(Set the speed of the sequences between 1x and 10x.)

### Motion (矢印の流れるモーションの変化)
矢印の速度を一定ではなく、変動させるモーションをつけるか設定します。  
(Set the motion of sequences to make it faster or slower on the way.)

|種類|内容|
|----|----|
|OFF|変化なし<br>(Same speed from beginning to end)|
|Boost|初めは初速、ステップゾーンに近づくにつれて速くなります。<br>(Initially initial speed, faster as it gets closer to the step zone)|
|Brake|初めは速く、ステップゾーンに近づくにつれて初速になります。<br>(Initially fast, and becomes initial speed as it gets closer to the step zone)|

### Reverse (矢印の流れる向き)
矢印の流れる向きを設定します。  
(Set the flow direction of the sequences.)

|種類|内容|
|----|----|
|OFF|下から上へ流れます。<br>両方にステップゾーンがある場合は一部上から下へも流れます。<br>(Generally, it flows from bottom to top.)|
|ON|上から下へ流れます。<br>両方にステップゾーンがある場合は、OFFの状態に対してそれぞれ逆になります。<br>(Generally, it flows from  top to bottom.)|

### Scroll (各レーンのスクロール方向の設定)
各レーンのスクロール方向をパターンに沿って設定します。  
(Set the scroll direction of each lane according to the pattern.)

|種類|内容|
|----|----|
|---|すべてのレーンが同じ方向に流れます。<br>(All lanes flow in the same direction.)|
|Cross|正、逆、正の順に流れるよう設定します。<br>(Generally, set the flow to be default, reverse, and default.)|
|Split|中央を境界として、スクロール方向を反転します。<br>(Reverses the scroll direction with the center as the boundary.)|
|Alternate|交互にスクロール方向が反転するよう設定します。<br>(Set the scroll direction to be reversed alternately.)|
|Twist|Crossの亜種で、もう少し細かくスクロール方向が反転するよう設定します。<br>(A variant of "Cross" that sets the scroll direction to be slightly more reversed.)|
|Asymmetry|Alternateの亜種で、基本的には交互にスクロール方向が反転するよう設定しますが、左右非対称になるよう設定します。<br>(A variant of "Alternate" that basically sets the scroll direction to be alternately reversed, but sets it to be asymmetrical.)|
|Flat|すべてのレーンが矢印の重なりに関係なく同じ方向に流れます。<br>一部のキーのみ使用できます。<br>(All lanes flow in the same direction regardless of arrow overlap. <br>Only some keys can be used.)|

### Shuffle (ミラー、ランダム)
譜面を左右反転したり、ランダムにします。  
ランダムにした場合は別譜面扱いとなり、**ハイスコアは保存されません。**  
(Flip the sequences left or right or make it random.
If you make it random, it will be treated as another sequences, and the high score will not be saved.)

|種類|内容|
|----|----|
|OFF|変化なし|
|Mirror|譜面をグループレーンごとに左右反転します。<br>(Flip the sequences horizontally for each group lane.)|
|Random|譜面をグループレーンごとにランダムに再配置します。<br>(Rearrange the sequences randomly for each group lane.)|
|Random+|譜面をグループに関係なくレーンごとにランダムに再配置します。<br>(Rearrange the sequences randomly for each lane regardless of the group.)|
|S-Random|譜面をグループごとに矢印個別にランダムに再配置します。<br>(Arrange the sequences randomly for each group by arrows.)|
|S-Random+|譜面をグループに関係なく矢印個別にランダムに再配置します。<br>(Arrange the sequences randomly regardless of the groups and arrows individually.)|

### AutoPlay (オートプレイ)
一部もしくは全てのキーをアシストするかどうかを設定します。  
完全オートプレイ時は**ハイスコアを保存しません。**  
(Set whether some or all keys are assisted or not.  
High score is not saved during full auto play.)

### Gauge (ライフゲージ設定)
クリア条件を設定します。  
Dancing☆Onigiri (CW Edition)の場合、  
クリア条件設定は譜面により大きくライフ制ゲージ・ノルマ制ゲージに分かれます。  
詳細は下記の通りです。  
(Set the clear condition. The details are as follows.)

■ ライフ制ゲージ（回復・ダメージ固定） / Life-Left Mode
- プレイ終了までにライフゲージが1でも残っていたらクリアです。  
ライフゲージが0になった場合、途中終了します。  
回復・ダメージ量は矢印数によらず固定です。  
(It is clear if there is **one** life gauge left by the end of play.
If the life gauge reaches 0, it will stop prematurely.
The amount of recovery and damage is fixed regardless of the number of sequences.)

|種類|概要|
|----|----|
|Original|回復・ダメージ量固定のデフォルトゲージです。<br>(Default)|
|Light|Originalと同じですが、Originalよりも回復量が大きくなっています。<br>(Same as "Original", but with greater recovery than "Original")|
|Heavy|Originalよりも回復量が小さく、ダメージが大きい設定です。<br>(The amount of recovery is smaller than "Original", and the damage is large.)|
|NoRecovery|ゲージが最初からMAXの状態で開始しますが、回復しません。<br>(The gauge starts from the beginning in the state of MAX but does not recover.)|
|SuddenDeath|1ミス(ウワァン/イクナイ)で終了するモードです。<br>(It is a mode to end with 1 mistake.)|

■ ノルマ制ゲージ（回復・ダメージ変動） / Norm Mode
- プレイ終了時、ライフゲージがノルマに達している必要があります。  
ノルマが0の場合は、ライフ制ゲージと同じです。  
回復・ダメージ量は矢印数に応じて変動します。（SuddenDeathを除く）  
矢印数が多くなると、回復・ダメージ量の幅は小さくなります。  
(At the end of play, the life gauge needs to reach the norm.
If the norm is 0, it is the same as a "Life-Left Mode".
The amount of recovery and damage changes according to the number of sequences. (Except SuddenDeath)
The greater the number of sequences, the smaller the amount of recovery and damage.)

|種類|概要|
|----|----|
|Normal|ノルマ制ゲージが指定された場合のデフォルトゲージです。<br>目標ノルマ到達でクリアです。<br>(It is clear by reaching the target quota at the end of the play.)|
|Easy|Normalと同じですが、Normalよりも回復量が大きくなっています。<br>(Same as Normal, but with greater recovery than Normal)|
|Hard|ゲージが最初からMAXの状態で開始しますが、回復量が微小でダメージ量が大きいモードです。<br>最後までゲージが残っていればクリアです。<br>(The gauge starts from the beginning in the state of MAX, but it is a mode with a small amount of recovery and a large amount of damage. It is clear if the gauge remains to the end.)|
|SuddenDeath|1ミス(ウワァン/イクナイ)で終了するモードです。<br>(It is a mode to end with 1 mistake.)|

### Adjustment (タイミング調整)
タイミングにズレを感じる場合、数値を変えることでズレを直すことができます。  
(If you feel a gap in timing, you can correct the gap by changing the value.)

### Fadein (フェードイン)
譜面を途中から再生します。  
途中から開始した場合は**ハイスコアを保存しません。**  
(Play the music from the middle.
High score is not saved if you start from the middle.)

### Volume (音量)
ゲーム内の音量を設定します。  
(Set the in-game volume.)

## Display Settings / 画面の見え方
![12game-setting2](./wiki/12game-setting2-1_v10.png)

### Display (オブジェクト等の表示／非表示)
プレイ画面上に存在するものの表示／非表示を切り替えます。  
(Switch between showing and hiding what exists on the play screen.)

|種類|内容|
|----|----|
|StepZone|ステップゾーンの表示<br>(Step zone)|
|Judgment|判定キャラクタ・コンボの表示<br>(Judgment character and combo)|
|FastSlow|Fast/Slow表示<br>(Displays the number of difference frames by determining whether the timing of pressing is early or late)|
|LifeGauge|ライフゲージの表示<br>(Life gauge)|
|Score|現時点の判定数を表示<br>(Display the current judgment count)|
|MusicInfo|音楽情報（現状は時間表示のみ）<br>(Music information (currently time display only))|
|FilterLine|Hidden+, Sudden+使用時のフィルターの境界線表示<br>(Filter border display when using "Hidden+" or "Sudden+")|
|Speed|途中変速、個別加速の有効化<br>(Enable mid-shift and individual acceleration)|
|Color|色変化の有効化<br>(Enable color change)|
|Lyrics|歌詞表示の有効化<br>(Enable lyrics display)|
|Background|背景・マスクモーションの有効化<br>(Enable background and mask motion)|
|ArrowEffect|矢印・フリーズアローモーションの有効化<br>(Enable arrow and freeze arrow motion)|
|Special|作品固有の特殊演出の有効化<br>(Enable special productions specific to the work)|

### Appearance (流れる矢印の見え方)
流れる矢印の見え方を制御します。  
(Controls the appearance of flowing sequences.)  
「Hidden+」と「Sudden+」についてはプレイ中に「pageUp」「pageDown」を押すことで可視範囲を調整できます。  
(For "Hidden+" and "Sudden+", you can adjust the viewable range by pressing "pageUp" or "pageDown" during play.)

|種類|内容|
|----|----|
|Visible|すべてが見える状態<br>(Everything is visible)|
|Hidden|初めの50%までは見えますが、その後は見えなくなります。<br>(Visible up to the first 50%, then disappears)|
|Sudden|初めの40%までは見えませんが、その後は見えるようになります。<br>(Not visible until first 40%, then visible)|
|Hidden+|基本的にHiddenと同じですが、Hiddenの可視範囲をプレイ中に調整できます。<br>(Same as "Hidden", but the visibility of "Hidden" can be adjusted during play)|
|Sudden+|基本的にSuddenと同じですが、Suddenの可視範囲をプレイ中に調整できます。<br>(Same as "Sudden", but the visibility of "Sudden" can be adjusted during play)|
|Hid&Sud+|Hidden+とSudden+を組み合わせて表示します。<br>(The combination of "Hidden+" and "Sudden+" is displayed.)|

### Opacity (判定キャラクタの透明度)
判定キャラクタ、コンボ数、Fast/Slow、Hidden+/Sudden+の境界線表示の透明度を設定します。  
(Set the transparency of the judgment character, the number of combos, Fast and Slow, and the border line display of "Hidden+" and "Sudden+".)

## Keyconfig / キーコンフィグ（矢印に対応するキーの割り当て）
- 画面が表示されている間に対応するキーを押すことで、割り当てるキーを変えることができます。  
変更されたキーは「黄色」で表示されます。  
- また、設定画面で「Data Save」を「ON」にしていれば、  
次回以降、設定したキーコンフィグをパターンとして丸ごと保存します。  
保存したキーは青色で表示されます。  
(By pressing the corresponding key while the screen is displayed,
You can change the key assigned.
The changed key is displayed in "yellow".
Also, if "Data Save" is set to "ON" on the setting screen,
From the next time, the set key configuration will be saved as a whole pattern.
Saved keys are displayed in "blue".)

![21game-keyconfig1](https://cw7.sakura.ne.jp/danoni/wiki/21game-keyconfig1-1_v10.png)

### ConfigType
キーコンフィグ対象の矢印群を切り替えます。  
Dan★Oniでは、1つの矢印に2つ以上のキーを割り当てることが可能な場合があり、  
この場合は左上の「ConfigType」を「Replaced」「ALL」にすることで変更が可能です。  
(Switches sequences for key configuration.
DanOni may be able to assign more than one key per sequence,
In this case, you can change it by setting "ConfigType" on the top left to "Replaced" or "ALL".)

### ColorType
矢印色の配色パターンを変更できます。  
(You can change the color scheme of the arrow color.)

### KeyConfigパターン変更 (<< >> ボタン)
キーコンフィグの配列パターンを変更します。  
「前回のキーコンフィグパターン」→「パターン1」(→「パターン2」→・・・)  
の順に切り替わります。  
(Change the array pattern of key configuration.
"Previous key configuration pattern" → "pattern 1" (→ "pattern 2" → ...)
It changes in order of.)

#### 別キーモード (TransKey Mode)
キーによっては、形状の似ている別のキーで遊ぶことができます。  
ただし、正規の譜面では無い遊び方のため、キーコンフィグやハイスコアは保存されません。  
(Depending on the key, you can play with another key that has a similar shape.  
However, the key config and high score will not be saved because it is not a regular music.)

### Reset (KeyConfigのリセット)
キーコンフィグのキー配列をデフォルトのキーパターンに戻します。  
(Restore key configuration key layout to default key pattern.)

## Main / プレイ画面
- Ready? が出た後にゲームが始まります。  
※ゲームによって、表示の仕方が異なる場合があります。  
(The game starts after "Ready?".)

![31game-main1](./wiki/31game-main1.png)

タイミング良くキーボードを押すと(・∀・)ｲｲ!!や(ﾟ∀ﾟ)ｷﾀｰ!!となり、ライフが上がります。  
一方、タイミングを外すと(´・ω・\`)ｼｮﾎﾞｰﾝ、(\`Д´)ｳﾜｧﾝ、(・A・)ｲｸﾅｲとなり、ライフが下がります。  
ゲーム終了までにライフゲージのライフが残っているか、ノルマ以上であればゲームクリアです。  
(When you press the keyboard with good timing (・∀・)ｲｲ!! (ﾟ∀ﾟ)ｷﾀｰ!! and life will go up. On the other hand, if you remove the timing (´・ω・\`)ｼｮﾎﾞｰﾝ, (`Д´)ｳﾜｧﾝ, (・A・)ｲｸﾅｲ will be, life falls. If the life of the life gauge remains by the end of the game or it is over the quota, the game is cleared.)  

![howtoplay2](./wiki/howtoplay2.png)

![32game-main2](./wiki/32game-main2.png)

## Result / 結果画面
- ゲームが終わると、結果画面へ移行します。  
最終的な判定やランクが画面に表示されます。  
「Tweet」ボタンを押すことでTwitterへ投稿も可能です。  
(When the game is over, the screen shifts to the result screen.
The final judgment or rank is displayed on the screen.
You can post to Twitter by pressing the "Tweet" button.)

![41game-resultView1](./wiki/41game-resultView1_v10.png)