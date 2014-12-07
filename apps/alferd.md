# [Alferd](http://www.alfredapp.com/)

`免费|付费`

先来一睹芳容：

![Alferd芳容][1]

池建强老师这样夸她：

> Mac 平台上最为传奇的效率作品，誉为神兵利器毫不为过。

池老师还写了一篇文章：[神兵利器——Alfred](http://www.cnblogs.com/chijianqiang/p/alfred.html)。随便搜一下Alferd，保管找到一大堆有用文章来，连知乎这种非技术网站都有一堆Alferd的回答。

那么Alferd是什么？官网这么介绍：

> Alfred saves you time when you search for files online or on your Mac. Be more productive with hotkeys, keywords and file actions at your fingertips.

相信你用了后，会爱不释手，因为它是提高效率的神器！

## 免费版

免费版可以使用以下功能：

1. 打开应用和文件

	用Option + Space呼出Alfred后，输入应用程序的部分名字，就可以定位到应用了。

	当然也可以搜索文件，有4个关键字open、find、in、tags来对文件进行搜索。in、open、tags分别根据文件内容、文件名、文件标签来搜索文件然后直接打开，find根据文件名定位文件的位置，如下图：
	
	!["in"搜索文件内容][3]

2. 快速搜索Web

	使用内置的web搜索关键词或者是自定义的关键词来快速搜索，内置关键词如下图：
	
	![快速搜索web][2]

	如果你想自定义一个mac的关键词，用来搜索App Store中的应用，可以像这样子：
	
		Search URL：macappstore://ax.search.itunes.apple.com/WebObjects/MZSearch.woa/wa/search?q={query}
		Title：MacApp
		Keyword：mac

3. `计算器`：无须触发关键字，输入算式，按回车会直接把计算结果放到剪贴板中。

4. 词典：可以使用MAC自带的词典工具，搜索结果依赖于你安装的词库，搜索关键字 `define`。

5. 快速使用`系统工具`：使用`hide app`来隐藏窗口，`quit app`来关掉应用，或者是`force quit`强制关闭应用。此外，可以使用sleep命令来休眠，或者是lock来锁定计算机，或者是emptytrash来清空垃圾箱，此外还有restart、shutdown、logout等命令。

## Powerpack增强功能

免费的Alferd功能和Spotlight基本一样，没有太大的优势，不过在买了[Powerpack](http://www.alfredapp.com/powerpack/)之后，你才能真正体会到Alferd的强大之处。

1. 搜索通讯录：Alferd会搜索联系人，显示邮箱、手机号码等，在邮箱上回车即新建右键，并指定联系人为邮件接收人。
2. 剪贴板历史： Alferd会保存剪贴板历史，可以自定义快捷键或者关键字来呼出剪贴板历史，如下图：
	
	![剪贴板历史][4]

	选择相应的剪贴板之后，就会复制剪贴板内容，如果当前光标位置可编辑，会直接复制到当前位置。此外，可以用指定关键词(默认为`clear`)来清除剪贴板历史，也可以指定剪贴板不记录的程序，比如1password。

3. 快速打开命令行终端：用 > 后面加命令来打开终端(可以指定iTerm2)并执行明林。
4. 1passwrod：快速登录1password中保存的标签页。需要注意的是如果Alfred显示`Unable to find 1Password Data`的话，需要打开1Password的`启用与第三方应用整合`这个选项，如下图：
	![1password整合][5]
5. iTunes迷你播放器：用Alferd来播放iTune里的音乐或者博客，很cool，如图：
	![迷你播放器][6]

每个功能都有很大的配置自由度，可以定制自己的Alferd，根据配置选项也可以发现其他的用法。当然了，这些配置都可以方便地导入导出。

## workflows

上面的功能很吸引人，不过真正吸引人的是workflows。它支持用ruby，python,perl等等等等写入脚本，让alferd可以实现更多的功能，这些功能让键盘流的大侠们工作效率直线上升。

Alferd[官网论坛](http://www.alfredforum.com/forum/3-share-your-workflows)提供了许多workflows，此外[这里](http://www.alfredworkflow.com/)收集了快600个workflows，应该能在这里发现自己的最爱。安装workflows的方法很简单，只需要下载一个后缀名为workflows的文件，双击加载就ok了。

下边简单推荐几个我已经试用的，很好用。

* [新建文件](http://ianisted.co.uk/new-finder-file-alfred-2)
* 豆瓣搜索
* 有道翻译

不一一介绍了，各取所需吧。

参考  
[丢掉鼠标－Mac神软Alfred使用手册1](http://wellsnake.com/jekyll/update/2014/06/15/001/)
[借助 Alfred 2 的 Workflows 功能可以做哪些好玩的事情？](http://www.zhihu.com/question/20656680)  
[有哪些工具或者软件堪称神器？](http://www.zhihu.com/question/20772002)  

---
[![](../resource/apps.png)](http://github.com/xuelangZF/MacOSX/blob/gh-pages/apps/apps_summary.md)

[1]: http://xuelangzf-github.qiniudn.com/2014-11-11_Alferd.png
[2]: http://xuelangzf-github.qiniudn.com/apps_alferd_web.png
[3]: http://xuelangzf-github.qiniudn.com/apps_alferd_in.png
[4]: http://xuelangzf-github.qiniudn.com/apps_alferd_clibboard.png
[5]: http://xuelangzf-github.qiniudn.com/apps_alferd_1p.png
[6]: http://xuelangzf-github.qiniudn.com/apps_alferd_itunes.png