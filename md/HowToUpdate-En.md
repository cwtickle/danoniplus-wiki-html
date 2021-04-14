[<- Menu Title (English)](Sidebar-En.html)
# How to upgrade

## Check in advance
1. First, check the version of the device.
You can check the version on the title screen where "Dancing Onigiri" is launched.
(In this case, it is Ver3.9.0)
<img src="http://cw7.sakura.ne.jp/danoni/wiki/danoniVersion.png" width="400">

## Version upgrade method (when not using Git)
2. Go [Releases](https://github.com/cwtickle/danoniplus/releases). 

<img src="http://cw7.sakura.ne.jp/danoni/wiki/danoniReleaseA.png" width="600">

Check the red frame between the current version and the latest version (the part in the separate file is the update part).
Normally, there is no problem if you download only “danoni_main.js”.
As mentioned above, if other files are also targeted, download them together.  

3. Copy the contents of the [css] [js] folder directly under the [danoniplus] folder (the folder directly under the download) to the desktop.

4. Copy the file downloaded in step 2 to the [css] [js] folder.
* If the extension is ".css", put it in the [css] folder. If it is ".js", put it in the [js] folder.  

5. Start up "Dancing Onigiri" and upgrade is complete if the version number is new.
Play through the game and use it as is if there are no problems.

## Remarks
"danoni_custom.js", "danoni_custom2.js", and "danoni_setting.js" are user-customizable format files.
Usually, no replacement is required unless otherwise noted.
If you are customizing, note that the individually set source will be overwritten.

When this file is updated recently, the name is uploaded on Release as "danoni_custom-template.js".  

## How to check the difference between the current version and the latest version
- It can be confirmed from Release on GitHub.
For those who want to check source differences, there is usually no need to be aware of it.
If you check your current version and look at the corresponding Release, there is a link called “XX Commits”.
Click this to check the difference from the latest version.

- In addition, there are links to Pull Request and Issue in the part linked from the changes,
The reason for change and background are recorded.  
<img src="http://cw7.sakura.ne.jp/danoni/wiki/danoniReleaseB.png" width="600">

### Symbols displayed on Release
- In "Dancing Onigiri (CW Edition)", it is described so that the change contents can be understood by dividing as follows. 
- For changes, the relevant Pull Request or Issue numbers are linked.  

|Display|Description|
|----|----|
|:star: **New Features**|Describes new features.|
|:hammer_and_wrench: **Improvements**|Although it is not a new function, it is described when the code structure is reviewed.|
|:beetle: **Bug Fixes**|Described when the bug of the previous version is corrected.|
|:notebook_with_decorative_cover: **Documentation**|Describe the link destination of Wiki etc. related to this function change.|
|:heart: **Contributors**|Introducing new features, providing bug information, pull requests, etc. <br> Those who cooperated in this release are listed.|
|:four_leaf_clover: **Remarks**|If there are any details or notes regarding this change, please describe them.|

### When it does not work well even after upgrading
- Click "v6.4.0-> v6.5.0" or "XX Commits" in "How to check the difference between the current version and the latest version" above, and the following screen appears.  
<img src="http://cw7.sakura.ne.jp/danoni/wiki/danoniRelease4_2.png" width="600">

- When you scroll down, there is a link called "XX changed files", so clicking on it will display a list of files that have changed up to the latest version.
From this list, if there is a file whose extension has been changed to ".js" or ".css", and there is something that has not been downloaded, download the "Source code (zip)" set from the latest "Release" Overwrite the displayed file.
(However, please confirm whether "danoni_custom.js" needs to be overwritten after checking the contents.)  
<img src="http://cw7.sakura.ne.jp/danoni/wiki/danoniRelease5.png" width="600">