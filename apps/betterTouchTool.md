# [BetterTouchTool](http://www.bettertouchtool.net/)

`免费`

摘要：

> Mac 辅助应用，用来代替默认的系统操作方式（组合键、修饰键、手势等），其目的是方便用户创造出更适合自身习惯的操作行为，是Mac上非常强大的触控板辅助工具。

打开应用之后，界面看上去是这样的，有点粗糙：

![应用界面][1]

不过提供了2个醒目的简单说明，添加应用这一个说明还算清晰，另一个...好吧，在这里大家一起来看看怎么随心所欲地用BetterTouchControl(后面简称BTT)定制自己的快捷键、触控板手势吧。

<!--more-->

# 神奇的多点触控

先来看下Mac BookPro强大的Trackpad触控板吧，在“系统偏好设置——触控板”里可以看到系统自带的触控板`真人手势帮助`，常用的一些手势动作如下：

* **单指**：移动光标、轻拍点按、双击打开。 
* **双指**：辅助点按「即右键」、上下滚动、左右返回前进、放大或缩小、`旋转`、`双击智能缩放`、右侧边缘向左滑动呼出「通知中心」。
* **三指**：文本选择、窗口拖动、轻拍显示词语翻译「需下载相关词典」、张开显示桌面「全屏应用下无效」、捏拢显示 Launchpad。 
* **四指**：左右切换全屏应用、上推显示 Mission Control、下推预览当前应用所有窗口。

其实触控板还可以识别许多其他的手势动作，比较便于我们操作的手势动作如下：

* 单手指
	* 单指轻拍上边中点 
	* 单指轻拍下边中点 
	* 单指轻拍左边中点 
	* 单指轻拍右边中点
* 双手指
	* 中指拍住中央食指轻拍面板(Tipap left) 
	* 食指拍住中央中指轻拍面板(Tipap right)
* 三手指
	* 两指轻拍住，第三拍中（左，右）
	* 右二指固定拍住，左一上（下）滑
* 四手指
	* 中指无名小拍住，食单击
	* 食中指无名拍住，小单击
* 五手指
	* 五手指上滑 
	* 五手指下滑 
	* 五手指左滑 
	* 五手指右滑 
	* 五手指轻拍

全部操作的中英文对照可以看[这里](../resource/magic_trackpad.md)。

# BTT自定义触控板

虽然自带的多点触控功能已经很强大，不过我们可以利用BTT定义一些属于自己的手势动作。系统自带的手势大部分只能在OS X自带的应用里使用，而BTT则允许你为任何应用配置属于它的手势。

所以，使用BTT自定义手势动作的第一步就是选择应用，在下图中红色标记的区块1即可以添加，删除应用，这里以markdown编辑器Mou为例子：

![BTT设置][2]

选择应用之后，就可以设置该应用下特殊的手势动作了。手势动作的设置相当简单，只需要将手势动作绑定到该应用的快捷键即可。比如我们想用`Tipap left`来保存md文件，只需要绑定Tipap left到`⌘+s`即可，上图中蓝色区块下方区域即为该设置。设置完成之后，就可以中指拍住中央食指轻拍面板来保存Mou中的文件了，很方便吧。

设置时还需要注意图中区域3的设备选择区，我们前面提到的都是苹果笔记本自带的触控板，所以新建立的操作方式就是 `Add New Gesture`。

# BTT 自定义快捷键

实际上，我们还可以利用BTT重新绑定Keyboard。大家知道在印象笔记中插入链接的快捷键是`⌘+K`，而在Mou下插入链接的快捷键是`Ctrl-Shift-L`，为了统一风格，可以选择将印象笔记中插入链接的方式改为Ctrl-Shift-L。一是因为自己习惯了Mou下的快捷键，另一个是因为Mou下`⌘+K`为插入内联代码，如果将它统一为印象笔记下的插入链接，那么插入内联代码的快捷键就会失效。

此外，还可以将印象笔记中的缩进方式改为Mou的快捷键，如下：

Mou   	|  印象笔记  | 描述
---    	|  --- 		| ---
⇧⌃L   	|  ⌘k			| 插入链接
⌘]    	|  ⌘⇧] 		| 增加缩进级别
⌘[    	|  ⌘⇧[ 		| 降低缩进级别
⌃L			|  ⌘⇧U		| 转换为无序列表
⇧⌃1		|  ⌘⇧D		| 插入时间
⇧⌃2		|  ⌘⇧T		| 插入日期

在设置BTT时，需要注意下面问题：

* 在将手势操控设置关联到默认快捷键后，该快捷键依然可以操作；
* 若自定义的「手势」与系统指定「手势」冲突，软件会有提示；
* 设置 Global 对象时，所有操作代表整个系统而不是某应用程序。

# 窗口管理

BTT有快速让`窗口并排显示`的功能(Window Snapping)，可以在**Advanced-Action Settings-Window Snapping**标签里把Window Snapping Enabled的选项勾上就OK了。这样，移动窗口之后会自动出现阴影区域，停止移动窗口就会铺满阴影，如下：

![窗口并排显示][5]

这样方便我们在同一个窗口一边看文档，一边工作。

另外，也可以快速对窗口进行位置大小的调整(Window Moving & Resizing)。OS X里调整程序窗口大小的原始方法比较不方便――需要先点击一下要操作的窗口，把它拿到最前面，然后在窗口四边才能使用三指移动。用BTT就简单多了，在**Advanced-Action Settings-Window Moving & Resizing**里指定相应的功能键即可方便快捷对窗口大小进行调整。

# 其他功能

BTT还提供了强大的导入导出功能，方便我们在不同机器使用相同的配置。此外，还有强大的`Show Live View`，可以显示你当前的全局手势动作，这个功能是相当之爽啊。

一个简单的全局触控板设置如下：

![全局触控板配置][3]

在Show Live View中看下效果吧：

![触控效果检测][4]

当然，上面功能都是需要开启BetterTouchControl的，最好是设置开机启动。

**参考**

[Mac 触控板增强神器：BetterTouchTool 上手指南](http://sspai.com/27094)  
[BetterTouchTool的偏好设置](http://www.zhu.cm/mac-bettertouchtool-tutorial-preferences.html)  

[1]: http://xuelangzf-github.qiniudn.com/apps_betterTouchControl_view.png
[2]: http://xuelangzf-github.qiniudn.com/apps_betterTouchControl_etc.png
[3]: http://xuelangzf-github.qiniudn.com/apps_betterTouchControl_global.png
[4]: http://xuelangzf-github.qiniudn.com/apps_betterTouchControl_show.gif
[5]: http://xuelangzf-github.qiniudn.com/apps_betterTouchControl_snap.png

---
[![](../resource/apps.png)](http://github.com/xuelangZF/MacOSX/blob/gh-pages/apps/apps_summary.md)