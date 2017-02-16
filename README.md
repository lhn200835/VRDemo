# VR #
虚拟现实（Virtual Reality）技术是一种可以创建和体验虚拟世界的计算机仿真系统，它利用计算机生成一种模拟环境，是一种多源信息融合的、交互式的三维动态视景和实体行为的系统仿真, 使用户沉浸到该环境中。

* [Wikipedia](https://en.wikipedia.org/wiki/Virtual_reality)
* [视频](http://v.youku.com/v_show/id_XMTQ5NTk4ODE2MA==.html?&f=27013492&from=y1.2-3.4.1&spm=a2h0j.8191423.item_XMTQ5NTk4ODE2MA==.A)

# VR产品 #
* [Google VR](https://vr.google.com/)
* [Oculus](https://www.oculus.com/)
* [HTC Vivi](https://www.vive.com/cn/)


# Google VR for Android#
Google VR for Android支持DayDream和Cardboard。

* [Github](https://github.com/googlevr/gvr-android-sdk)
* [Document](https://developers.google.com/vr/android/)
* [API Reference](https://developers.google.com/vr/android/reference_overview)

## SDK下载 ##
使用git命名下载或者直接在github上下载压缩包

	git clone https://github.com/googlevr/gvr-android-sdk.git

## 官方Sample运行 ##
>注意build失败可使用本地gradle

### simplepanowidget ###
simplepanowidget展示了印加文明遗迹马丘比丘的全景图(Panorama)

![](img/simplepanowidget.gif)


在真机上运行时，会有一个Cardboard选项。

![](img/cardboard_option.jpg)

点击上图红色框中的按钮即可进入Cardboard模式。

![](img/cardboard_mode.jpg)

Demo代码的主要逻辑就是加载一张全景图放入VrPanoramaView中。

	istr = assetManager.open("andes.jpg");//加载assets目录下的全景图
	panoWidgetView.loadImageFromBitmap(BitmapFactory.decodeStream(istr), panoOptions);

全景图片andes是由两张图片组成，上面一张是给左眼看，下面一张是给右眼看。

![](img/stereo.png)


###  ###