[<- Menu Title (English)](Sidebar-En.html)
# Source hierarchy
This is an overview of the files used in the "Dancing Onigiri (CW Edition)" source.
Please see another page for a description of the contents.  

|1st layer|2nd layer|Description|
|----|----|----|
|css|danoni_main.css|Use for arrow color change, Result motion, etc. <br> Since it sometimes changes at the time of version upgrade, it is recommended to separate it from CSS for each page.|
|danoni|---|Contains a sample HTML file for Dancing Onigiri.|
|img|---|Image file. A set of arrows and ASCII art.|
|img|cursor.png|Cursor image used in the key configuration screen|
|img|frzbar.png|Freeze arrow bar, life gauge body|
|img|borderline.png|An image that displays the border position when using a quota gauge.|
|img|arrow_500.png|Sequences body|
|img|arrowShadow_500.png|For drawing the backside of the arrow. Use with freeze arrow.|
|img|c_600.png|ASCII art(C)|
|img|giko_600.png|ASCII art(Giko)|
|img|iyo_600.png|ASCII art(Iyo)|
|img|monar_600.png|ASCII art(Monar)|
|img|morara_600.png|ASCII art(Morara)|
|img|onigiri_600.png|ASCII art(Onigiri, Riceball)|
|img|aaShadow_500.png|For drawing back side of ASCII art. Use with freeze arrow.|
|js|---|Many of the sources for Dancing Onigiri (CW Edition) are listed here. <br> "danoni_main.js" is required. Other custom files can be divided into settings and renamed by work. Setting is possible [Chart Header Specification#customjs](dos-h0019-customjs.html).|
|js|danoni_main.js|Main source. Used in combination with "danoni_main.css". <br> As a library, this file is usually replaced with each version upgrade. <br> If you want to remodel, we recommend using the following custom file.|
|js|danoni_setting.js|User common settings. <br> Added from ver3.0.0. Used for items that are set in common to all works.|
|js|danoni_custom.js|User custom source 1 (common custom). <br> Call from "danoni_main.js" and use it.<br>It is possible to change the name, but in that case, setting is required in [Chart header specification #customjs](dos-h0019-customjs.html).|
|js|danoni_custom2.js|User custom source 2 (custom by work). <br> Call from "danoni_main.js" and use it. Use is optional.<br>When using, it can not be used unless it is set in [Chart header specification #customjs](dos-h0019-customjs.html).|
|music|---|Storage location for music files. [Chart header specification #musicFolder](dos-h0013-musicFolder.html) can be changed for each work.|
|music|nosound.mp3|Silence file that is included from the beginning.|

