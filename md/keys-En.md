[<- Menu Title (English)](Sidebar-En.html)
# Keys Specification
![keys](http://cw7.sakura.ne.jp/danoni/wiki/keys1.png)

Each key of "Dancing Onigiri" consists of a combination of keys and patterns.  
The following indicates that it is the 1st(0th) pattern of "11key".  
<pre>
pos<b>11</b>_<b>0</b>
</pre>

The settings for patterns belonging to the same key are similar, but they are treated as completely different keys.   Settings can also be changed individually.  
The order in which the sequences are listed must be from left to right and top to bottom.  

|Element|Description|Details|
|----|----|----|
|charaX_Y|Read variable prefix|Represents a character string before "_data" such as "left_data", "down_data".|
|colorX_Y|Arrow color assignment|Allocate the color code described in "setColor" in the chart data. <br>Normally, 0 to 4 can be used, and the color corresponding to the number when "setColor" is arranged is assigned as the initial color.|
|stepRtnX_Y|Angle / ASCII Art type|This indicates how many times the rotated arrow is arranged based on the left-pointing arrow. <br> Alternatively, specify the target ASCII art (AA). <br>6 types of ASCII Art can be specified: "onigiri", "giko", "iyo", "c", "morara", "monar".|
|posX_Y|Step zone position|A number indicating where to place step zones when they are spaced equally. See the image above. <br> If you don't want to be evenly spaced, you can skip the step zone by skipping numbers as in the example above.|
|divX_Y|Upper or lower folding position|Specify the position to fold the upper and lower steps of the step zone. <br> The value specified is posX_Y. Specify the lower number for the first time. <br> If there is no upper or lower binding, specify the last digit +1.|
|blankX_Y|Step zone interval (X coordinate)|Specify the step zone interval. If not specified, it will normally be 55px.|
|keyCtrlX_Y|Key config|Specify the key code corresponding to each step. Expressed as a multidimensional array. Multiple keys can be assigned to the same step.|
|shuffleX_Y|Shuffle group|When using Mirror, Random, S-Random, swap with the same group. The same number is in the same group.|
|transKeyX_Y|Set different key mode|Specifies the name of the key if the specified key pattern is for another key. <u>Do not specify for the same key. </u><br>If specified, the key specified here will be displayed as supplementary information on the result screen. <br> Also, while playing in another key mode, high score, key config, etc. are not saved.|
|keyRetryX_Y|Retry key|Specify the key code of the key that can be retried with the shortcut during play. <br>The default is 8 (BackSpace).|
|keyTitleBackX_Y|Title back key|Specify the key code of the key that can be used for title back with the shortcut during play. <br> The default is 46 (Delete).|

## A little concrete example (in case of 11key) 

Since it may not come with a pin even if it is written in letters, let's look specifically at the example of 11key pattern 0 (first).
The setting value looks like this. The order is left to right and top to bottom.  
  
|Element|Example|
|----|----|
|chara11_0|["sleft", "sdown", "sup", "sright", "left", "leftdia", "down", "space", "up", "rightdia", "right"]|

In this case, you can import in the following chart format. (Numbers omitted) 
<pre>
|sleft_data=...|sdown_data=...|...|right_data=...|
</pre>

|Element|Example|
|----|----|
|color11_0|[3, 3, 3, 3, 0, 1, 0, 2, 0, 1, 0]|
|setColor|0xcc99ff, 0xffccff, 0xffffff, 0xffff99, 0xff9966|

In the top image, the upper row is 3 (#ffff99, yellow), the lower odd number is 0 (#cc99ff, purple), the even number is 1 (#ffccff, pink), Onigiri is 2 (#ffffff, white).  


|Element|Example|
|----|----|
|stepRtn11_0|[0, -90, 90, 180, 0, -45, -90, "onigiri", 90, 135, 180]|

In the top image, with respect to the left arrow, -90° is a down arrow, 90° is an up arrow, and 180° is a right arrow.
The part of "onigiri" is a rice ball. 

|Element|Example|
|----|----|
|pos11_0|[2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]|
|div11_0|6|

I put numbers in yellow letters in the top image.
It wraps to the bottom from where the number is written as 6.
Since 0 and 1 are not specified, the arrow is not displayed.

|Element|Example|
|----|----|
|keyCtrl11_0|[ [37], [40], [38, 0], [39], [83], [68], [70], [32], [74], [75], [76] ]|

The key code is written.
This isn't a pinch, but you can see that there are only two-third elements.
This part indicates that there is a substitute key.


## For custom keys  

If you want to publish your own key, you need to describe it in the chart data.
The basic idea is exactly the same as above, but the description method is slightly different.

### keyExtraList
A list of keys to add. You can add any number separated by commas.  
<pre>
|keyExtraList=6|
</pre>

### colorX, charaX, divX, stepRtnX, keyCtrlX, blankX, shuffleX
They correspond to colorX_Y, charaX_Y, divX_Y, stepRtnX_Y, keyCtrlX_Y, blankX_Y, shuffleX_Y, respectively. Separate multiple specifications with "$".  
For keyCtrl, separate alternate key specifications with a slash (/).    

|Element|Example|
|----|----|
|colorX|color6=0,1,0,1,0,2$0,1,0,1,0,2|
|charaX|chara6=arrowA,arrowB,arrowC,arrowD,arrowE,arrowF$arrowA,arrowB,arrowC,arrowD,arrowE,arrowF|
|divX|div6=6$3|
|stepRtnX|stepRtn6=0,45,-90,135,180,onigiri$0,45,-90,135,180,onigiri|
|keyCtrlX|keyCtrl6=75,79,76,80,187,32/0$75,79,76,80,187,32/0|
|blankX|blank6=60$60|
|shuffleX|shuffle6=0,0,0,0,0,1$0,0,0,0,0,1|
|transKeyX|transKey6=$6i|
|keyRetryX|keyRetry6=9|
|keyTitleBackX|keyTitleBack6=46|