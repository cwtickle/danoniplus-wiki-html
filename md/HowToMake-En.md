[<- Menu Title (English)](Sidebar-En.html)
# How to make chart overview

## Preparation
- DancingOnigiri(CW Edition) Source  
([Releases](https://github.com/cwtickle/danoniplus/releases) in Github, or download from `git clone`)
  - When downloading from "Releases", press "Source code (zip)" to download a complete set.
- DancingOnigiri Editor　* Download either
  - [Cross Walker](http://cw7.sakura.ne.jp/) (tickle's Editor)  
-> [Tools]   
　-> Dancing Onigiri Editor (Ver3.6.0 or later)
  - [Kibuntenkan ni RPG](http://www.kt-rpg.sakura.ne.jp/) (FUJI's Editor)  
-> [Tools]   
　-> editor200.lzh (5, 7, 7i, 9, 11keys) or nkeyeditor.lzh (Others keys)  
    - If you want to use "FUJI's Editor", please download and replace the template file [here](https://cw7.sakura.ne.jp/gift/editorFuji_templateHTML5.zip).  
- Text editor (You can use an easy-to-use one. The following is recommended.)  
  - [Sakura Editor](https://sakura-editor.github.io/) : for HTML, CSS  
  - [Visual Studio Code](https://code.visualstudio.com/) : from HTML, CSS, JavaScript  

## Overview of creating charts

1. Save the source set to any folder.  
2. Use [danoni/danoni0.html] as a reference to create an HTML base.  
At a minimum, the following description is required. (Copy and paste available)    
Place the save destination in the [danoni] folder or any folder in the same hierarchy.  
Detailed settings are possible in the charts header.  
See [Charts Header Specification](dos_header-En.html) for details.  
```html
<!DOCTYPE html>
<html>
  <head>
    <!--// Character code specification (specify html character code such as Shift_jis, UTF-8) //-->
    <meta http-equiv="Content-Type" content="text/html;charset=shift_jis">

    <!--// Usage definition of Javascript and CSS //-->
    <meta http-equiv="Content-Script-Type" content="text/javascript">
    <meta http-equiv="Content-Style-Type" content="text/css">

    <!--// Javascript and CSS files used by DanOni. 
           You can also specify another CSS file for this page. The following are required. //-->
    <script src="../js/danoni_main.js" charset="UTF-8"></script>
    <link rel="stylesheet" type="text/css" href="../css/danoni_main.css">

  </head>
  <body>
    <!--//
      The chart data itself. At a minimum, the following description is required.  
      The bracketed part and http://~ must be changed to the actual address.  
        musicTitle: Music information
        difData: Chart information (Specify in order of number of keys, chart name, initial speed.
                 You can specify multiple charts with $ separator.)
        musicUrl: Specify the music file name to be stored in the [music] folder.
        tuning: Maker information
    //-->
    <input type="hidden" name="dos" id="dos" value='

|musicTitle=(Music name),(Artist name),http://www.google.co.jp/|
|difData=5,Normal,3.5$5,Hard,3.5|
|setColor=#99ffff,#ffff33,#ffffff,#ff0066,#ff9966|
|frzColor=#66ffff,#6666ff,#ffff66,#ffff66|
|startFrame=0|
|musicUrl=nosound.mp3|

|left_data=200|down_data=|up_data=|right_data=|space_data=300|

|tuning=(Maker name),http://www.google.co.jp/|

    '>
    <!--// Dancing☆Onigiri(CW Edition) itself. 
           The width value can be changed. 500px or more recommended. //-->
    <div id="canvas-frame" style="width:500px;margin:auto;">
      <canvas id="layer0" width="500" height="500"></canvas>
      <canvas id="layer1" width="500" height="500"></canvas>
    </div>
  </body>
</html>
```

3. Place the music file in the [music] folder.  
Replace the description of |musicUrl=nosound.mp3| in the HTML file described in 2.   
with the name of the saved music file.  

4. Open the created HTML file and check that the screen is displayed.  
Also, go to [Click Here!]-> [Play] and check that the specified music file is loaded.  

5. Open the "Dancing Onigiri Editor".
   - Please refer to the help in the editor for how to make. [Example (Japanese)](http://cw7.sakura.ne.jp/gift/editor/editorhelp.html)  
   - If you have made a Flash version, the procedure is exactly the same.  
   - "dos.txt" in the procedure corresponds to the above-mentioned chart data itself.  
The SWF file is only for the Flash version.  

6. Replace the created chart data with the following part in the html file created in 2.  
```
|left_data=300|down_data=|up_data=|right_data=|space_data=200|
```

7. Save the HTML file and check if the music and charts play.  
Please adjust the timing appropriately using the editor.  

## How to make chart data in an external file (ver2.5.0 or later)
Variables are the same except for the described method.  
A combination with the above method is also possible.

```html
<!DOCTYPE html>
<html>
  <head>
    <!--// Character code specification (specify html character code such as Shift_jis, UTF-8) //-->
    <meta http-equiv="Content-Type" content="text/html;charset=shift_jis">

    <!--// Usage definition of Javascript and CSS //-->
    <meta http-equiv="Content-Script-Type" content="text/javascript">
    <meta http-equiv="Content-Style-Type" content="text/css">

    <!--// Javascript and CSS files used by DanOni. 
           You can also specify another CSS file for this page. The following are required. //-->
    <script src="../js/danoni_main.js" charset="UTF-8"></script>
    <link rel="stylesheet" type="text/css" href="../css/danoni_main.css">

  </head>
  <body>
    <!--// Description when the chart data is written in a separate file //-->
    <input type="hidden" name="externalDos" id="externalDos" value="dos1.txt">
    <!--// Set the character code of the score file. 
           Unnecessary if both page and music file have the same character code. //-->
    <input type="hidden" name="externalDosCharset" id="externalDosCharset" value="Shift_JIS">
    <!--// Dancing☆Onigiri(CW Edition) itself. The width value can be changed. 500px or more recommended. //-->
    <div id="canvas-frame" style="width:500px;margin:auto;">
      <canvas id="layer0" width="500" height="500"></canvas>
      <canvas id="layer1" width="500" height="500"></canvas>
    </div>
  </body>
</html>
```

Contents of external file (dos1.txt in this case)  
(Characters in two lines above and below are required)
```javascript
function externalDosInit() {   /* required */
  g_externalDos = `            /* required */

|musicTitle=(Music name),(Artist name),http://www.google.co.jp/|
|difData=5,Normal,3.5$5,Hard,3.5|
|setColor=#99ffff,#ffff33,#ffffff,#ff0066,#ff9966|
|frzColor=#66ffff,#6666ff,#ffff66,#ffff66|
|startFrame=0|
|musicUrl=nosound.mp3|

|left_data=200|down_data=|up_data=|right_data=|space_data=300|

|tuning=(Maker name),http://www.google.co.jp/|

  `;                           /* required */
}                              /* required */
```

### How to create an external chart file using FUJI's editor
- By setting as follows, chart data can be output directly to a text file.

#### Header
```javascript
function externalDosInit() {
  g_externalDos = `

|musicTitle=(Music name),(Artist name),http://www.google.co.jp/|
|difData=5,Normal,3.5$5,Hard,3.5|
|setColor=#99ffff,#ffff33,#ffffff,#ff0066,#ff9966|
|frzColor=#66ffff,#6666ff,#ffff66,#ffff66|
|startFrame=0|
|musicUrl=nosound.mp3|
```
#### Footer
- Since `&tuning=NAME` follows, put`//`at the end to prevent js errors.
```javascript
|
`;
}//
```