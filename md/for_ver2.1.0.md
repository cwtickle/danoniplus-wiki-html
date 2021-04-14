# ver2.1.0への移行について
ver2.1.0より、danoni_custom.js側にあった記述がdanoni_main.js側に移りました。  
これまでのdanoni_custom.jsもそのままの利用が可能で、  
独自の表示を行いたい場合は変更不要ですが、  
タイトル表示のデフォルトに対してカスタムを行っている場合、  
記述を変更（基本的には表示の削除）を行うことで、新しい設定変更にも対応できます。  

## 変更箇所
### customTitleInit
＜Before＞
```javascript
	// レイヤー情報取得
	var layer0 = document.getElementById(`layer0`);
	var l0ctx = layer0.getContext(`2d`);

	// 画面背景を指定 (background-color)
	var grd = l0ctx.createLinearGradient(0, 0, 0, g_sHeight);
	grd.addColorStop(0, `#000000`);
	grd.addColorStop(1, `#222222`);
	l0ctx.fillStyle = grd;
	l0ctx.fillRect(0, 0, g_sWidth, g_sHeight);


	// 背景の矢印オブジェクトを表示
	var lblArrow = createArrowEffect(`lblArrow`, g_headerObj[`setColor`][0], (g_sWidth - 500) / 2, -15, 500, 180);
	lblArrow.style.opacity = 0.25;
	lblArrow.style.zIndex = 0;
	divRoot.appendChild(lblArrow);

	// 曲名文字描画（曲名は譜面データから取得）
	// TEST:試験的に矢印色の1番目と3番目を使ってタイトルをグラデーション
	var grd = l0ctx.createLinearGradient(0, 0, g_sHeight, 0);
	if (g_headerObj[`setColor`][0] != undefined) {
		grd.addColorStop(0, g_headerObj[`setColor`][0]);
	} else {
		grd.addColorStop(0, `#ffffff`);
	}
	if (g_headerObj[`setColor`][2] != undefined) {
		grd.addColorStop(1, g_headerObj[`setColor`][2]);
	} else {
		grd.addColorStop(1, `#66ffff`);
	}
	var titlefontsize = 64 * (12 / g_headerObj[`musicTitle`].length);
	if (titlefontsize >= 64) {
		titlefontsize = 64;
	}

	// カスタム変数 titlesize の定義
	if (g_rootObj.titlesize != undefined && g_rootObj.titlesize != ``) {
		titlefontsize = setVal(g_rootObj.titlesize, titlefontsize, `number`);
	}

	createLabel(l0ctx, g_headerObj[`musicTitle`], g_sWidth / 2, g_sHeight / 2,
		titlefontsize, `メイリオ`, grd, `center`);
```
＜After＞　※ver3.6.0以降は下記記載も不要です。
```javascript
	// 以下は全体設定です。作品別に設定する場合は不要です。

	// タイトル曲名表示のカスタム利用有無 (false:デフォルトを利用 / true:カスタムを利用(これまで通り))
	g_headerObj.customTitleUse = `false`;
	// タイトル背景矢印表示のカスタム利用有無 (false:デフォルトを利用 / true:カスタムを利用(これまで通り))
	g_headerObj.customTitleArrowUse = `false`;
	// タイトル背景表示のカスタム利用有無 (false:デフォルトを利用 / true:カスタムを利用(これまで通り))
	g_headerObj.customBackUse = `false`;
	// タイトル背景表示（メイン画面のみ適用）のカスタム利用有無 (false:デフォルトを利用 / true:カスタムを利用(これまで通り))
	g_headerObj.customBackMainUse = `false`;
	// Ready表示のカスタム利用有無 (false:デフォルトを利用 / true:カスタムを利用(これまで通り))
	g_headerObj.customReadyUse = `false`;
```

### customOptionInit
＜Before＞
```javascript
	// レイヤー情報取得
	var layer0 = document.getElementById(`layer0`);
	var l0ctx = layer0.getContext(`2d`);

	// 画面背景を指定 (background-color)
	var grd = l0ctx.createLinearGradient(0, 0, 0, g_sHeight);
	grd.addColorStop(0, `#000000`);
	grd.addColorStop(1, `#222222`);
	l0ctx.fillStyle = grd;
	l0ctx.fillRect(0, 0, g_sWidth, g_sHeight);
```

＜After＞
```javascript
	// 記述不要
```

### customSettingsDisplayInit
＜Before＞
```javascript
	// レイヤー情報取得
	var layer0 = document.getElementById(`layer0`);
	var l0ctx = layer0.getContext(`2d`);

	// 画面背景を指定 (background-color)
	var grd = l0ctx.createLinearGradient(0, 0, 0, g_sHeight);
	grd.addColorStop(0, `#000000`);
	grd.addColorStop(1, `#222222`);
	l0ctx.fillStyle = grd;
	l0ctx.fillRect(0, 0, g_sWidth, g_sHeight);
```

＜After＞
```javascript
	// 記述不要
```

### customMainInit
＜Before＞
```javascript
	// レイヤー情報取得
	var layer0 = document.getElementById(`layer0`);
	var l0ctx = layer0.getContext(`2d`);

	// 画面背景を指定 (background-color)
	var grd = l0ctx.createLinearGradient(0, 0, 0, g_sHeight);
	grd.addColorStop(0, `#000000`);
	grd.addColorStop(1, `#222222`);
	l0ctx.fillStyle = grd;
	l0ctx.fillRect(0, 0, g_sWidth, g_sHeight);

	// Ready?表示
	var lblReady = createDivLabel(`lblReady`, g_sWidth / 2 - 100, g_sHeight / 2 - 100,
		200, 50, 40, C_CLR_TITLE,
		`<span style='color:#9999ff;font-size:60px;'>R</span>EADY?`);
	divRoot.appendChild(lblReady);
	lblReady.style.animationDuration = `2.5s`;
	lblReady.style.animationName = `leftToRightFade`;
	lblReady.style.opacity = 0;
```

＜After＞
```javascript
	// 記述不要
```

### customResultInit
＜Before＞
```javascript
	// レイヤー情報取得
	var layer0 = document.getElementById(`layer0`);
	var l0ctx = layer0.getContext(`2d`);

	// 画面背景を指定 (background-color)
	var grd = l0ctx.createLinearGradient(0, 0, 0, g_sHeight);
	grd.addColorStop(0, `#000000`);
	grd.addColorStop(1, `#222222`);
	l0ctx.fillStyle = grd;
	l0ctx.fillRect(0, 0, g_sWidth, g_sHeight);
```

＜After＞
```javascript
	// 記述不要
```