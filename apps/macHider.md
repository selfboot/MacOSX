# [MacHider](http://macpaw.com/support/hider/knowledgebase/machider-support)

`付费`

是不是有一些文件、图片不想被别人看到？作为程序员，你当然可以通过设置权限阻止别人来看。不过我们有更简单的方法，那就是用MacHider来隐藏文件了，如下：

![MacHider界面][1]

界面有点不够Mac，不过这是老版了，有最新版的Hider2了。

**隐藏文件**

只需要打开MacHider（需要输入为MacHider设置的专有应用密码），将隐私文件拖入到上图打马赛克的区域，点击软件右侧的`Hide`开关按钮，然后隐私文件就会从你的电脑“消失”。下面是我将桌面上的一个图片apps_alferd_in.png隐藏前后用ls命令查看的结果

	➜  ~  ls -l Desktop
	total 296
	-rw-r--r--@ 1 feizhao  staff  107520 Nov 16 21:32 Thumbs.db
	-rw-r--r--  1 feizhao  staff   21675 Nov 29 11:19 apps_alferd_in.png
	-rw-r-----@ 1 feizhao  staff   14848 Nov 11 21:51 套餐余量.xls
	➜  ~  ls -l Desktop
	total 248
	-rw-r--r--@ 1 feizhao  staff  107520 Nov 16 21:32 Thumbs.db
	-rw-r-----@ 1 feizhao  staff   14848 Nov 11 21:51 套餐余量.xls

此外，MacHider可以设置隐私群组，将隐私文件分门别类的放在相应群组。

**显示文件**

显示文件也很简单，只需要在相应MacHider群组找到自己需要显示的文件，然后点击右侧的`Hide`开关按钮到OFF即可，这样就可以浏览隐私文件了。

[1]:http://xuelangzf-github.qiniudn.com/2014-11-11_MacHider.png