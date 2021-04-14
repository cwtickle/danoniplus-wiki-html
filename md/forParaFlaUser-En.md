[<- Menu Title (English)](Sidebar-En.html)
# Migration overview for ParaFla! Users

## Download source  
Download the source from "Clone or Download".  
(If you know Git or want to do source control in the future, you may want to Clone.)  
![Download Source](http://cw7.sakura.ne.jp/danoni/wiki/parafla1.png)

## Source configuration
"Js", "css", and "img" are in this configuration and do not change the hierarchy.  
![](http://cw7.sakura.ne.jp/danoni/wiki/parafla2.png)

|Folder name|Description|
|----|----|
|js|Main Source. required.|
|css|Performs DanOni color change and Canvas size management. Required.|
|img|Contains images of DanOni's arrows and rice balls. Required.|
|music|Music folder. Put mp3 data here. Folder creation is required.|
|danoni|Works folder. The name of "Danoni" can be changed freely according to the title of the work. <br> You can cut as many folders as you like in the same hierarchy <br> (same as the current SWF format). <br> It is also possible to group them in the same folder.|

## Things to prepare (for charts conversion) 
- Chart file (dos.txt)
- Music file (mp3, wav, ogg file)
- HTML file (Recommend diversion of sample in "Danoni" folder)

## How to Convert  
### Charts Conversion

For the charts file, replace "&" with "|".  
- Before  
`
&left_data=230,250,270,...&down_data=250,290,310,...&
`
- After  
`
|left_data=230,250,270,...|down_data=250,290,310,...|
`

The following information is added to the charts file.  
Replace "music.mp3" with the mp3 file name.   
Single-byte alphanumeric characters are recommended for the file name.  
`
|musicUrl=music.mp3|blankFrame=200|
`  

"blankFrame" is equivalent to the "do nothing" frame before the start in ParaFla! source.  
Usually 200 frames.    


In this state, select all the contents of the charts file  
and put it between the following in the source of the sample page.  
`
<input type="hidden" name="dos" id="dos" value='(Put the charts file here.)'>  
`

It should actually look like this: Line feed is OK.  
What is enclosed in this is the core of DanOni.    
```html  
<input type="hidden" name="dos" id="dos" value='
   |musicTitle=Petit Magie,Napi,http://mart.kitunebi.com/|
   |difData=11W,Normal,3.5,x,10,5$11W,Hard,3.5,70,2,7|
   |setColor=0x9999ff,0xccffff,0xffffff,0xffff99,0xff9966|
   |frzColor=0x00ffff,0x6600ff,0xffff66,0xffff66|
   |startFrame=0|blankFrame=195|
   |musicUrl=PetitMagie.mp3|
   |left_data=264,857,1704,1873,1916,2043|leftdia_data=603,920,1492,1619,4351|down_data=899,1471,1556,1958,2170|
   |color_data=200,34,0xcc99ff,200,35,0x9966ff|
   |tuning=tickle,http://cw7.sakura.ne.jp/|
'>
<div id="canvas-frame" style="width:600px;margin:auto;">
   <canvas id="layer0" width="600" height="500"></canvas>
   <canvas id="layer1" width="600" height="500"></canvas>
</div>
```

If you do not use the sample html file,
Put the following two lines in the &lt;head&gt; tag.  
```html  
<script src="../js/danoni_main.js" charset="UTF-8"></script>
<link rel="stylesheet" type="text/css" href="../css/danoni_main.css">
```  

### Storing music files  

Put the music file (mp3) specified above into the "music" folder.  
If you open an HTML file in this state, it will work.  

### Warning  
- About single-byte single quotes in the charts files  
Since the data is enclosed in single-byte single quotes, it cannot be used.  
Either escape (&amp;#39;) or use full-width single quotes (’).  

- About the "music" folder  
If you can use .htaccess, it is recommended to put it in.  
Specify as follows.
<pre>
SetEnvIf Request_URI "\.(mp3|wav|ogg)$" deny_ref
SetEnvIf Referer <b>"cw7\.sakura\.ne\.jp"</b> !deny_ref
Order Allow,Deny
Allow from all
Deny from env=deny_ref
</pre>
Replace the bold text with the server. Replace "\." With "\\\."  


### Charts header supplement  
Lists the configurable score headers that do not appear in SWF created with ParaFla! Source.  
For others, please refer to [Charts Header Specification](dos_header-En.html).  

|Variable name|Description|Usage examples|
|----|----|----|
|adjustment|Specify how many frames to advance(slow) the current score.|adjustment=40|
|endFrame|The number of frames at the end of the music. <br> It is usually unnecessary because it is obtained from music data, but it is used when there is a surplus.|endFrame=6000|
|fadeFrame|Number of frames to fade out.<br>Can be specified for each chart, separated by "$".|fadeFrame=3600$7200|
|titlesize|Changed the text size of the title on the title screen. <br>Used when out of the frame.|titlesize=40|
