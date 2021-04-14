⭐ New Features / 🛠️ Improvements / 🐞 Bug Fixes

 | **v21** | [**v20 ->**](Changelog-v20.html)

## v21.4.2 ([2021-04-07](https://github.com/cwtickle/danoniplus/releases/tag/v21.4.2))
- ⭐ Changed the corresponding key locations in the key configuration from labels to buttons. ( PR [#1040](https://github.com/cwtickle/danoniplus/pull/1040), [#1048](https://github.com/cwtickle/danoniplus/pull/1048) )
- 🛠️ Organize the source code for the number of keys and common processing systems. ( PR [#1041](https://github.com/cwtickle/danoniplus/pull/1041), [#1042](https://github.com/cwtickle/danoniplus/pull/1042), [#1043](https://github.com/cwtickle/danoniplus/pull/1043), [#1045](https://github.com/cwtickle/danoniplus/pull/1045), [#1046](https://github.com/cwtickle/danoniplus/pull/1046), [#1050](https://github.com/cwtickle/danoniplus/pull/1050) )
- 🛠️ Improved vertical layout collapse in the warning window. ( Issue [#823](https://github.com/cwtickle/danoniplus/pull/823), PR [#1046](https://github.com/cwtickle/danoniplus/pull/1046) )
- 🐞 Fixed an issue where the full combo display would appear earlier when S-Random was applied to a score containing empty arrow data.
 ( PR [#1044](https://github.com/cwtickle/danoniplus/pull/1044), Gitter [2021-04-06](https://gitter.im/danonicw/community?at=606c808592a3431fd67b1640) ) <- :boom: [**v3.1.0**](Changelog-v3.html#v310-2019-02-26)

## v21.3.0 ([2021-04-03](https://github.com/cwtickle/danoniplus/releases/tag/v21.3.0))
- 🛠️ Fixed an issue that could cause the same warning message to be displayed twice. ( PR [#1037](https://github.com/cwtickle/danoniplus/pull/1037)  )
- 🛠️ Changed the value of each property of "g_loadObj" to "true" when loading is completed. ( PR [#1036](https://github.com/cwtickle/danoniplus/pull/1036) )
- 🛠️ The process of creating an empty sprite is shifted from "createSprite" to "createEmptySprite" function. ( PR [#1038](https://github.com/cwtickle/danoniplus/pull/1038) )

## v21.2.0 ([2021-03-28](https://github.com/cwtickle/danoniplus/releases/tag/v21.2.0))
- ⭐ Changed to use a color set for light and dark depending on background conditions. ( PR [#1033](https://github.com/cwtickle/danoniplus/pull/1033) )
- ⭐ Changed ColorType: Type0 to automatically set the intermediate color to black if it is not specified and the background is light. ( PR [#1033](https://github.com/cwtickle/danoniplus/pull/1033) )
- 🛠️ Changed the data save flag switching button to be displayed on the Display settings screen as well. ( PR [#1032](https://github.com/cwtickle/danoniplus/pull/1032) )
- 🛠️ Update custom js sample in danoni3.html ( PR [#1034](https://github.com/cwtickle/danoniplus/pull/1034) )
- 🛠️ Organize the source code around the message display. ( PR [#1033](https://github.com/cwtickle/danoniplus/pull/1033) )
- 🛠️ Changed to wait for loading completion for dynamic loading of CSS files. ( PR [#1033](https://github.com/cwtickle/danoniplus/pull/1033) )

## v21.1.0 ([2021-03-19](https://github.com/cwtickle/danoniplus/releases/tag/v21.1.0))
- ⭐ Custom gauge lists can now be created for each chart. ( PR [#1024](https://github.com/cwtickle/danoniplus/pull/1024) )
- ⭐ Individual gauge settings, included chart header, now support split notation for each chart. ( PR [#1024](https://github.com/cwtickle/danoniplus/pull/1024) )
- ⭐ Changed so that initial arrow and freeze arrow colors (setColor2, frzColor2, ...) can be written to individual chart files in the same way as when all the chart numbers are same. ( PR [#1024](https://github.com/cwtickle/danoniplus/pull/1024) )
- ⭐ Changed the custom gauge list so that the specified list can be set in the life-based gauge, quota-based gauge and common setting file. ( Issue [#1026](https://github.com/cwtickle/danoniplus/pull/1026), PR [#1027](https://github.com/cwtickle/danoniplus/pull/1027) )
- 🛠️ Organize string-related source code. ( PR [#1024](https://github.com/cwtickle/danoniplus/pull/1024), [#1025](https://github.com/cwtickle/danoniplus/pull/1025) )

## v21.0.0 ([2021-03-12](https://github.com/cwtickle/danoniplus/releases/tag/v21.0.0))
- ⭐ Implemented initial arrow and freeze arrow color, as setColor and frzColor, settings for each chart sheet. ( Issue [#390](https://github.com/cwtickle/danoniplus/pull/390), PR [#1019](https://github.com/cwtickle/danoniplus/pull/1019) )
- ⭐ Changed to adopt the value of setColor, frzColor, setShadowColor, and frzShadowColor in the individual chart file when the chart files are split and all the chart numbers are same, if any. ( PR [#1019](https://github.com/cwtickle/danoniplus/pull/1019) )
- ⭐ Implemented shortcut keys for displaying the chart selector. ( PR [#1013](https://github.com/cwtickle/danoniplus/pull/1013) )
- ⭐ Support more than 20 keys for arrow and freeze arrow motion. ( PR [#1020](https://github.com/cwtickle/danoniplus/pull/1020) )
- 🛠️ Move deprecated functions to "danoni_legacy_function.js". ( PR [#1017](https://github.com/cwtickle/danoniplus/pull/1017) )
- 🛠️ Disabled shortcut keys for hidden buttons except for Difficulty setting and each screen movement when displaying chart selector. ( PR [#1013](https://github.com/cwtickle/danoniplus/pull/1013) )
- 🛠️ Changed the shadow arrow part of the key configuration screen to correspond to changes in ColorType. ( PR [#1013](https://github.com/cwtickle/danoniplus/pull/1013) )
- 🛠️ Organize the source code around the key configuration screen and level calculation tool. ( PR [#1016](https://github.com/cwtickle/danoniplus/pull/1016), [#1018](https://github.com/cwtickle/danoniplus/pull/1018), [#1021](https://github.com/cwtickle/danoniplus/pull/1021) )

 | **v21** | [**v20 ->**](Changelog-v20.html)
