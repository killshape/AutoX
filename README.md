# Auto.js And Autox.js


## Introduction

A JavaScript runtime environment and development environment on Android platform supporting accessibility services, with development goals similar to JsBox and Workflow.


This project was obtained from [hyb1996](https://github.com/hyb1996/Auto.js) autojs, and named Autox.js (autojs modified version).
You are looking at the project based on the original 4.1 version.
Later we will introduce how to develop and run the project itself, and welcome more developers to participate in the maintenance and upgrade of this project. [hyb1996](https://github.com/hyb1996/Auto.js) uses the
[Mozilla Public License Version 2.0](https://github.com/hyb1996/NoRootScriptDroid/blob/master/LICENSE.md)
+*Non-Commercial Use** This product is licensed under the [GPL-V2](https://opensource.org/licenses/GPL-2.0) for a variety of reasons.
Both the other contributors and the use of this product are required to use it in accordance with MPL-2.0+Non-Commercial Use and GPL-V2.

Regarding the two protocols:

* GPL-V2 (https://opensource.org/licenses/GPL-2.0)
* MPL-2 (https://www.mozilla.org/MPL/2.0)

### Now for Autox.js:

* Autox.js documentation: http://doc.autoxjs.com/
* Open source address https://github.com/kkevsekk1/AutoX
* pc-side development [VS Code plug-in] (https://marketplace.visualstudio.com/items?itemName=aaroncheng.auto-js-vsce-fixed)
* Official forum: [www.autoxjs.com](http://www.autoxjs.com)
* autoxjs[changelog](CHANGELOG.md)

### Autox.js download address:
[https://github.com/kkevsekk1/AutoX/releases](https://github.com/kkevsekk1/AutoX/releases)  
If the download is too slow you can right click and copy the link address of the APK file in Release Assets and paste it into [http://toolwa.com/github/](http://toolwa.com/github/) and other github acceleration sites to download

#### APK version description:
- universal: universal version (don't care about the size of the installation package / lazy to choose, use this version, including the following 2 CPU architecture so)
- armeabi-v7a: 32-bit ARM device (preferred for spare machines)
- arm64-v8a: 64-bit ARM device (mainstream flagship)

### Features

1. easy-to-use auto-operation functions implemented by accessibility services
2. Hover window recording and running
3. more professional & powerful selector API to provide find, traverse, get information, manipulate controls on the screen, etc. Similar to Google's UI testing framework UiAutomator, you can also use him as a mobile version of the UI testing framework
4. using JavaScript as the scripting language , and support code completion , variable renaming , code formatting , find and replace , etc. , you can use as a JavaScript IDE
5. support the use of e4x to write the interface, and can package JavaScript as an apk file, you can use it to develop widget applications
6. Support using Root permission to provide more powerful screen click, swipe, record function and run shell commands. Recording recording can produce js files or binary files, the playback of recorded actions is more smooth
7. provide functions to intercept screen, save screenshot, find color of image, find map, etc.
8. can be used as Tasker plug-in, combined with Tasker can be competent for daily workflow
9. With interface analysis tools, similar to Android Studio's LayoutInspector, which can analyze the interface level and scope, and get the information of controls on the interface.

This software is different from Keystroke Wizard and other software, the main differences are:

1. Auto.js is mainly aimed at automation and workflow, and is more convenient for daily work, such as automatically blocking notifications when starting games, one-click WeChat video with specific contacts (the problem has appeared on Zhihu, and it is difficult for the elderly to perform complex operations and children to WeChat video)
2. Auto.js is more compatible. Coordinate-based keystroke wizard and script wizard are prone to resolution problems, while the control-based Auto.js does not have this problem
3. Auto.js does not require root access to perform most tasks. Only functions that require precise coordinate clicks and swipes require root access.
4. Auto.js can provide functions such as interface writing, not just exist as a scripting software

### autojs information

* Official forum: [autojs.org](http://www.autojs.org)
* Documentation: Online documentation can be viewed [here](https://hyb1996.github.io/AutoJs-Docs/). The documentation is still not perfect.
*

Examples: Some examples can be viewed at [here](https://github.com/hyb1996/NoRootScriptDroid/tree/master/app/src/main/assets/sample), or viewed and run directly within the application.

### Architecture diagram

To be added, but is anyone really interested in this? Feel free to contact me to exchange

## About License

##### This product is licensed under the [GPL-V2](https://opensource.org/licenses/GPL-2.0) license

##### For historical reasons also has to follow the [autojs project](https://github.com/hyb1996/Auto.js) agreement:

Based on [Mozilla Public License Version 2.0](https://github.com/hyb1996/NoRootScriptDroid/blob/master/LICENSE.md) and with the following additional terms:

* **Non-Commercial Use** - The source code and binaries of this project and its derivative projects may not be used for any commercial and for-profit purposes

#### Can this Autox.js be GPL-V2?

It should be easy to understand about GPL-V2, the famous linux license. However, there are many articles about MPL-2.0 that are stuck with MPL-1.1, which causes problems for many domestic developers.
This is a more standard [translation](https://github.com/rachelzhang1/MPL2.0_zh-CN/blob/93d2feec60d8b0b5a54a1843c866994af4610d4f/Mozilla_Public_License_2.0) _Simplified_Chinese_Reference.txt)
You can study it if you are interested.

#### Note to code contributors:

No one declared the license in the original article that is MPL2.0, new files or modify (limited to repair your own) code using GPL-V2, you need to do the relevant declaration.

``` java
// SPDX-License-Identifier: GPL-2.0
// Declare your copyright
```

#### others use Autox.js, do deep development please note

* If you use code with GPL-2.0 declaration or compiled binary. You need to open source all your code.
* If you are using only MPL-2.0 stuff, you need to open source your modified related code.

#### Open source and commercial aside from this product

* Open source is not the same as free to use, and open source is not the same as prohibiting commercial use!
* Open source stuff can be commercially available, but you need to open source it as specified!
* Commercial products can be open source, like redhat!
* not according to the open source protocol to use open source products, that can understand the source of openwrt, and the recent years of domestic infringement cases!

#### about js scripts developed by others to run on this. Whether you need to follow the GPL-2.0 for open source

* That's your freedom, not restricted by this agreement, just like linux running software

#### Is it possible to use this product or autojs product commercially?

* Whether this product is commercially available depends on the original autojs, as many features and code are currently copyrighted by autojs.
* Whether autojs is commercially available depends on your understanding of the " **non-commercial use**" attached to it and its legal benefits.
* This product will not be used commercially with autojs anyway.

#### Compiler related:
Command description: Run the command in the project root directory, if using Windows powerShell < 7.0, use the command containing ";"

##### Install debug version locally to device:
```shell
. /gradlew inrt:assembleTemplateDebug && . /gradlew inrt:cp2APPDebug && . /gradlew app:assembleV6Debug && . /gradlew app:installV6Debug
# or
. /gradlew inrt:assembleTemplateDebug ; . /gradlew inrt:cp2APPDebug ; . /gradlew app:assembleV6Debug ; . /gradlew app:installV6Debug
```
The generated debug version of the APK file is under app/build/outputs/apk/v6/debug, using the default signature

##### local build release version:
```shell
. /gradlew inrt:assembleTemplate && . /gradlew inrt:cp2APP && . /gradlew app:assembleV6
# or
. /gradlew inrt:assembleTemplate ; . /gradlew inrt:cp2APP ; . /gradlew app:assembleV6
```
The generated APK file is unsigned and is under app/build/outputs/apk/v6/release and needs to be signed before it can be installed

##### Local Android Studio to run the debug version to the device:
First run the following command:

```shell
. /gradlew inrt:assembleTemplate && . /gradlew inrt:cp2APP
# or
. /gradlew inrt:assembleTemplate ; . /gradlew inrt:cp2APP
```

Then click the Android Studio Run button

##### Local Android Studio compiles the release and signs it:
Start by running the following command:

```shell
. /gradlew inrt:assembleTemplate && . /gradlew inrt:cp2APP
# or
. /gradlew inrt:assembleTemplate ; . /gradlew inrt:cp2APP
```

Click on Android Studio menu "Build" -> "Generate Signed Bundle /APK..." -> check "APK" -> "Next" -> select or create a new certificate -> "Next" -> select "v6Release" -> "Finish"
The generated APK file is under app/v6/release

