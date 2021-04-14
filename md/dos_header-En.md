[<- Menu Title (English)](Sidebar-En.html)
# Chart Header Specification 
- Please see [Migration overview for ParaFla! Users](forParaFlaUser-En.html) for notes.  
- Required items are marked with (*) and shared items with ParaFla source are marked with (★).  

## 🎶 Music &amp; chart information
- [musicTitle](dos-h0001-musicTitle.html) (*, ★)  Music and Artist Information
- [difData](dos-h0002-difData.html) (*, ★)  Chart Information 
- [musicUrl](dos-h0011-musicUrl.html) (*)  Music file name
- [musicNo](dos-h0012-musicNo.html)  Associating music files with charts
- [musicFolder](dos-h0013-musicFolder.html)  Music file directory location
- [dummyId](dos-h0042-dummyId.html)  Dummy chart specification

## ⏳ Play time control &amp; music position adjustment
- [startFrame](dos-h0005-startFrame.html) (★)  start frame number
- [blankFrame](dos-h0006-blankFrame.html)  The number of blank frames before the music starts
- [endFrame](dos-h0007-endFrame.html)  End frame number
- [fadeFrame](dos-h0008-fadeFrame.html)  Fade out start frame number
- [adjustment](dos-h0009-adjustment.html)  Initial adjustment of chart position
- [playbackRate](dos-h0010-playbackRate.html)  Music playback speed (mainly for test play)

## 🛠 Initial settings
- [minSpeed](dos-h0015-minSpeed.html)  Minimum speed of sequences that can be set
- [maxSpeed](dos-h0016-maxSpeed.html)  Maximum speed of sequences that can be set
- [settingUse](dos-h0035-settingUse.html)  Use of setting items
- [transKeyUse](dos-h0024-transKeyUse.html)  Use of different key mode
- [customFont](dos-h0020-customFont.html)  General screen font
- [colorDataType](dos-h0046-colorDataType.html)  Past compatible settings for color change of sequences
- [colorCdPaddingUse](dos-h0047-colorCdPaddingUse.html)  Zero padding setting for initial sequences color

## ⏯ Initial settings during play
- [stepY](dos-h0014-stepY.html)  Y coordinate position of step zone
- [stepYR](dos-h0049-stepYR.html)  Difference from the current Y coordinate position of the step zone (bottom)
- [setColor](dos-h0003-setColor.html) (*, ★)  Arrow (sequences) color
- [frzColor](dos-h0004-frzColor.html) (*, ★)  Freeze arrow (sequences) color
- [setShadowColor](dos-h0041-setShadowColor.html)  Settings for filling the inside of the arrow of sequences and it's color
- [maxLifeVal](dos-h0045-maxLifeVal.html)  The number of life limit
- [gaugeX](dos-h0022-gaugeX.html)  Gauge setting details
- [frzStartjdgUse](dos-h0037-frzStartjdgUse.html)  Whether to make judgements at the start of the freeze arrow
- [frzAttempt](dos-h0038-frzAttempt.html)  Number of frames allowed at freeze arrow hit
- [finishView](dos-h0023-finishView.html)  Full combo production
- [keyRetry](dos-h0039-keyRetry.html)  Key code of shortcut key to retry
- [keyTitleBack](dos-h0040-keyTitleBack.html)  Key code of shortcut key for title back

## ⚓️ Initial settings of title &amp; result screen
- [masktitleButton](dos-h0043-masktitleButton.html)  Enable or disable setting of buttons on title screen
- [maskresultButton](dos-h0044-maskresultButton.html)  Valid or invalid setting of buttons on the result screen
- [resultMotionSet](dos-h0048-resultMotionSet.html)  Result effect ON / OFF setting

## 🏙 Import custom data
- [customjs](dos-h0019-customjs.html)  Specify customjs file
- [preloadImages](dos-h0021-preloadImages.html)  Preload settings for image files

## 🍂 Use of default design
- [customTitleUse](dos-h0025-customTitleUse.html)  Music title character of title
- [customTitleArrowUse](dos-h0026-customTitleArrowUse.html)  Title background arrow
- [customBackUse](dos-h0027-customBackUse.html)  Background (except play screen)
- [customBackMainUse](dos-h0028-customBackMainUse.html)  Background (play screen)
- [customReadyUse](dos-h0029-customReadyUse.html)  Production at the start of play

## 🌟 Title text effect (default design) 
- [titlesize](dos-h0030-titlesize.html)  Font size
- [titlefont](dos-h0031-titlefont.html)  Font name
- [titlegrd](dos-h0032-titlegrd.html)  Text gradation
- [titlepos](dos-h0033-titlepos.html)  X, Y coordinate position
- [titlelineheight](dos-h0034-titlelineheight.html)  Line spacing for multiple lines

## 📋 Credit related
- [tuning](dos-h0017-tuning.html) (★)  Producer credit
- [hashTag](dos-h0018-hashTag.html)  Hashtag
- [releaseDate](dos-h0036-releaseDate.html)  Work release date
